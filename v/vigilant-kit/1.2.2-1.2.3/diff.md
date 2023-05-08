# Comparing `tmp/vigilant_kit-1.2.2.tar.gz` & `tmp/vigilant_kit-1.2.3.tar.gz`

## Comparing `vigilant_kit-1.2.2.tar` & `vigilant_kit-1.2.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 vigilant_kit-1.2.2/.vigilant.env.example
--rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 vigilant_kit-1.2.2/bin/doc_generator.py
--rw-r--r--   0        0        0    31508 2020-02-02 00:00:00.000000 vigilant_kit-1.2.2/docs/actions.md
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 vigilant_kit-1.2.2/docs/browser_options.md
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 vigilant_kit-1.2.2/docs/native_selenium.md
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 vigilant_kit-1.2.2/docs/selenium_install.md
--rw-r--r--   0        0        0    11059 2020-02-02 00:00:00.000000 vigilant_kit-1.2.2/docs/tutorial_pytest.md
--rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 vigilant_kit-1.2.2/docs/vigilant_pytest.md
--rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 vigilant_kit-1.2.2/docs/vigilant_unittest.md
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 vigilant_kit-1.2.2/src/vgl_cli/install_dev_kit_command.py
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 vigilant_kit-1.2.2/src/vgl_cli/install_standalone_command.py
--rw-r--r--   0        0        0     5058 2020-02-02 00:00:00.000000 vigilant_kit-1.2.2/src/vgl_cli/install_webdriver_command.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 vigilant_kit-1.2.2/src/vgl_cli/run_selenium_command.py
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 vigilant_kit-1.2.2/src/vgl_cli/vgl.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vigilant_kit-1.2.2/src/vigilant/__init__.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 vigilant_kit-1.2.2/src/vigilant/logger.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vigilant_kit-1.2.2/src/vigilant/actions/__init__.py
--rw-r--r--   0        0        0     6038 2020-02-02 00:00:00.000000 vigilant_kit-1.2.2/src/vigilant/actions/assertions.py
--rw-r--r--   0        0        0     2585 2020-02-02 00:00:00.000000 vigilant_kit-1.2.2/src/vigilant/actions/finder.py
--rw-r--r--   0        0        0    11684 2020-02-02 00:00:00.000000 vigilant_kit-1.2.2/src/vigilant/actions/vigilant_actions.py
--rw-r--r--   0        0        0     5064 2020-02-02 00:00:00.000000 vigilant_kit-1.2.2/src/vigilant/actions/waiter.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 vigilant_kit-1.2.2/src/vigilant/driver/__init__.py
--rw-r--r--   0        0        0     3398 2020-02-02 00:00:00.000000 vigilant_kit-1.2.2/src/vigilant/driver/vigilant_driver.py
--rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 vigilant_kit-1.2.2/.gitignore
--rw-r--r--   0        0        0    35125 2020-02-02 00:00:00.000000 vigilant_kit-1.2.2/LICENSE
--rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 vigilant_kit-1.2.2/README.md
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 vigilant_kit-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 vigilant_kit-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 vigilant_kit-1.2.3/.vigilant.env.example
+-rw-r--r--   0        0        0     2503 2020-02-02 00:00:00.000000 vigilant_kit-1.2.3/bin/doc_generator.py
+-rw-r--r--   0        0        0    28724 2020-02-02 00:00:00.000000 vigilant_kit-1.2.3/docs/actions.md
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 vigilant_kit-1.2.3/docs/browser_options.md
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 vigilant_kit-1.2.3/docs/native_selenium.md
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 vigilant_kit-1.2.3/docs/selenium_install.md
+-rw-r--r--   0        0        0    11059 2020-02-02 00:00:00.000000 vigilant_kit-1.2.3/docs/tutorial_pytest.md
+-rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 vigilant_kit-1.2.3/docs/vigilant_pytest.md
+-rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 vigilant_kit-1.2.3/docs/vigilant_unittest.md
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 vigilant_kit-1.2.3/src/vgl_cli/install_dev_kit_command.py
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 vigilant_kit-1.2.3/src/vgl_cli/install_standalone_command.py
+-rw-r--r--   0        0        0     5058 2020-02-02 00:00:00.000000 vigilant_kit-1.2.3/src/vgl_cli/install_webdriver_command.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 vigilant_kit-1.2.3/src/vgl_cli/run_selenium_command.py
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 vigilant_kit-1.2.3/src/vgl_cli/vgl.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vigilant_kit-1.2.3/src/vigilant/__init__.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 vigilant_kit-1.2.3/src/vigilant/logger.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vigilant_kit-1.2.3/src/vigilant/actions/__init__.py
+-rw-r--r--   0        0        0     6038 2020-02-02 00:00:00.000000 vigilant_kit-1.2.3/src/vigilant/actions/assertions.py
+-rw-r--r--   0        0        0     2585 2020-02-02 00:00:00.000000 vigilant_kit-1.2.3/src/vigilant/actions/finder.py
+-rw-r--r--   0        0        0    11684 2020-02-02 00:00:00.000000 vigilant_kit-1.2.3/src/vigilant/actions/vigilant_actions.py
+-rw-r--r--   0        0        0     5064 2020-02-02 00:00:00.000000 vigilant_kit-1.2.3/src/vigilant/actions/waiter.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 vigilant_kit-1.2.3/src/vigilant/driver/__init__.py
+-rw-r--r--   0        0        0     3398 2020-02-02 00:00:00.000000 vigilant_kit-1.2.3/src/vigilant/driver/vigilant_driver.py
+-rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 vigilant_kit-1.2.3/.gitignore
+-rw-r--r--   0        0        0    35125 2020-02-02 00:00:00.000000 vigilant_kit-1.2.3/LICENSE
+-rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 vigilant_kit-1.2.3/README.md
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 vigilant_kit-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 vigilant_kit-1.2.3/PKG-INFO
```

### Comparing `vigilant_kit-1.2.2/bin/doc_generator.py` & `vigilant_kit-1.2.3/bin/doc_generator.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,37 +44,39 @@
     all_functions.sort(key=lambda x: x['func_name'])
 
     # Write the table of contents and the functions to the output file
     with open(output_file, "w") as f:
         f.write("# Table of Contents\n\n")
         for func in all_functions:
             func_name = func['func_name']
-            anchor = func_name.replace("(", "").replace(")", "").replace(",", "").replace(" ", "")
-            f.write(f"- [{func_name}](#{anchor})\n")
+            func_name_no_args = re.sub(r'\([^)]*\)', '', func_name)
+            anchor = func_name_no_args.replace(" ", "")
+            f.write(f"- [{func_name_no_args}](#{anchor})\n")
         f.write("\n")
 
         for func in all_functions:
             func_name = func['func_name']
+            func_name_no_args = re.sub(r'\([^)]*\)', '', func_name)
             docstring = func['docstring']
             line_number = func['line_number']
             file_path = func['file_path']
 
-            f.write(f"## {func_name}\n\n")
+            f.write(f"## {func_name_no_args}\n\n")
             f.write(f"{docstring}\n\n")
 
             f.write(
                 f"```python\n# {file_path} (line {line_number})\ndef {func_name} -> return_type:\n    \"\"\"{docstring}\"\"\"\n    # Function code goes here\n```\n\n")
 
 
 if __name__ == "__main__":
     if len(sys.argv) != 2:
         print("Usage: python script.py <target_directory>")
         sys.exit(1)
 
     target_directory = Path(sys.argv[1])
-    output_file = "../documentation.md"
+    output_file = "documentation.md"
 
     # Remove existing output file if it exists
     if os.path.exists(output_file):
         os.remove(output_file)
 
     generate_md_docs(target_directory, output_file)
```

### Comparing `vigilant_kit-1.2.2/docs/actions.md` & `vigilant_kit-1.2.3/docs/actions.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,69 +1,67 @@
-# Actions
-
 # Table of Contents
 
-- [accept_alert(self)](#accept_alertself)
-- [by_xpath_or_css(self, selector: str)](#by_xpath_or_cssselfselector:str)
-- [clear_field(self, selector)](#clear_fieldselfselector)
-- [click(self, selector)](#clickselfselector)
-- [click_with_delay(self, selector, delay=2)](#click_with_delayselfselectordelay=2)
-- [close(self)](#closeself)
-- [count_elements(self, selector: str)](#count_elementsselfselector:str)
-- [delete_all_cookies(self)](#delete_all_cookiesself)
-- [delete_cookie(self, cookie_to_delete)](#delete_cookieselfcookie_to_delete)
-- [dismiss_alert(self)](#dismiss_alertself)
-- [dont_see(self, selectors: [str | list])](#dont_seeselfselectors:[str|list])
-- [dont_see_in_current_url(self, search_key: str)](#dont_see_in_current_urlselfsearch_key:str)
-- [dont_see_in_title(self, search_key: str)](#dont_see_in_titleselfsearch_key:str)
-- [execute_async_js_script(self, js_script, arguments=None)](#execute_async_js_scriptselfjs_scriptarguments=None)
-- [execute_js_script(self, js_script, arguments=None)](#execute_js_scriptselfjs_scriptarguments=None)
-- [fill_field(self, selector, value)](#fill_fieldselfselectorvalue)
-- [fill_form(self, selector_data)](#fill_formselfselector_data)
-- [find(self, selector: str)](#findselfselector:str)
-- [find_by_class(self, selector: str)](#find_by_classselfselector:str)
-- [find_multiply_by_css(self, selector: str)](#find_multiply_by_cssselfselector:str)
-- [find_multiply_by_xpath(self, selector: str)](#find_multiply_by_xpathselfselector:str)
-- [get_all_cookies(self)](#get_all_cookiesself)
-- [get_base_url()](#get_base_url)
-- [get_cookie(self, cookie)](#get_cookieselfcookie)
-- [get_page_title(self)](#get_page_titleself)
-- [get_text_from_element(self, selector)](#get_text_from_elementselfselector)
-- [get_timeout()](#get_timeout)
-- [maximize_window(self)](#maximize_windowself)
-- [move_mouse_on_element(self, selector)](#move_mouse_on_elementselfselector)
-- [page_back(self)](#page_backself)
-- [page_forward(self)](#page_forwardself)
-- [page_refresh(self)](#page_refreshself)
-- [press_key(self, key)](#press_keyselfkey)
-- [quit(self)](#quitself)
-- [resize_window(self, width, height)](#resize_windowselfwidthheight)
-- [scroll_to(self, selector)](#scroll_toselfselector)
-- [see(self, selectors: [str | list])](#seeselfselectors:[str|list])
-- [see_at_least_one(self, selector)](#see_at_least_oneselfselector)
-- [see_elements_in_quantity_of(self, selector: str, qty: int)](#see_elements_in_quantity_ofselfselector:strqty:int)
-- [see_in_title(self, search_key)](#see_in_titleselfsearch_key)
-- [see_in_url(self, search_key: str)](#see_in_urlselfsearch_key:str)
-- [see_text(self, text)](#see_textselftext)
-- [send_keys(self, selector, keys)](#send_keysselfselectorkeys)
-- [set_cookie(self, cookie_name: dict)](#set_cookieselfcookie_name:dict)
-- [strict_wait(self, seconds: int)](#strict_waitselfseconds:int)
-- [submit_form(self, selector)](#submit_formselfselector)
-- [switch_to_default(self)](#switch_to_defaultself)
-- [switch_to_frame(self, frame_id)](#switch_to_frameselfframe_id)
-- [type_in_alert(self, value)](#type_in_alertselfvalue)
-- [wait_for_alert_(self, selector: str)](#wait_for_alert_selfselector:str)
-- [wait_for_element_to_be_present_in_dom(self, selector: str)](#wait_for_element_to_be_present_in_domselfselector:str)
-- [wait_for_element_to_be_visible(self, selector: str)](#wait_for_element_to_be_visibleselfselector:str)
-- [wait_for_element_to_disappear(self, selector: str)](#wait_for_element_to_disappearselfselector:str)
-- [wait_for_text_to_be_present_in_element(self, selector: str, text: str)](#wait_for_text_to_be_present_in_elementselfselector:strtext:str)
-- [wait_for_text_to_be_present_in_element_attribute(self, selector: str, text_in_attribute: str)](#wait_for_text_to_be_present_in_element_attributeselfselector:strtext_in_attribute:str)
-- [wait_for_text_to_be_present_in_element_value(self, selector: str, value_text: str)](#wait_for_text_to_be_present_in_element_valueselfselector:strvalue_text:str)
+- [accept_alert](#accept_alert)
+- [by_xpath_or_css](#by_xpath_or_css)
+- [clear_field](#clear_field)
+- [click](#click)
+- [click_with_delay](#click_with_delay)
+- [close](#close)
+- [count_elements](#count_elements)
+- [delete_all_cookies](#delete_all_cookies)
+- [delete_cookie](#delete_cookie)
+- [dismiss_alert](#dismiss_alert)
+- [dont_see](#dont_see)
+- [dont_see_in_current_url](#dont_see_in_current_url)
+- [dont_see_in_title](#dont_see_in_title)
+- [execute_async_js_script](#execute_async_js_script)
+- [execute_js_script](#execute_js_script)
+- [fill_field](#fill_field)
+- [fill_form](#fill_form)
+- [find](#find)
+- [find_by_class](#find_by_class)
+- [find_multiply_by_css](#find_multiply_by_css)
+- [find_multiply_by_xpath](#find_multiply_by_xpath)
+- [get_all_cookies](#get_all_cookies)
+- [get_base_url](#get_base_url)
+- [get_cookie](#get_cookie)
+- [get_page_title](#get_page_title)
+- [get_text_from_element](#get_text_from_element)
+- [get_timeout](#get_timeout)
+- [maximize_window](#maximize_window)
+- [move_mouse_on_element](#move_mouse_on_element)
+- [page_back](#page_back)
+- [page_forward](#page_forward)
+- [page_refresh](#page_refresh)
+- [press_key](#press_key)
+- [quit](#quit)
+- [resize_window](#resize_window)
+- [scroll_to](#scroll_to)
+- [see](#see)
+- [see_at_least_one](#see_at_least_one)
+- [see_elements_in_quantity_of](#see_elements_in_quantity_of)
+- [see_in_title](#see_in_title)
+- [see_in_url](#see_in_url)
+- [see_text](#see_text)
+- [send_keys](#send_keys)
+- [set_cookie](#set_cookie)
+- [strict_wait](#strict_wait)
+- [submit_form](#submit_form)
+- [switch_to_default](#switch_to_default)
+- [switch_to_frame](#switch_to_frame)
+- [type_in_alert](#type_in_alert)
+- [wait_for_alert_](#wait_for_alert_)
+- [wait_for_element_to_be_present_in_dom](#wait_for_element_to_be_present_in_dom)
+- [wait_for_element_to_be_visible](#wait_for_element_to_be_visible)
+- [wait_for_element_to_disappear](#wait_for_element_to_disappear)
+- [wait_for_text_to_be_present_in_element](#wait_for_text_to_be_present_in_element)
+- [wait_for_text_to_be_present_in_element_attribute](#wait_for_text_to_be_present_in_element_attribute)
+- [wait_for_text_to_be_present_in_element_value](#wait_for_text_to_be_present_in_element_value)
 
-## accept_alert(self)
+## accept_alert
 
 
         Accepts the alert.
 
         :return: self
         
 
@@ -74,15 +72,15 @@
         Accepts the alert.
 
         :return: self
         """
     # Function code goes here
 ```
 
-## by_xpath_or_css(self, selector: str)
+## by_xpath_or_css
 
 
         Return tuple with search pattern (XPATH or CSS) and searched selector.
 
         :param selector: XPATH or CSS selector string
         :return: tuple with search pattern (XPATH or CSS) and searched selector
         
@@ -95,15 +93,15 @@
 
         :param selector: XPATH or CSS selector string
         :return: tuple with search pattern (XPATH or CSS) and searched selector
         """
     # Function code goes here
 ```
 
-## clear_field(self, selector)
+## clear_field
 
 
         Clears a field after it becomes visible.
 
         :param selector: The field to clear
         :return: self
         
@@ -116,15 +114,15 @@
 
         :param selector: The field to clear
         :return: self
         """
     # Function code goes here
 ```
 
-## click(self, selector)
+## click
 
 
         Clicks on an element after it becomes visible.
 
         :param selector: The element to click on
         :return: self
         
@@ -137,15 +135,15 @@
 
         :param selector: The element to click on
         :return: self
         """
     # Function code goes here
 ```
 
-## click_with_delay(self, selector, delay=2)
+## click_with_delay
 
 
         Clicks on an element only after it becomes visible and adds an additional delay before click.
 
         :param selector: The element to click on
         :param delay: The additional delay in seconds (default is 2)
         :return: self
@@ -160,15 +158,15 @@
         :param selector: The element to click on
         :param delay: The additional delay in seconds (default is 2)
         :return: self
         """
     # Function code goes here
 ```
 
-## close(self)
+## close
 
 
         Closes the current window.
 
         :return: self
         
 
@@ -179,15 +177,15 @@
         Closes the current window.
 
         :return: self
         """
     # Function code goes here
 ```
 
-## count_elements(self, selector: str)
+## count_elements
 
 
         Count all elements that match the provided selector, visible or not.
 
         :param selector: CSS selector
         :return: number of elements that match the selector
         
@@ -200,15 +198,15 @@
 
         :param selector: CSS selector
         :return: number of elements that match the selector
         """
     # Function code goes here
 ```
 
-## delete_all_cookies(self)
+## delete_all_cookies
 
 
         Deletes all cookies in the scope of the session.
 
         :return: self
         
 
@@ -219,15 +217,15 @@
         Deletes all cookies in the scope of the session.
 
         :return: self
         """
     # Function code goes here
 ```
 
-## delete_cookie(self, cookie_to_delete)
+## delete_cookie
 
 
         Deletes a specific cookie.
 
         :param cookie_to_delete: The name of the cookie to delete
         :return: self
         
@@ -240,15 +238,15 @@
 
         :param cookie_to_delete: The name of the cookie to delete
         :return: self
         """
     # Function code goes here
 ```
 
-## dismiss_alert(self)
+## dismiss_alert
 
 
         Dismisses the alert.
 
         :return: self
         
 
@@ -259,15 +257,15 @@
         Dismisses the alert.
 
         :return: self
         """
     # Function code goes here
 ```
 
-## dont_see(self, selectors: [str | list])
+## dont_see
 
 
         Assert that none of the elements matching the provided selectors are visible.
 
         :param selectors: list of CSS selectors
         
 
@@ -278,15 +276,15 @@
         Assert that none of the elements matching the provided selectors are visible.
 
         :param selectors: list of CSS selectors
         """
     # Function code goes here
 ```
 
-## dont_see_in_current_url(self, search_key: str)
+## dont_see_in_current_url
 
 
         Assert that the provided search key is not present in the current page URL.
 
         :param search_key: string to search for
         
 
@@ -297,15 +295,15 @@
         Assert that the provided search key is not present in the current page URL.
 
         :param search_key: string to search for
         """
     # Function code goes here
 ```
 
-## dont_see_in_title(self, search_key: str)
+## dont_see_in_title
 
 
         Assert that the provided search key is not present in the current page title.
 
         :param search_key: string to search for
         
 
@@ -316,15 +314,15 @@
         Assert that the provided search key is not present in the current page title.
 
         :param search_key: string to search for
         """
     # Function code goes here
 ```
 
-## execute_async_js_script(self, js_script, arguments=None)
+## execute_async_js_script
 
 
         Executes an asynchronous JavaScript script with optional arguments.
 
         :param js_script: The JavaScript script to execute
         :param arguments: Optional arguments for the script
         :return: self
@@ -339,15 +337,15 @@
         :param js_script: The JavaScript script to execute
         :param arguments: Optional arguments for the script
         :return: self
         """
     # Function code goes here
 ```
 
-## execute_js_script(self, js_script, arguments=None)
+## execute_js_script
 
 
         Executes a JavaScript script with optional arguments.
 
         :param js_script: The JavaScript script to execute
         :param arguments: Optional arguments for the script
         :return: self
@@ -362,15 +360,15 @@
         :param js_script: The JavaScript script to execute
         :param arguments: Optional arguments for the script
         :return: self
         """
     # Function code goes here
 ```
 
-## fill_field(self, selector, value)
+## fill_field
 
 
         Fills a field with a specified value after the field becomes visible.
 
         :param selector: The field to fill
         :param value: The value to fill in the field
         :return: self
@@ -385,15 +383,15 @@
         :param selector: The field to fill
         :param value: The value to fill in the field
         :return: self
         """
     # Function code goes here
 ```
 
-## fill_form(self, selector_data)
+## fill_form
 
 
         Fills multiple fields in a form using a dictionary of selectors and values.
 
         :param selector_data: A dictionary of selectors and values
         :return: self
         
@@ -406,15 +404,15 @@
 
         :param selector_data: A dictionary of selectors and values
         :return: self
         """
     # Function code goes here
 ```
 
-## find(self, selector: str)
+## find
 
 
         return self.driver.find_element(*self.by_xpath_or_css(selector))
 
     def find_multiply(self, selector: str) -> List[WebElement]:
         
 
@@ -425,15 +423,15 @@
         return self.driver.find_element(*self.by_xpath_or_css(selector))
 
     def find_multiply(self, selector: str) -> List[WebElement]:
         """
     # Function code goes here
 ```
 
-## find_by_class(self, selector: str)
+## find_by_class
 
 
         Find element by class name.
 
         :param selector: class name string
         :return: the element found using the class name selector
         
@@ -446,15 +444,15 @@
 
         :param selector: class name string
         :return: the element found using the class name selector
         """
     # Function code goes here
 ```
 
-## find_multiply_by_css(self, selector: str)
+## find_multiply_by_css
 
 
         Find multiple elements by CSS selector.
 
         :param selector: CSS selector string
         :return: list of elements found using the CSS selector
         
@@ -467,15 +465,15 @@
 
         :param selector: CSS selector string
         :return: list of elements found using the CSS selector
         """
     # Function code goes here
 ```
 
-## find_multiply_by_xpath(self, selector: str)
+## find_multiply_by_xpath
 
 
         Find multiple elements by XPATH selector.
 
         :param selector: XPATH selector string
         :return: list of elements found using the XPATH selector
         
@@ -488,15 +486,15 @@
 
         :param selector: XPATH selector string
         :return: list of elements found using the XPATH selector
         """
     # Function code goes here
 ```
 
-## get_all_cookies(self)
+## get_all_cookies
 
 
         Returns a set of dictionaries corresponding to cookies visible in the current session.
 
         :return: self
         
 
@@ -507,15 +505,15 @@
         Returns a set of dictionaries corresponding to cookies visible in the current session.
 
         :return: self
         """
     # Function code goes here
 ```
 
-## get_base_url()
+## get_base_url
 
 
     Get the base URL from the environment variable 'BASE_URL'.
 
     :return: base URL as a string
     
 
@@ -526,15 +524,15 @@
     Get the base URL from the environment variable 'BASE_URL'.
 
     :return: base URL as a string
     """
     # Function code goes here
 ```
 
-## get_cookie(self, cookie)
+## get_cookie
 
 
         Gets a single cookie.
 
         :param cookie: The name of the cookie to retrieve
         :return: self
         
@@ -547,15 +545,15 @@
 
         :param cookie: The name of the cookie to retrieve
         :return: self
         """
     # Function code goes here
 ```
 
-## get_page_title(self)
+## get_page_title
 
 
         Returns the title of the current page.
 
         :return: page title as a string
         
 
@@ -566,15 +564,15 @@
         Returns the title of the current page.
 
         :return: page title as a string
         """
     # Function code goes here
 ```
 
-## get_text_from_element(self, selector)
+## get_text_from_element
 
 
         Gets the text from an element after it becomes visible.
 
         :param selector: The element to get text from
         :return: The text of the element
         
@@ -587,15 +585,15 @@
 
         :param selector: The element to get text from
         :return: The text of the element
         """
     # Function code goes here
 ```
 
-## get_timeout()
+## get_timeout
 
 
         Waits for the element with the specified selector to be clickable.
 
         :param selector: The element's selector
         :return: self
         
@@ -608,15 +606,15 @@
 
         :param selector: The element's selector
         :return: self
         """
     # Function code goes here
 ```
 
-## maximize_window(self)
+## maximize_window
 
 
         Maximizes the current window that the WebDriver is using.
 
         :return: self
         
 
@@ -627,15 +625,15 @@
         Maximizes the current window that the WebDriver is using.
 
         :return: self
         """
     # Function code goes here
 ```
 
-## move_mouse_on_element(self, selector)
+## move_mouse_on_element
 
 
         Moves the mouse cursor over an element after the element becomes visible.
 
         :param selector: The element to move the mouse cursor over
         :return: self
         
@@ -648,15 +646,15 @@
 
         :param selector: The element to move the mouse cursor over
         :return: self
         """
     # Function code goes here
 ```
 
-## page_back(self)
+## page_back
 
 
         Goes one step backward in the browser history.
 
         :return: self
         
 
@@ -667,15 +665,15 @@
         Goes one step backward in the browser history.
 
         :return: self
         """
     # Function code goes here
 ```
 
-## page_forward(self)
+## page_forward
 
 
         Goes one step forward in the browser history.
 
         :return: self
         
 
@@ -686,15 +684,15 @@
         Goes one step forward in the browser history.
 
         :return: self
         """
     # Function code goes here
 ```
 
-## page_refresh(self)
+## page_refresh
 
 
         Refreshes the current page.
 
         :return: self
         
 
@@ -705,15 +703,15 @@
         Refreshes the current page.
 
         :return: self
         """
     # Function code goes here
 ```
 
-## press_key(self, key)
+## press_key
 
 
         Presses a specified key.
 
         :param key: The key to press
         :return: self
         
@@ -726,15 +724,15 @@
 
         :param key: The key to press
         :return: self
         """
     # Function code goes here
 ```
 
-## quit(self)
+## quit
 
 
         Quits the driver and closes every associated window.
 
         :return: self
         
 
@@ -745,15 +743,15 @@
         Quits the driver and closes every associated window.
 
         :return: self
         """
     # Function code goes here
 ```
 
-## resize_window(self, width, height)
+## resize_window
 
 
         Sets the current window width and height.
 
         :param width: The desired window width in pixels
         :param height: The desired window height in pixels
         :return: self
@@ -768,15 +766,15 @@
         :param width: The desired window width in pixels
         :param height: The desired window height in pixels
         :return: self
         """
     # Function code goes here
 ```
 
-## scroll_to(self, selector)
+## scroll_to
 
 
         Scrolls to an element.
 
         :param selector: The element to scroll to
         :return: self
         
@@ -789,15 +787,15 @@
 
         :param selector: The element to scroll to
         :return: self
         """
     # Function code goes here
 ```
 
-## see(self, selectors: [str | list])
+## see
 
 
         Assert that at least one of the elements matching the provided selectors is visible.
 
         :param selectors: list of CSS selectors
         
 
@@ -808,15 +806,15 @@
         Assert that at least one of the elements matching the provided selectors is visible.
 
         :param selectors: list of CSS selectors
         """
     # Function code goes here
 ```
 
-## see_at_least_one(self, selector)
+## see_at_least_one
 
 
         Assert that at least one element matching the provided selector is visible.
 
         :param selector: CSS selector
         
 
@@ -827,15 +825,15 @@
         Assert that at least one element matching the provided selector is visible.
 
         :param selector: CSS selector
         """
     # Function code goes here
 ```
 
-## see_elements_in_quantity_of(self, selector: str, qty: int)
+## see_elements_in_quantity_of
 
 
         Assert that the number of visible elements that match the provided selector is equal to the provided quantity.
 
         :param selector: CSS selector
         :param qty: expected number of elements
         
@@ -848,15 +846,15 @@
 
         :param selector: CSS selector
         :param qty: expected number of elements
         """
     # Function code goes here
 ```
 
-## see_in_title(self, search_key)
+## see_in_title
 
 
         Assert that the provided search key is present in the current page title.
 
         :param search_key: string to search for
         
 
@@ -867,15 +865,15 @@
         Assert that the provided search key is present in the current page title.
 
         :param search_key: string to search for
         """
     # Function code goes here
 ```
 
-## see_in_url(self, search_key: str)
+## see_in_url
 
 
         Assert that the provided search key is present in the current page URL.
 
         :param search_key: string to search for
         
 
@@ -886,15 +884,15 @@
         Assert that the provided search key is present in the current page URL.
 
         :param search_key: string to search for
         """
     # Function code goes here
 ```
 
-## see_text(self, text)
+## see_text
 
 
         Assert that the provided text is present on the current page.
 
         :param text: text to search for
         
 
@@ -905,15 +903,15 @@
         Assert that the provided text is present on the current page.
 
         :param text: text to search for
         """
     # Function code goes here
 ```
 
-## send_keys(self, selector, keys)
+## send_keys
 
 
         Sends keys to a specified field.
 
         :param selector: The field to send keys to
         :param keys: The keys to send
         :return: self
@@ -928,15 +926,15 @@
         :param selector: The field to send keys to
         :param keys: The keys to send
         :return: self
         """
     # Function code goes here
 ```
 
-## set_cookie(self, cookie_name: dict)
+## set_cookie
 
 
         Sets a new cookie.
 
         :param cookie_name: A dictionary containing the cookie name and value
         
 
@@ -947,15 +945,15 @@
         Sets a new cookie.
 
         :param cookie_name: A dictionary containing the cookie name and value
         """
     # Function code goes here
 ```
 
-## strict_wait(self, seconds: int)
+## strict_wait
 
 
         Waits for the specified number of seconds.
 
         :param seconds: The number of seconds to wait
         :return: self
         
@@ -968,15 +966,15 @@
 
         :param seconds: The number of seconds to wait
         :return: self
         """
     # Function code goes here
 ```
 
-## submit_form(self, selector)
+## submit_form
 
 
         Submits a form using a specified selector.
 
         :param selector: The form to submit
         :return: self
         
@@ -989,15 +987,15 @@
 
         :param selector: The form to submit
         :return: self
         """
     # Function code goes here
 ```
 
-## switch_to_default(self)
+## switch_to_default
 
 
         Switches the WebDriver focus to the default frame.
 
         :return: self
         
 
@@ -1008,15 +1006,15 @@
         Switches the WebDriver focus to the default frame.
 
         :return: self
         """
     # Function code goes here
 ```
 
-## switch_to_frame(self, frame_id)
+## switch_to_frame
 
 
         Switches the WebDriver focus to the specified frame.
 
         :param frame_id: The ID of the frame to switch to
         :return: self
         
@@ -1029,15 +1027,15 @@
 
         :param frame_id: The ID of the frame to switch to
         :return: self
         """
     # Function code goes here
 ```
 
-## type_in_alert(self, value)
+## type_in_alert
 
 
         Types the specified value in the alert.
 
         :param value: The value to type in the alert
         :return: self
         
@@ -1050,15 +1048,15 @@
 
         :param value: The value to type in the alert
         :return: self
         """
     # Function code goes here
 ```
 
-## wait_for_alert_(self, selector: str)
+## wait_for_alert_
 
 
         Waits for an alert to be present.
 
         :param selector: The element's selector
         :return: self
         
@@ -1071,15 +1069,15 @@
 
         :param selector: The element's selector
         :return: self
         """
     # Function code goes here
 ```
 
-## wait_for_element_to_be_present_in_dom(self, selector: str)
+## wait_for_element_to_be_present_in_dom
 
 
         Waits for the element with the specified selector to be present in the DOM.
 
         :param selector: The element's selector
         :return: self
         
@@ -1092,15 +1090,15 @@
 
         :param selector: The element's selector
         :return: self
         """
     # Function code goes here
 ```
 
-## wait_for_element_to_be_visible(self, selector: str)
+## wait_for_element_to_be_visible
 
 
         Waits for the element with the specified selector to be visible.
 
         :param selector: The element's selector
         :return: self
         
@@ -1113,15 +1111,15 @@
 
         :param selector: The element's selector
         :return: self
         """
     # Function code goes here
 ```
 
-## wait_for_element_to_disappear(self, selector: str)
+## wait_for_element_to_disappear
 
 
         Waits for the element with the specified selector to disappear.
 
         :param selector: The element's selector
         :return: self
         
@@ -1134,15 +1132,15 @@
 
         :param selector: The element's selector
         :return: self
         """
     # Function code goes here
 ```
 
-## wait_for_text_to_be_present_in_element(self, selector: str, text: str)
+## wait_for_text_to_be_present_in_element
 
 
         Waits for the specified text to be present in the element with the given selector.
 
         :param selector: The element's selector
         :param text: The text to wait for
         :return: self
@@ -1157,15 +1155,15 @@
         :param selector: The element's selector
         :param text: The text to wait for
         :return: self
         """
     # Function code goes here
 ```
 
-## wait_for_text_to_be_present_in_element_attribute(self, selector: str, text_in_attribute: str)
+## wait_for_text_to_be_present_in_element_attribute
 
 
         Waits for the specified text to be present in the attribute of the element with the given selector.
 
         :param selector: The element's selector
         :param text_in_attribute: The text to wait for
         :return: self
@@ -1180,15 +1178,15 @@
         :param selector: The element's selector
         :param text_in_attribute: The text to wait for
         :return: self
         """
     # Function code goes here
 ```
 
-## wait_for_text_to_be_present_in_element_value(self, selector: str, value_text: str)
+## wait_for_text_to_be_present_in_element_value
 
 
         Waits for the specified text to be present in the value of the element with the given selector.
 
         :param selector: The element's selector
         :param value_text: The text to wait for
         :return: self
```

### Comparing `vigilant_kit-1.2.2/docs/browser_options.md` & `vigilant_kit-1.2.3/docs/browser_options.md`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.2/docs/native_selenium.md` & `vigilant_kit-1.2.3/docs/native_selenium.md`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.2/docs/selenium_install.md` & `vigilant_kit-1.2.3/docs/selenium_install.md`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.2/docs/tutorial_pytest.md` & `vigilant_kit-1.2.3/docs/tutorial_pytest.md`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.2/docs/vigilant_pytest.md` & `vigilant_kit-1.2.3/docs/vigilant_pytest.md`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.2/docs/vigilant_unittest.md` & `vigilant_kit-1.2.3/docs/vigilant_unittest.md`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.2/src/vgl_cli/install_dev_kit_command.py` & `vigilant_kit-1.2.3/src/vgl_cli/install_dev_kit_command.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.2/src/vgl_cli/install_standalone_command.py` & `vigilant_kit-1.2.3/src/vgl_cli/install_standalone_command.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.2/src/vgl_cli/install_webdriver_command.py` & `vigilant_kit-1.2.3/src/vgl_cli/install_webdriver_command.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.2/src/vgl_cli/run_selenium_command.py` & `vigilant_kit-1.2.3/src/vgl_cli/run_selenium_command.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.2/src/vgl_cli/vgl.py` & `vigilant_kit-1.2.3/src/vgl_cli/vgl.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.2/src/vigilant/actions/assertions.py` & `vigilant_kit-1.2.3/src/vigilant/actions/assertions.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.2/src/vigilant/actions/finder.py` & `vigilant_kit-1.2.3/src/vigilant/actions/finder.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.2/src/vigilant/actions/vigilant_actions.py` & `vigilant_kit-1.2.3/src/vigilant/actions/vigilant_actions.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.2/src/vigilant/actions/waiter.py` & `vigilant_kit-1.2.3/src/vigilant/actions/waiter.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.2/src/vigilant/driver/vigilant_driver.py` & `vigilant_kit-1.2.3/src/vigilant/driver/vigilant_driver.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.2/.gitignore` & `vigilant_kit-1.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.2/LICENSE` & `vigilant_kit-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.2/README.md` & `vigilant_kit-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.2/pyproject.toml` & `vigilant_kit-1.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "vigilant_kit"
-version = "1.2.2"
+version = "1.2.3"
 authors = [
   { name="Pelykh Ivan", email="ivan.pelykh@protonmail.com" },
 ]
 description = "Library that makes functional testing with Selenium WebDriver fast and easy. "
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `vigilant_kit-1.2.2/PKG-INFO` & `vigilant_kit-1.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vigilant_kit
-Version: 1.2.2
+Version: 1.2.3
 Summary: Library that makes functional testing with Selenium WebDriver fast and easy. 
 Project-URL: Homepage, https://github.com/ivpel/vigilant
 Project-URL: Bug Tracker, https://github.com/ivpel/vigilant/issues
 Author-email: Pelykh Ivan <ivan.pelykh@protonmail.com>
 License-File: LICENSE
 Keywords: bdd,functional,functional-testing,pytest,selenium,tdd,testing,unittest,webdriver
 Requires-Python: >=3.7
```

