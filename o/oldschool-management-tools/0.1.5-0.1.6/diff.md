# Comparing `tmp/oldschool_management_tools-0.1.5.tar.gz` & `tmp/oldschool_management_tools-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oldschool_management_tools-0.1.5.tar", max compression
+gzip compressed data, was "oldschool_management_tools-0.1.6.tar", max compression
```

## Comparing `oldschool_management_tools-0.1.5.tar` & `oldschool_management_tools-0.1.6.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1315 2023-04-10 13:00:12.829587 oldschool_management_tools-0.1.5/oldschool_management_tools/calendar_items/calendar_item.py
--rw-r--r--   0        0        0      907 2023-04-10 14:57:09.545095 oldschool_management_tools-0.1.5/oldschool_management_tools/mgmt_tools_cmd.py
--rw-r--r--   0        0        0     4804 2023-04-10 14:52:09.479176 oldschool_management_tools-0.1.5/oldschool_management_tools/oldschool_management_tools.py
--rw-r--r--   0        0        0      352 2023-04-15 13:08:32.632526 oldschool_management_tools-0.1.5/oldschool_management_tools/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-10 12:00:27.259073 oldschool_management_tools-0.1.5/oldschool_management_tools/README.md
--rw-r--r--   0        0        0      698 2022-11-06 16:58:42.825790 oldschool_management_tools-0.1.5/oldschool_management_tools/special_prompts/special_prompts.py
--rw-r--r--   0        0        0        0 2023-04-10 12:00:27.259073 oldschool_management_tools-0.1.5/oldschool_management_tools/tests/__init__.py
--rw-r--r--   0        0        0      447 2023-04-09 07:24:56.391208 oldschool_management_tools-0.1.5/oldschool_management_tools/testy.py
--rw-r--r--   0        0        0      440 2023-04-15 13:12:16.920724 oldschool_management_tools-0.1.5/pyproject.toml
--rw-r--r--   0        0        0        4 2022-10-15 13:56:15.832011 oldschool_management_tools-0.1.5/README.md
--rw-r--r--   0        0        0      476 1970-01-01 00:00:00.000000 oldschool_management_tools-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1315 2023-04-10 13:00:12.829587 oldschool_management_tools-0.1.6/oldschool_management_tools/calendar_items/calendar_item.py
+-rw-r--r--   0        0        0     5598 2023-05-08 17:21:30.876195 oldschool_management_tools-0.1.6/oldschool_management_tools/calendar_tools.py
+-rw-r--r--   0        0        0     1110 2023-05-08 17:15:45.368647 oldschool_management_tools-0.1.6/oldschool_management_tools/mgmt_tools_cmd.py
+-rw-r--r--   0        0        0        0 2023-04-10 12:00:27.259073 oldschool_management_tools-0.1.6/oldschool_management_tools/README.md
+-rw-r--r--   0        0        0      698 2022-11-06 16:58:42.825790 oldschool_management_tools-0.1.6/oldschool_management_tools/special_prompts/special_prompts.py
+-rw-r--r--   0        0        0        0 2023-04-10 12:00:27.259073 oldschool_management_tools-0.1.6/oldschool_management_tools/tests/__init__.py
+-rw-r--r--   0        0        0      447 2023-04-09 07:24:56.391208 oldschool_management_tools-0.1.6/oldschool_management_tools/testy.py
+-rw-r--r--   0        0        0      457 2023-05-08 17:23:37.950971 oldschool_management_tools-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0        4 2022-10-15 13:56:15.832011 oldschool_management_tools-0.1.6/README.md
+-rw-r--r--   0        0        0      511 1970-01-01 00:00:00.000000 oldschool_management_tools-0.1.6/PKG-INFO
```

### Comparing `oldschool_management_tools-0.1.5/oldschool_management_tools/calendar_items/calendar_item.py` & `oldschool_management_tools-0.1.6/oldschool_management_tools/calendar_items/calendar_item.py`

 * *Files identical despite different names*

### Comparing `oldschool_management_tools-0.1.5/oldschool_management_tools/mgmt_tools_cmd.py` & `oldschool_management_tools-0.1.6/oldschool_management_tools/mgmt_tools_cmd.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 import cmd
-from oldschool_management_tools.oldschool_management_tools import parse_day, show_day_sched, prompt_day_tasks, fill_prep, wipe_prep
-
+from oldschool_management_tools.calendar_tools import parse_day, prompt_day_tasks
+from oldschool_management_tools.calendar_tools import CalendarReader
 
 
 class MgmtToolsCmd(cmd.Cmd):
     intro = "Welcome to Old School Management Tools"
     prompt = "(mgmt) "
 
+    def __init__(self):
+        super(MgmtToolsCmd, self).__init__()
+        self.calendar_reader = CalendarReader()
+
     def do_prompt_tasks(self, day):
         parsed_day = parse_day(day)
         prompt_day_tasks(parsed_day)
 
     def do_show_sched(self, day):
         parsed_day = parse_day(day)
-        show_day_sched(parsed_day)
+        self.calendar_reader.show_day_sched(parsed_day)
 
     def do_fill_prep(self, day):
         parsed_day = parse_day(day)
-        fill_prep(parsed_day)
+        self.calendar_reader.fill_prep(parsed_day)
 
     def do_wipe_prep(self, day):
         parsed_day = parse_day(day)
-        wipe_prep(parsed_day)
+        self.calendar_reader.wipe_prep(parsed_day)
 
     def do_die(self, args):
         return True
 
 
     def do_exit(self, args):
         return True
```

### Comparing `oldschool_management_tools-0.1.5/oldschool_management_tools/oldschool_management_tools.py` & `oldschool_management_tools-0.1.6/oldschool_management_tools/calendar_tools.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,46 +2,107 @@
 
 import win32com.client
 from win32com import client
 from oldschool_management_tools.special_prompts.special_prompts import SPECIAL_PROMPTS
 from os import system
 from oldschool_management_tools.calendar_items.calendar_item import CalendarItem
 from dataclasses import dataclass
+from re import match as re_match
+import yaml
 
 # Ideas:
 #  - See allocated time per day
 #  - Plan in breaks
 #  - Draw schedule in hours
 
 # Do the work where it is fast :)
 
 CATEGORIES_REQUIRING_PREP = ["green"]
 PREP_DURATION = 15
 system('color')
 
+class CalendarReader:
 
-def get_calendar(begin, end) -> client.CDispatch:
-    outlook = client.Dispatch('Outlook.Application').GetNamespace('MAPI')
-    calendar = outlook.getDefaultFolder(9).Items
-    calendar.IncludeRecurrences = True
-    calendar.Sort('[Start]')
-
-    restriction = "[Start] >= '" + begin.strftime('%d/%m/%Y') + "' AND [END] <= '" + end.strftime('%d/%m/%Y') + "'"
-    calendar = calendar.Restrict(restriction)
-    return calendar
-
-
-def get_day_cal(date: datetime):
-    return get_calendar(date, date + timedelta(days=1))
-
-
-def print_cal(cal):
-    for outlook_apt in cal:
-        cal_apt = CalendarItem.from_outlook_apt(outlook_apt)
-        cal_apt.print()
+    def __init__(self):
+        with open("management_tools_config.yaml", "r") as stream:
+            config = yaml.safe_load(stream)
+            self.config = config
+
+    def get_calendar(self, begin, end) -> client.CDispatch:
+        outlook = client.Dispatch('Outlook.Application').GetNamespace('MAPI')
+        calendar = outlook.getDefaultFolder(9).Items
+        calendar.IncludeRecurrences = True
+        calendar.Sort('[Start]')
+
+        restriction = "[Start] >= '" + begin.strftime('%d/%m/%Y') + "' AND [END] <= '" + end.strftime(
+            '%d/%m/%Y') + "'"
+        calendar = calendar.Restrict(restriction)
+        return calendar
+
+    def get_day_cal(self, date: datetime):
+        return self.get_calendar(date, date + timedelta(days=1))
+
+    def fill_prep(self, parsed_day=datetime.today()):
+        valid_apts = self.get_valid_apts(self.get_day_cal(parsed_day))
+        apts = [CalendarItem.from_outlook_apt(apt) for apt in valid_apts]
+        free_slots: list[TimeSlot] = []
+        last_apt_end_time: datetime = None
+        new_apts = []
+
+        for apt in apts:
+            if not free_slots:
+                free_slots.append(TimeSlot(apt.start_datetime.replace(hour=8, minute=0, second=0), apt.start_datetime))
+            elif last_apt_end_time and free_slots[-1].end_datetime < apt.start_datetime \
+                    and last_apt_end_time < apt.start_datetime:
+                new_free_slot = TimeSlot(last_apt_end_time, apt.start_datetime)
+                free_slots.append(new_free_slot)
+
+            if apt.category.lower() in CATEGORIES_REQUIRING_PREP:
+                last_free_slot = free_slots[-1]
+                if last_free_slot.end_datetime < apt.end_datetime:
+                    prep_slot = TimeSlot(last_free_slot.end_datetime - timedelta(minutes=PREP_DURATION),
+                                         last_free_slot.end_datetime)
+                    last_free_slot.end_datetime = last_free_slot.end_datetime - timedelta(minutes=PREP_DURATION)
+                    if last_free_slot.end_datetime - timedelta(minutes=PREP_DURATION) <= last_free_slot.start_datetime:
+                        free_slots.pop()
+                new_apts.append(CalendarItem(f"Prep {apt.name}", "Desk", "yellow",
+                                             prep_slot.start_datetime, prep_slot.start_datetime.time(),
+                                             prep_slot.end_datetime, prep_slot.end_datetime.time()))
+            last_apt_end_time = apt.end_datetime
+
+        [add_apt(valid_apts, apt) for apt in new_apts]
+
+    def show_day_sched(self, parsed_day=datetime.today()):
+        cal = self.get_day_cal(parsed_day)
+        self.print_cal(cal)
+
+    def wipe_prep(self, parsed_day=datetime.today()):
+        cal = self.get_day_cal(parsed_day)
+        cal_item_num = 0
+        try:
+            while cal.Count > cal_item_num + 1:
+                appt = cal[cal_item_num]
+                cal_item = CalendarItem.from_outlook_apt(appt)
+
+                if cal_item.category == "yellow" and cal_item.name.startswith("Prep"):
+                    appt.Delete()
+                    cal = self.get_day_cal(parsed_day)
+                else:
+                    cal_item_num = cal_item_num + 1
+        except IndexError:
+            # Probably fine
+            pass
+
+    def get_valid_apts(self, cal):
+        return [apt for apt in cal if not re_match(self.config['ignore_subject_regex'], str(apt.Subject))]
+
+    def print_cal(self, cal):
+        for outlook_apt in self.get_valid_apts(cal):
+            cal_apt = CalendarItem.from_outlook_apt(outlook_apt)
+            cal_apt.print()
 
 
 def start_of_day(day: date) -> datetime:
     return datetime.combine(day, time())
 
 
 def parse_day(day) -> datetime:
@@ -52,18 +113,14 @@
             return start_of_day(date.today()) + timedelta(days=1)
         case d if day.isnumeric():
             return start_of_day(date.today()) + timedelta(days=int(d))
         case _:
             raise ValueError(f"Bad day [{day}]")
 
 
-def show_day_sched(parsed_day=datetime.today()):
-    cal = get_day_cal(parsed_day)
-    print_cal(cal)
-
 
 def prompt_day_tasks(parsed_day=datetime.today()):
     for spec_prompt in SPECIAL_PROMPTS:
         spec_prompt.show()
     apts = [CalendarItem.from_outlook_apt(apt) for apt in cal]
     for apt in apts:
         if apt.category.lower() in CATEGORIES_REQUIRING_PREP:
@@ -72,62 +129,14 @@
 
 @dataclass
 class TimeSlot:
     start_datetime: datetime
     end_datetime: datetime
 
 
-def fill_prep(parsed_day=datetime.today()):
-    cal = get_day_cal(parsed_day)
-    apts = [CalendarItem.from_outlook_apt(apt) for apt in cal]
-    free_slots: list[TimeSlot] = []
-    last_apt_end_time: datetime = None
-    new_apts = []
-
-    for apt in apts:
-        if not free_slots:
-            free_slots.append(TimeSlot(apt.start_datetime.replace(hour=8, minute=0, second=0), apt.start_datetime))
-        elif last_apt_end_time and free_slots[-1].end_datetime < apt.start_datetime \
-                and last_apt_end_time < apt.start_datetime:
-            new_free_slot = TimeSlot(last_apt_end_time, apt.start_datetime)
-            free_slots.append(new_free_slot)
-
-        if apt.category.lower() in CATEGORIES_REQUIRING_PREP:
-            last_free_slot = free_slots[-1]
-            if last_free_slot.end_datetime < apt.end_datetime:
-                prep_slot = TimeSlot(last_free_slot.end_datetime - timedelta(minutes=PREP_DURATION), last_free_slot.end_datetime)
-                last_free_slot.end_datetime = last_free_slot.end_datetime - timedelta(minutes=PREP_DURATION)
-                if last_free_slot.end_datetime - timedelta(minutes=PREP_DURATION) <= last_free_slot.start_datetime:
-                    free_slots.pop()
-            new_apts.append(CalendarItem(f"Prep {apt.name}", "Desk", "yellow",
-                                         prep_slot.start_datetime, prep_slot.start_datetime.time(),
-                                         prep_slot.end_datetime, prep_slot.end_datetime.time()))
-        last_apt_end_time = apt.end_datetime
-
-    [add_apt(cal, apt) for apt in new_apts]
-
-
-def wipe_prep(parsed_day=datetime.today()):
-    cal = get_day_cal(parsed_day)
-    cal_item_num = 0
-    try:
-        while cal.Count > cal_item_num + 1:
-            appt = cal[cal_item_num]
-            cal_item = CalendarItem.from_outlook_apt(appt)
-
-            if cal_item.category == "yellow" and cal_item.name.startswith("Prep"):
-                appt.Delete()
-                cal = get_day_cal(parsed_day)
-            else:
-                cal_item_num = cal_item_num + 1
-    except IndexError:
-        # Probably fine
-        pass
-
-
 def add_apt(cal: win32com.client.CDispatch, apt: CalendarItem):
     outlook = client.Dispatch('Outlook.Application')
     apt.print()
     appt = outlook.CreateItem(1)
     appt.Start = str(apt.start_datetime)[0:-6]
     appt.Subject = apt.name
     appt.Categories = apt.category + " Category"
```

### Comparing `oldschool_management_tools-0.1.5/oldschool_management_tools/special_prompts/special_prompts.py` & `oldschool_management_tools-0.1.6/oldschool_management_tools/special_prompts/special_prompts.py`

 * *Files identical despite different names*

