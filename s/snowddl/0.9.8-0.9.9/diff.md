# Comparing `tmp/snowddl-0.9.8.tar.gz` & `tmp/snowddl-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snowddl-0.9.8.tar", last modified: Tue Oct 11 15:26:53 2022, max compression
+gzip compressed data, was "snowddl-0.9.9.tar", last modified: Thu Oct 13 09:47:37 2022, max compression
```

## Comparing `snowddl-0.9.8.tar` & `snowddl-0.9.9.tar`

### file list

```diff
@@ -1,298 +1,298 @@
-drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-11 15:26:53.900257 snowddl-0.9.8/
--rw-r--r--   0 vmarkov    (501) staff       (20)    11309 2022-01-27 15:42:20.000000 snowddl-0.9.8/LICENSE.txt
--rw-r--r--   0 vmarkov    (501) staff       (20)       61 2022-01-27 16:29:40.000000 snowddl-0.9.8/MANIFEST.in
--rw-r--r--   0 vmarkov    (501) staff       (20)     1786 2022-10-11 15:26:53.900057 snowddl-0.9.8/PKG-INFO
--rw-r--r--   0 vmarkov    (501) staff       (20)     3601 2022-10-04 08:35:09.000000 snowddl-0.9.8/README.md
--rw-r--r--   0 vmarkov    (501) staff       (20)       38 2022-10-11 15:26:53.900308 snowddl-0.9.8/setup.cfg
--rw-r--r--   0 vmarkov    (501) staff       (20)     2499 2022-10-04 10:38:37.000000 snowddl-0.9.8/setup.py
-drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-11 15:26:53.843051 snowddl-0.9.8/snowddl/
--rw-r--r--   0 vmarkov    (501) staff       (20)      380 2022-08-19 13:39:10.000000 snowddl-0.9.8/snowddl/__init__.py
-drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-11 15:26:53.838201 snowddl-0.9.8/snowddl/_config/
-drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-11 15:26:53.844734 snowddl-0.9.8/snowddl/_config/sample01_01/
--rw-r--r--   0 vmarkov    (501) staff       (20)     1050 2022-05-12 16:00:34.000000 snowddl-0.9.8/snowddl/_config/sample01_01/business_role.yaml
-drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-11 15:26:53.837425 snowddl-0.9.8/snowddl/_config/sample01_01/snowddl_db/
-drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-11 15:26:53.844969 snowddl-0.9.8/snowddl/_config/sample01_01/snowddl_db/bookings/
-drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-11 15:26:53.845361 snowddl-0.9.8/snowddl/_config/sample01_01/snowddl_db/bookings/function/
--rw-r--r--   0 vmarkov    (501) staff       (20)      305 2022-01-31 13:45:39.000000 snowddl-0.9.8/snowddl/_config/sample01_01/snowddl_db/bookings/function/lang(object).yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)      103 2022-01-31 12:37:22.000000 snowddl-0.9.8/snowddl/_config/sample01_01/snowddl_db/bookings/function/now().yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)       41 2022-01-31 11:51:07.000000 snowddl-0.9.8/snowddl/_config/sample01_01/snowddl_db/bookings/params.yaml
-drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-11 15:26:53.845512 snowddl-0.9.8/snowddl/_config/sample01_01/snowddl_db/bookings/procedure/
--rw-r--r--   0 vmarkov    (501) staff       (20)      311 2022-02-01 17:44:32.000000 snowddl-0.9.8/snowddl/_config/sample01_01/snowddl_db/bookings/procedure/check_in(varchar,number,number,varchar).yaml
-drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-11 15:26:53.845661 snowddl-0.9.8/snowddl/_config/sample01_01/snowddl_db/bookings/sequence/
--rw-r--r--   0 vmarkov    (501) staff       (20)       21 2022-01-31 12:00:29.000000 snowddl-0.9.8/snowddl/_config/sample01_01/snowddl_db/bookings/sequence/flights_id_seq.yaml
-drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-11 15:26:53.846825 snowddl-0.9.8/snowddl/_config/sample01_01/snowddl_db/bookings/table/
--rw-r--r--   0 vmarkov    (501) staff       (20)      496 2022-01-31 13:10:50.000000 snowddl-0.9.8/snowddl/_config/sample01_01/snowddl_db/bookings/table/aircrafts_data.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)      637 2022-01-31 13:10:50.000000 snowddl-0.9.8/snowddl/_config/sample01_01/snowddl_db/bookings/table/airports_data.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)     1013 2022-01-31 11:06:29.000000 snowddl-0.9.8/snowddl/_config/sample01_01/snowddl_db/bookings/table/boarding_passes.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)      649 2022-01-31 12:23:15.000000 snowddl-0.9.8/snowddl/_config/sample01_01/snowddl_db/bookings/table/bookings.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)     2087 2022-01-31 13:46:08.000000 snowddl-0.9.8/snowddl/_config/sample01_01/snowddl_db/bookings/table/flights.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)      590 2022-01-31 11:26:43.000000 snowddl-0.9.8/snowddl/_config/sample01_01/snowddl_db/bookings/table/seats.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)      681 2022-01-31 11:30:32.000000 snowddl-0.9.8/snowddl/_config/sample01_01/snowddl_db/bookings/table/ticket_flights.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)      960 2022-01-31 11:34:08.000000 snowddl-0.9.8/snowddl/_config/sample01_01/snowddl_db/bookings/table/tickets.yaml
-drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-11 15:26:53.847404 snowddl-0.9.8/snowddl/_config/sample01_01/snowddl_db/bookings/view/
--rw-r--r--   0 vmarkov    (501) staff       (20)      431 2022-01-31 13:34:28.000000 snowddl-0.9.8/snowddl/_config/sample01_01/snowddl_db/bookings/view/aircrafts.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)      663 2022-01-31 13:34:55.000000 snowddl-0.9.8/snowddl/_config/sample01_01/snowddl_db/bookings/view/airports.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)     1103 2022-01-31 13:37:38.000000 snowddl-0.9.8/snowddl/_config/sample01_01/snowddl_db/bookings/view/flights_v.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)     1377 2022-01-31 13:37:38.000000 snowddl-0.9.8/snowddl/_config/sample01_01/snowddl_db/bookings/view/routes.yaml
-drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-11 15:26:53.837364 snowddl-0.9.8/snowddl/_config/sample01_01/snowddl_db/sakila/
-drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-11 15:26:53.849643 snowddl-0.9.8/snowddl/_config/sample01_01/snowddl_db/sakila/table/
--rw-r--r--   0 vmarkov    (501) staff       (20)      169 2022-01-29 19:17:21.000000 snowddl-0.9.8/snowddl/_config/sample01_01/snowddl_db/sakila/table/actor.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)      377 2022-01-31 13:44:58.000000 snowddl-0.9.8/snowddl/_config/sample01_01/snowddl_db/sakila/table/address.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)      143 2022-01-29 20:43:43.000000 snowddl-0.9.8/snowddl/_config/sample01_01/snowddl_db/sakila/table/category.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)      265 2022-01-31 13:44:58.000000 snowddl-0.9.8/snowddl/_config/sample01_01/snowddl_db/sakila/table/city.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)      135 2022-01-29 20:30:41.000000 snowddl-0.9.8/snowddl/_config/sample01_01/snowddl_db/sakila/table/country.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)      543 2022-01-31 13:44:58.000000 snowddl-0.9.8/snowddl/_config/sample01_01/snowddl_db/sakila/table/customer.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)      769 2022-01-31 13:44:58.000000 snowddl-0.9.8/snowddl/_config/sample01_01/snowddl_db/sakila/table/film.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)      311 2022-01-31 13:44:58.000000 snowddl-0.9.8/snowddl/_config/sample01_01/snowddl_db/sakila/table/film_actor.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)      324 2022-01-31 13:44:58.000000 snowddl-0.9.8/snowddl/_config/sample01_01/snowddl_db/sakila/table/film_category.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)      343 2022-01-31 13:44:58.000000 snowddl-0.9.8/snowddl/_config/sample01_01/snowddl_db/sakila/table/inventory.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)      143 2022-01-29 20:43:43.000000 snowddl-0.9.8/snowddl/_config/sample01_01/snowddl_db/sakila/table/language.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)      530 2022-01-31 13:44:58.000000 snowddl-0.9.8/snowddl/_config/sample01_01/snowddl_db/sakila/table/payment.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)      549 2022-01-31 13:44:58.000000 snowddl-0.9.8/snowddl/_config/sample01_01/snowddl_db/sakila/table/rental.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)      579 2022-01-31 13:44:58.000000 snowddl-0.9.8/snowddl/_config/sample01_01/snowddl_db/sakila/table/staff.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)      362 2022-01-31 13:44:58.000000 snowddl-0.9.8/snowddl/_config/sample01_01/snowddl_db/sakila/table/store.yaml
-drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-11 15:26:53.850574 snowddl-0.9.8/snowddl/_config/sample01_01/snowddl_db/sakila/view/
--rw-r--r--   0 vmarkov    (501) staff       (20)      127 2022-02-02 20:30:32.000000 snowddl-0.9.8/snowddl/_config/sample01_01/snowddl_db/sakila/view/actor_list.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)      526 2022-01-29 19:43:23.000000 snowddl-0.9.8/snowddl/_config/sample01_01/snowddl_db/sakila/view/customer_list.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)      580 2022-01-29 19:44:18.000000 snowddl-0.9.8/snowddl/_config/sample01_01/snowddl_db/sakila/view/film_list.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)      384 2022-01-29 19:48:01.000000 snowddl-0.9.8/snowddl/_config/sample01_01/snowddl_db/sakila/view/sales_by_film_category.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)      577 2022-01-29 19:47:01.000000 snowddl-0.9.8/snowddl/_config/sample01_01/snowddl_db/sakila/view/sales_by_store.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)      447 2022-01-29 19:45:27.000000 snowddl-0.9.8/snowddl/_config/sample01_01/snowddl_db/sakila/view/staff_list.yaml
-drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-11 15:26:53.850710 snowddl-0.9.8/snowddl/_config/sample01_01/snowddl_db/sakila_sandbox/
--rw-r--r--   0 vmarkov    (501) staff       (20)       97 2022-02-01 16:56:18.000000 snowddl-0.9.8/snowddl/_config/sample01_01/snowddl_db/sakila_sandbox/params.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)      605 2022-05-24 14:49:33.000000 snowddl-0.9.8/snowddl/_config/sample01_01/tech_role.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)     2144 2022-05-24 14:53:10.000000 snowddl-0.9.8/snowddl/_config/sample01_01/user.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)      406 2022-02-01 13:51:42.000000 snowddl-0.9.8/snowddl/_config/sample01_01/warehouse.yaml
-drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-11 15:26:53.851671 snowddl-0.9.8/snowddl/_config/sample01_02/
--rw-r--r--   0 vmarkov    (501) staff       (20)     1019 2022-05-30 17:15:57.000000 snowddl-0.9.8/snowddl/_config/sample01_02/business_role.yaml
-drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-11 15:26:53.838140 snowddl-0.9.8/snowddl/_config/sample01_02/snowddl_db/
-drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-11 15:26:53.851883 snowddl-0.9.8/snowddl/_config/sample01_02/snowddl_db/bookings/
-drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-11 15:26:53.852402 snowddl-0.9.8/snowddl/_config/sample01_02/snowddl_db/bookings/function/
--rw-r--r--   0 vmarkov    (501) staff       (20)      305 2022-01-31 13:45:39.000000 snowddl-0.9.8/snowddl/_config/sample01_02/snowddl_db/bookings/function/lang(object).yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)      103 2022-02-02 20:21:25.000000 snowddl-0.9.8/snowddl/_config/sample01_02/snowddl_db/bookings/function/now().yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)       41 2022-01-31 11:51:07.000000 snowddl-0.9.8/snowddl/_config/sample01_02/snowddl_db/bookings/params.yaml
-drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-11 15:26:53.852625 snowddl-0.9.8/snowddl/_config/sample01_02/snowddl_db/bookings/procedure/
--rw-r--r--   0 vmarkov    (501) staff       (20)      293 2022-02-02 20:19:54.000000 snowddl-0.9.8/snowddl/_config/sample01_02/snowddl_db/bookings/procedure/check_in(varchar,number,number).yaml
-drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-11 15:26:53.852859 snowddl-0.9.8/snowddl/_config/sample01_02/snowddl_db/bookings/sequence/
--rw-r--r--   0 vmarkov    (501) staff       (20)       59 2022-02-02 20:21:25.000000 snowddl-0.9.8/snowddl/_config/sample01_02/snowddl_db/bookings/sequence/flights_id_seq.yaml
-drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-11 15:26:53.854427 snowddl-0.9.8/snowddl/_config/sample01_02/snowddl_db/bookings/table/
--rw-r--r--   0 vmarkov    (501) staff       (20)      496 2022-02-02 20:21:25.000000 snowddl-0.9.8/snowddl/_config/sample01_02/snowddl_db/bookings/table/aircrafts_data.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)      724 2022-02-02 20:23:58.000000 snowddl-0.9.8/snowddl/_config/sample01_02/snowddl_db/bookings/table/airports_data.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)      988 2022-02-02 20:22:27.000000 snowddl-0.9.8/snowddl/_config/sample01_02/snowddl_db/bookings/table/boarding_passes.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)      649 2022-01-31 12:23:15.000000 snowddl-0.9.8/snowddl/_config/sample01_02/snowddl_db/bookings/table/bookings.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)     2087 2022-02-02 20:21:25.000000 snowddl-0.9.8/snowddl/_config/sample01_02/snowddl_db/bookings/table/flights.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)      592 2022-02-02 20:22:27.000000 snowddl-0.9.8/snowddl/_config/sample01_02/snowddl_db/bookings/table/seats.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)      681 2022-02-02 20:21:25.000000 snowddl-0.9.8/snowddl/_config/sample01_02/snowddl_db/bookings/table/ticket_flights.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)      960 2022-01-31 11:34:08.000000 snowddl-0.9.8/snowddl/_config/sample01_02/snowddl_db/bookings/table/tickets.yaml
-drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-11 15:26:53.855384 snowddl-0.9.8/snowddl/_config/sample01_02/snowddl_db/bookings/view/
--rw-r--r--   0 vmarkov    (501) staff       (20)      431 2022-02-14 21:45:55.000000 snowddl-0.9.8/snowddl/_config/sample01_02/snowddl_db/bookings/view/aircrafts.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)      741 2022-02-02 20:42:35.000000 snowddl-0.9.8/snowddl/_config/sample01_02/snowddl_db/bookings/view/airports.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)     1103 2022-01-31 13:37:38.000000 snowddl-0.9.8/snowddl/_config/sample01_02/snowddl_db/bookings/view/flights_v.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)     1377 2022-01-31 13:37:38.000000 snowddl-0.9.8/snowddl/_config/sample01_02/snowddl_db/bookings/view/routes.yaml
-drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-11 15:26:53.838069 snowddl-0.9.8/snowddl/_config/sample01_02/snowddl_db/sakila/
-drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-11 15:26:53.858706 snowddl-0.9.8/snowddl/_config/sample01_02/snowddl_db/sakila/table/
--rw-r--r--   0 vmarkov    (501) staff       (20)      191 2022-02-02 20:29:39.000000 snowddl-0.9.8/snowddl/_config/sample01_02/snowddl_db/sakila/table/actor.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)      377 2022-01-31 13:44:58.000000 snowddl-0.9.8/snowddl/_config/sample01_02/snowddl_db/sakila/table/address.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)      143 2022-01-29 20:43:43.000000 snowddl-0.9.8/snowddl/_config/sample01_02/snowddl_db/sakila/table/category.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)      265 2022-01-31 13:44:58.000000 snowddl-0.9.8/snowddl/_config/sample01_02/snowddl_db/sakila/table/city.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)      135 2022-01-29 20:30:41.000000 snowddl-0.9.8/snowddl/_config/sample01_02/snowddl_db/sakila/table/country.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)      543 2022-01-31 13:44:58.000000 snowddl-0.9.8/snowddl/_config/sample01_02/snowddl_db/sakila/table/customer.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)      769 2022-01-31 13:44:58.000000 snowddl-0.9.8/snowddl/_config/sample01_02/snowddl_db/sakila/table/film.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)      311 2022-01-31 13:44:58.000000 snowddl-0.9.8/snowddl/_config/sample01_02/snowddl_db/sakila/table/film_actor.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)      324 2022-01-31 13:44:58.000000 snowddl-0.9.8/snowddl/_config/sample01_02/snowddl_db/sakila/table/film_category.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)      343 2022-01-31 13:44:58.000000 snowddl-0.9.8/snowddl/_config/sample01_02/snowddl_db/sakila/table/inventory.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)      143 2022-01-29 20:43:43.000000 snowddl-0.9.8/snowddl/_config/sample01_02/snowddl_db/sakila/table/language.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)      530 2022-01-31 13:44:58.000000 snowddl-0.9.8/snowddl/_config/sample01_02/snowddl_db/sakila/table/payment.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)      549 2022-01-31 13:44:58.000000 snowddl-0.9.8/snowddl/_config/sample01_02/snowddl_db/sakila/table/rental.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)      579 2022-01-31 13:44:58.000000 snowddl-0.9.8/snowddl/_config/sample01_02/snowddl_db/sakila/table/staff.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)      362 2022-01-31 13:44:58.000000 snowddl-0.9.8/snowddl/_config/sample01_02/snowddl_db/sakila/table/store.yaml
-drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-11 15:26:53.860150 snowddl-0.9.8/snowddl/_config/sample01_02/snowddl_db/sakila/view/
--rw-r--r--   0 vmarkov    (501) staff       (20)      126 2022-02-02 20:30:32.000000 snowddl-0.9.8/snowddl/_config/sample01_02/snowddl_db/sakila/view/actor_list.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)      526 2022-01-29 19:43:23.000000 snowddl-0.9.8/snowddl/_config/sample01_02/snowddl_db/sakila/view/customer_list.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)      580 2022-01-29 19:44:18.000000 snowddl-0.9.8/snowddl/_config/sample01_02/snowddl_db/sakila/view/film_list.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)      384 2022-01-29 19:48:01.000000 snowddl-0.9.8/snowddl/_config/sample01_02/snowddl_db/sakila/view/sales_by_film_category.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)      577 2022-01-29 19:47:01.000000 snowddl-0.9.8/snowddl/_config/sample01_02/snowddl_db/sakila/view/sales_by_store.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)      447 2022-01-29 19:45:27.000000 snowddl-0.9.8/snowddl/_config/sample01_02/snowddl_db/sakila/view/staff_list.yaml
-drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-11 15:26:53.860339 snowddl-0.9.8/snowddl/_config/sample01_02/snowddl_db/sakila_sandbox/
--rw-r--r--   0 vmarkov    (501) staff       (20)       97 2022-02-01 16:56:18.000000 snowddl-0.9.8/snowddl/_config/sample01_02/snowddl_db/sakila_sandbox/params.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)      518 2022-07-28 16:18:39.000000 snowddl-0.9.8/snowddl/_config/sample01_02/tech_role.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)     2086 2022-02-02 20:29:39.000000 snowddl-0.9.8/snowddl/_config/sample01_02/user.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)      404 2022-02-02 20:29:39.000000 snowddl-0.9.8/snowddl/_config/sample01_02/warehouse.yaml
-drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-11 15:26:53.861896 snowddl-0.9.8/snowddl/_config/sample02_01/
-drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-11 15:26:53.838314 snowddl-0.9.8/snowddl/_config/sample02_01/another_db/
-drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-11 15:26:53.838355 snowddl-0.9.8/snowddl/_config/sample02_01/another_db/another_schema/
-drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-11 15:26:53.862148 snowddl-0.9.8/snowddl/_config/sample02_01/another_db/another_schema/view/
--rw-r--r--   0 vmarkov    (501) staff       (20)      212 2022-03-27 09:25:23.000000 snowddl-0.9.8/snowddl/_config/sample02_01/another_db/another_schema/view/test_view_1.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)      200 2022-02-17 12:10:30.000000 snowddl-0.9.8/snowddl/_config/sample02_01/network_policy.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)      337 2022-07-28 14:31:03.000000 snowddl-0.9.8/snowddl/_config/sample02_01/outbound_share.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)      139 2022-04-02 10:46:52.000000 snowddl-0.9.8/snowddl/_config/sample02_01/placeholder.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)      245 2022-02-17 14:07:52.000000 snowddl-0.9.8/snowddl/_config/sample02_01/resource_monitor.yaml
-drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-11 15:26:53.838459 snowddl-0.9.8/snowddl/_config/sample02_01/test_db/
-drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-11 15:26:53.839231 snowddl-0.9.8/snowddl/_config/sample02_01/test_db/test_schema/
-drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-11 15:26:53.862651 snowddl-0.9.8/snowddl/_config/sample02_01/test_db/test_schema/external_function/
--rw-r--r--   0 vmarkov    (501) staff       (20)      171 2022-03-02 15:34:20.000000 snowddl-0.9.8/snowddl/_config/sample02_01/test_db/test_schema/external_function/local_echo(varchar).yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)      341 2022-03-02 16:36:18.000000 snowddl-0.9.8/snowddl/_config/sample02_01/test_db/test_schema/external_function/test_translator(varchar).yaml
-drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-11 15:26:53.866219 snowddl-0.9.8/snowddl/_config/sample02_01/test_db/test_schema/external_table/
--rw-r--r--   0 vmarkov    (501) staff       (20)      369 2022-05-09 13:11:09.000000 snowddl-0.9.8/snowddl/_config/sample02_01/test_db/test_schema/external_table/test_ext_table_1.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)      336 2022-05-09 13:11:06.000000 snowddl-0.9.8/snowddl/_config/sample02_01/test_db/test_schema/external_table/test_ext_table_2.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)      371 2022-05-09 13:19:07.000000 snowddl-0.9.8/snowddl/_config/sample02_01/test_db/test_schema/external_table/test_ext_table_3.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)      356 2022-05-09 13:11:45.000000 snowddl-0.9.8/snowddl/_config/sample02_01/test_db/test_schema/external_table/test_ext_table_4.yaml
-drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-11 15:26:53.866887 snowddl-0.9.8/snowddl/_config/sample02_01/test_db/test_schema/file_format/
--rw-r--r--   0 vmarkov    (501) staff       (20)       77 2022-02-10 12:48:07.000000 snowddl-0.9.8/snowddl/_config/sample02_01/test_db/test_schema/file_format/test_avro_format.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)      130 2022-02-10 12:37:46.000000 snowddl-0.9.8/snowddl/_config/sample02_01/test_db/test_schema/file_format/test_csv_format.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)       76 2022-02-10 12:37:46.000000 snowddl-0.9.8/snowddl/_config/sample02_01/test_db/test_schema/file_format/test_parquet_format.yaml
-drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-11 15:26:53.868316 snowddl-0.9.8/snowddl/_config/sample02_01/test_db/test_schema/function/
--rw-r--r--   0 vmarkov    (501) staff       (20)      451 2022-05-09 13:02:38.000000 snowddl-0.9.8/snowddl/_config/sample02_01/test_db/test_schema/function/test1_xx_hash(varchar).yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)      245 2022-05-09 13:02:38.000000 snowddl-0.9.8/snowddl/_config/sample02_01/test_db/test_schema/function/test2_xx_hash(varchar).yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)      275 2022-06-15 18:56:33.000000 snowddl-0.9.8/snowddl/_config/sample02_01/test_db/test_schema/function/test_py_udf().yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)       82 2022-03-02 16:35:42.000000 snowddl-0.9.8/snowddl/_config/sample02_01/test_db/test_schema/function/test_req_translator(object).yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)       82 2022-03-02 16:35:42.000000 snowddl-0.9.8/snowddl/_config/sample02_01/test_db/test_schema/function/test_res_translator(object).yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)      112 2022-07-27 18:38:50.000000 snowddl-0.9.8/snowddl/_config/sample02_01/test_db/test_schema/function/test_secure_udf(varchar).yaml
-drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-11 15:26:53.868813 snowddl-0.9.8/snowddl/_config/sample02_01/test_db/test_schema/masking_policy/
--rw-r--r--   0 vmarkov    (501) staff       (20)      177 2022-02-10 12:19:48.000000 snowddl-0.9.8/snowddl/_config/sample02_01/test_db/test_schema/masking_policy/test_masking_policy_1.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)      245 2022-02-10 12:19:48.000000 snowddl-0.9.8/snowddl/_config/sample02_01/test_db/test_schema/masking_policy/test_masking_policy_2.yaml
-drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-11 15:26:53.869067 snowddl-0.9.8/snowddl/_config/sample02_01/test_db/test_schema/materialized_view/
--rw-r--r--   0 vmarkov    (501) staff       (20)       51 2022-02-10 12:09:31.000000 snowddl-0.9.8/snowddl/_config/sample02_01/test_db/test_schema/materialized_view/test_mat_view_1.yaml
-drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-11 15:26:53.869466 snowddl-0.9.8/snowddl/_config/sample02_01/test_db/test_schema/pipe/
--rw-r--r--   0 vmarkov    (501) staff       (20)       77 2022-05-09 13:02:38.000000 snowddl-0.9.8/snowddl/_config/sample02_01/test_db/test_schema/pipe/test_pipe_1.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)      142 2022-05-09 13:02:38.000000 snowddl-0.9.8/snowddl/_config/sample02_01/test_db/test_schema/pipe/test_pipe_2.yaml
-drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-11 15:26:53.870334 snowddl-0.9.8/snowddl/_config/sample02_01/test_db/test_schema/procedure/
--rw-r--r--   0 vmarkov    (501) staff       (20)      137 2022-02-10 12:51:24.000000 snowddl-0.9.8/snowddl/_config/sample02_01/test_db/test_schema/procedure/test1_proc(number).yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)      553 2022-06-27 10:17:56.000000 snowddl-0.9.8/snowddl/_config/sample02_01/test_db/test_schema/procedure/test2_proc(varchar).yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)      177 2022-06-27 10:07:58.000000 snowddl-0.9.8/snowddl/_config/sample02_01/test_db/test_schema/procedure/test3_proc().yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)      312 2022-06-27 10:47:45.000000 snowddl-0.9.8/snowddl/_config/sample02_01/test_db/test_schema/procedure/test4_proc().yaml
-drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-11 15:26:53.870879 snowddl-0.9.8/snowddl/_config/sample02_01/test_db/test_schema/row_access_policy/
--rw-r--r--   0 vmarkov    (501) staff       (20)      152 2022-02-10 13:32:20.000000 snowddl-0.9.8/snowddl/_config/sample02_01/test_db/test_schema/row_access_policy/test_row_policy_1.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)      172 2022-02-10 13:34:07.000000 snowddl-0.9.8/snowddl/_config/sample02_01/test_db/test_schema/row_access_policy/test_row_policy_2.yaml
-drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-11 15:26:53.871496 snowddl-0.9.8/snowddl/_config/sample02_01/test_db/test_schema/stage/
--rw-r--r--   0 vmarkov    (501) staff       (20)      109 2022-05-09 13:02:38.000000 snowddl-0.9.8/snowddl/_config/sample02_01/test_db/test_schema/stage/test_external_stage.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)      119 2022-02-22 12:18:39.000000 snowddl-0.9.8/snowddl/_config/sample02_01/test_db/test_schema/stage/test_internal_stage.yaml
-drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-11 15:26:53.872176 snowddl-0.9.8/snowddl/_config/sample02_01/test_db/test_schema/stream/
--rw-r--r--   0 vmarkov    (501) staff       (20)       87 2022-02-10 12:03:54.000000 snowddl-0.9.8/snowddl/_config/sample02_01/test_db/test_schema/stream/test_stream_1.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)       76 2022-02-10 12:09:31.000000 snowddl-0.9.8/snowddl/_config/sample02_01/test_db/test_schema/stream/test_stream_2.yaml
-drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-11 15:26:53.873397 snowddl-0.9.8/snowddl/_config/sample02_01/test_db/test_schema/table/
--rw-r--r--   0 vmarkov    (501) staff       (20)       95 2022-06-05 20:44:28.000000 snowddl-0.9.8/snowddl/_config/sample02_01/test_db/test_schema/table/test_table_1.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)       72 2022-02-10 11:53:23.000000 snowddl-0.9.8/snowddl/_config/sample02_01/test_db/test_schema/table/test_table_2.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)      189 2022-08-08 16:02:29.000000 snowddl-0.9.8/snowddl/_config/sample02_01/test_db/test_schema/table/test_table_3.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)      226 2022-08-08 16:17:12.000000 snowddl-0.9.8/snowddl/_config/sample02_01/test_db/test_schema/table/test_table_4.yaml
-drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-11 15:26:53.874243 snowddl-0.9.8/snowddl/_config/sample02_01/test_db/test_schema/task/
--rw-r--r--   0 vmarkov    (501) staff       (20)       75 2022-02-10 13:09:38.000000 snowddl-0.9.8/snowddl/_config/sample02_01/test_db/test_schema/task/test_task_1.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)       80 2022-08-08 16:30:21.000000 snowddl-0.9.8/snowddl/_config/sample02_01/test_db/test_schema/task/test_task_2.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)       96 2022-08-08 16:30:21.000000 snowddl-0.9.8/snowddl/_config/sample02_01/test_db/test_schema/task/test_task_3.yaml
--rw-r--r--   0 vmarkov    (501) staff       (20)      173 2022-02-22 12:18:39.000000 snowddl-0.9.8/snowddl/_config/sample02_01/warehouse.yaml
-drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-11 15:26:53.875420 snowddl-0.9.8/snowddl/app/
--rw-r--r--   0 vmarkov    (501) staff       (20)       92 2022-06-05 17:29:09.000000 snowddl-0.9.8/snowddl/app/__init__.py
--rw-r--r--   0 vmarkov    (501) staff       (20)    15519 2022-08-23 09:44:54.000000 snowddl-0.9.8/snowddl/app/base.py
--rw-r--r--   0 vmarkov    (501) staff       (20)     5539 2022-08-23 14:53:35.000000 snowddl-0.9.8/snowddl/app/convert.py
--rw-r--r--   0 vmarkov    (501) staff       (20)     7744 2022-08-23 14:53:35.000000 snowddl-0.9.8/snowddl/app/singledb.py
-drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-11 15:26:53.878576 snowddl-0.9.8/snowddl/blueprint/
--rw-r--r--   0 vmarkov    (501) staff       (20)     1749 2022-07-28 16:17:49.000000 snowddl-0.9.8/snowddl/blueprint/__init__.py
--rw-r--r--   0 vmarkov    (501) staff       (20)     8950 2022-08-08 16:27:12.000000 snowddl-0.9.8/snowddl/blueprint/blueprint.py
--rw-r--r--   0 vmarkov    (501) staff       (20)      703 2022-08-08 15:14:25.000000 snowddl-0.9.8/snowddl/blueprint/column.py
--rw-r--r--   0 vmarkov    (501) staff       (20)     2887 2022-10-04 08:35:33.000000 snowddl-0.9.8/snowddl/blueprint/data_type.py
--rw-r--r--   0 vmarkov    (501) staff       (20)      113 2022-02-10 16:03:51.000000 snowddl-0.9.8/snowddl/blueprint/edition.py
--rw-r--r--   0 vmarkov    (501) staff       (20)      353 2022-05-29 21:46:56.000000 snowddl-0.9.8/snowddl/blueprint/grant.py
--rw-r--r--   0 vmarkov    (501) staff       (20)     5604 2022-08-08 14:54:34.000000 snowddl-0.9.8/snowddl/blueprint/ident.py
--rw-r--r--   0 vmarkov    (501) staff       (20)     3253 2022-07-28 16:17:49.000000 snowddl-0.9.8/snowddl/blueprint/ident_builder.py
--rw-r--r--   0 vmarkov    (501) staff       (20)     5327 2022-07-28 13:20:21.000000 snowddl-0.9.8/snowddl/blueprint/object_type.py
--rw-r--r--   0 vmarkov    (501) staff       (20)      620 2022-05-29 22:22:13.000000 snowddl-0.9.8/snowddl/blueprint/reference.py
--rw-r--r--   0 vmarkov    (501) staff       (20)      313 2022-05-29 22:22:13.000000 snowddl-0.9.8/snowddl/blueprint/stage.py
--rw-r--r--   0 vmarkov    (501) staff       (20)     2935 2022-07-28 16:06:52.000000 snowddl-0.9.8/snowddl/config.py
--rw-r--r--   0 vmarkov    (501) staff       (20)     4027 2022-05-30 08:01:02.000000 snowddl-0.9.8/snowddl/context.py
-drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-11 15:26:53.881161 snowddl-0.9.8/snowddl/converter/
--rw-r--r--   0 vmarkov    (501) staff       (20)      518 2022-10-05 14:51:29.000000 snowddl-0.9.8/snowddl/converter/__init__.py
--rw-r--r--   0 vmarkov    (501) staff       (20)      581 2022-02-21 10:26:09.000000 snowddl-0.9.8/snowddl/converter/_yaml.py
--rw-r--r--   0 vmarkov    (501) staff       (20)     3890 2022-08-13 16:43:51.000000 snowddl-0.9.8/snowddl/converter/abc_converter.py
--rw-r--r--   0 vmarkov    (501) staff       (20)      628 2022-05-30 12:51:04.000000 snowddl-0.9.8/snowddl/converter/abc_schema_object_converter.py
--rw-r--r--   0 vmarkov    (501) staff       (20)      858 2022-02-15 11:28:36.000000 snowddl-0.9.8/snowddl/converter/database.py
--rw-r--r--   0 vmarkov    (501) staff       (20)      884 2022-02-15 11:28:36.000000 snowddl-0.9.8/snowddl/converter/schema.py
--rw-r--r--   0 vmarkov    (501) staff       (20)     1654 2022-02-14 19:14:50.000000 snowddl-0.9.8/snowddl/converter/sequence.py
--rw-r--r--   0 vmarkov    (501) staff       (20)     6436 2022-10-11 15:05:29.000000 snowddl-0.9.8/snowddl/converter/table.py
--rw-r--r--   0 vmarkov    (501) staff       (20)     2642 2022-10-05 08:29:31.000000 snowddl-0.9.8/snowddl/converter/view.py
--rw-r--r--   0 vmarkov    (501) staff       (20)     3673 2022-08-19 18:36:34.000000 snowddl-0.9.8/snowddl/engine.py
--rw-r--r--   0 vmarkov    (501) staff       (20)      708 2022-01-20 18:29:46.000000 snowddl-0.9.8/snowddl/error.py
--rw-r--r--   0 vmarkov    (501) staff       (20)     5167 2022-08-19 18:36:34.000000 snowddl-0.9.8/snowddl/formatter.py
-drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-11 15:26:53.889252 snowddl-0.9.8/snowddl/parser/
--rw-r--r--   0 vmarkov    (501) staff       (20)     2126 2022-07-27 15:52:54.000000 snowddl-0.9.8/snowddl/parser/__init__.py
--rw-r--r--   0 vmarkov    (501) staff       (20)     2366 2022-08-13 16:39:57.000000 snowddl-0.9.8/snowddl/parser/_parsed_file.py
--rw-r--r--   0 vmarkov    (501) staff       (20)     2290 2022-07-28 14:14:09.000000 snowddl-0.9.8/snowddl/parser/abc_parser.py
--rw-r--r--   0 vmarkov    (501) staff       (20)      774 2022-03-17 12:54:13.000000 snowddl-0.9.8/snowddl/parser/account_params.py
--rw-r--r--   0 vmarkov    (501) staff       (20)     4667 2022-07-28 14:23:01.000000 snowddl-0.9.8/snowddl/parser/business_role.py
--rw-r--r--   0 vmarkov    (501) staff       (20)     1197 2022-05-29 22:30:16.000000 snowddl-0.9.8/snowddl/parser/database.py
--rw-r--r--   0 vmarkov    (501) staff       (20)     3281 2022-07-26 19:08:25.000000 snowddl-0.9.8/snowddl/parser/external_function.py
--rw-r--r--   0 vmarkov    (501) staff       (20)     7538 2022-05-30 12:53:24.000000 snowddl-0.9.8/snowddl/parser/external_table.py
--rw-r--r--   0 vmarkov    (501) staff       (20)     1207 2022-05-30 12:51:04.000000 snowddl-0.9.8/snowddl/parser/file_format.py
--rw-r--r--   0 vmarkov    (501) staff       (20)     3939 2022-06-15 18:52:38.000000 snowddl-0.9.8/snowddl/parser/function.py
--rw-r--r--   0 vmarkov    (501) staff       (20)     1414 2022-07-26 18:21:20.000000 snowddl-0.9.8/snowddl/parser/inbound_share.py
--rw-r--r--   0 vmarkov    (501) staff       (20)     2638 2022-05-30 11:32:04.000000 snowddl-0.9.8/snowddl/parser/masking_policy.py
--rw-r--r--   0 vmarkov    (501) staff       (20)     1802 2022-05-29 22:48:19.000000 snowddl-0.9.8/snowddl/parser/materialized_view.py
--rw-r--r--   0 vmarkov    (501) staff       (20)     1452 2022-02-22 11:52:26.000000 snowddl-0.9.8/snowddl/parser/network_policy.py
--rw-r--r--   0 vmarkov    (501) staff       (20)     2996 2022-07-28 16:14:37.000000 snowddl-0.9.8/snowddl/parser/outbound_share.py
--rw-r--r--   0 vmarkov    (501) staff       (20)     2856 2022-05-30 11:32:04.000000 snowddl-0.9.8/snowddl/parser/pipe.py
--rw-r--r--   0 vmarkov    (501) staff       (20)     1393 2022-05-24 16:33:42.000000 snowddl-0.9.8/snowddl/parser/placeholder.py
--rw-r--r--   0 vmarkov    (501) staff       (20)     3902 2022-06-27 10:03:47.000000 snowddl-0.9.8/snowddl/parser/procedure.py
--rw-r--r--   0 vmarkov    (501) staff       (20)     1416 2022-02-22 13:46:12.000000 snowddl-0.9.8/snowddl/parser/resource_monitor.py
--rw-r--r--   0 vmarkov    (501) staff       (20)     2540 2022-05-30 11:32:05.000000 snowddl-0.9.8/snowddl/parser/row_access_policy.py
--rw-r--r--   0 vmarkov    (501) staff       (20)     3099 2022-05-30 11:32:04.000000 snowddl-0.9.8/snowddl/parser/schema.py
--rw-r--r--   0 vmarkov    (501) staff       (20)      950 2022-05-29 22:48:19.000000 snowddl-0.9.8/snowddl/parser/sequence.py
--rw-r--r--   0 vmarkov    (501) staff       (20)     3006 2022-05-30 11:32:04.000000 snowddl-0.9.8/snowddl/parser/stage.py
--rw-r--r--   0 vmarkov    (501) staff       (20)     1485 2022-05-30 11:32:04.000000 snowddl-0.9.8/snowddl/parser/stream.py
--rw-r--r--   0 vmarkov    (501) staff       (20)     8345 2022-08-08 15:14:25.000000 snowddl-0.9.8/snowddl/parser/table.py
--rw-r--r--   0 vmarkov    (501) staff       (20)     1985 2022-05-30 11:32:04.000000 snowddl-0.9.8/snowddl/parser/tag.py
--rw-r--r--   0 vmarkov    (501) staff       (20)     2466 2022-08-08 17:18:54.000000 snowddl-0.9.8/snowddl/parser/task.py
--rw-r--r--   0 vmarkov    (501) staff       (20)     2242 2022-07-28 16:17:49.000000 snowddl-0.9.8/snowddl/parser/tech_role.py
--rw-r--r--   0 vmarkov    (501) staff       (20)     4729 2022-05-30 12:51:04.000000 snowddl-0.9.8/snowddl/parser/user.py
--rw-r--r--   0 vmarkov    (501) staff       (20)     1795 2022-05-30 11:32:04.000000 snowddl-0.9.8/snowddl/parser/view.py
--rw-r--r--   0 vmarkov    (501) staff       (20)     1851 2022-05-29 22:48:49.000000 snowddl-0.9.8/snowddl/parser/warehouse.py
--rw-r--r--   0 vmarkov    (501) staff       (20)     1250 2022-08-19 18:40:50.000000 snowddl-0.9.8/snowddl/query_builder.py
-drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-11 15:26:53.899720 snowddl-0.9.8/snowddl/resolver/
--rw-r--r--   0 vmarkov    (501) staff       (20)     3001 2022-07-27 18:00:28.000000 snowddl-0.9.8/snowddl/resolver/__init__.py
--rw-r--r--   0 vmarkov    (501) staff       (20)      963 2022-01-19 18:08:26.000000 snowddl-0.9.8/snowddl/resolver/_utils.py
--rw-r--r--   0 vmarkov    (501) staff       (20)     6870 2022-08-08 17:40:46.000000 snowddl-0.9.8/snowddl/resolver/abc_resolver.py
--rw-rw-rw-   0 vmarkov    (501) staff       (20)     7876 2022-09-09 15:25:17.000000 snowddl-0.9.8/snowddl/resolver/abc_role_resolver.py
--rw-r--r--   0 vmarkov    (501) staff       (20)     1497 2022-06-05 20:46:57.000000 snowddl-0.9.8/snowddl/resolver/abc_schema_object_resolver.py
--rw-r--r--   0 vmarkov    (501) staff       (20)     1935 2022-02-01 17:00:20.000000 snowddl-0.9.8/snowddl/resolver/account_params.py
--rw-r--r--   0 vmarkov    (501) staff       (20)      355 2022-01-28 17:04:59.000000 snowddl-0.9.8/snowddl/resolver/business_role.py
--rw-r--r--   0 vmarkov    (501) staff       (20)     2937 2022-05-30 08:45:04.000000 snowddl-0.9.8/snowddl/resolver/database.py
--rw-r--r--   0 vmarkov    (501) staff       (20)     5079 2022-08-15 17:42:29.000000 snowddl-0.9.8/snowddl/resolver/external_function.py
--rw-r--r--   0 vmarkov    (501) staff       (20)     5484 2022-08-15 17:42:29.000000 snowddl-0.9.8/snowddl/resolver/external_table.py
--rw-r--r--   0 vmarkov    (501) staff       (20)     3431 2022-08-15 17:52:08.000000 snowddl-0.9.8/snowddl/resolver/file_format.py
--rw-r--r--   0 vmarkov    (501) staff       (20)     3825 2022-01-30 19:42:27.000000 snowddl-0.9.8/snowddl/resolver/foreign_key.py
--rw-r--r--   0 vmarkov    (501) staff       (20)     4926 2022-08-15 17:42:29.000000 snowddl-0.9.8/snowddl/resolver/function.py
--rw-r--r--   0 vmarkov    (501) staff       (20)     3275 2022-07-26 19:22:57.000000 snowddl-0.9.8/snowddl/resolver/inbound_share.py
--rw-r--r--   0 vmarkov    (501) staff       (20)     2070 2022-07-26 19:12:21.000000 snowddl-0.9.8/snowddl/resolver/inbound_share_role.py
--rw-r--r--   0 vmarkov    (501) staff       (20)     7690 2022-06-05 21:30:51.000000 snowddl-0.9.8/snowddl/resolver/masking_policy.py
--rw-r--r--   0 vmarkov    (501) staff       (20)     3331 2022-03-02 16:20:07.000000 snowddl-0.9.8/snowddl/resolver/materialized_view.py
--rw-r--r--   0 vmarkov    (501) staff       (20)     4022 2022-02-17 12:09:48.000000 snowddl-0.9.8/snowddl/resolver/network_policy.py
--rw-r--r--   0 vmarkov    (501) staff       (20)     5487 2022-07-28 16:24:43.000000 snowddl-0.9.8/snowddl/resolver/outbound_share.py
--rw-r--r--   0 vmarkov    (501) staff       (20)     5424 2022-05-09 13:02:38.000000 snowddl-0.9.8/snowddl/resolver/pipe.py
--rw-r--r--   0 vmarkov    (501) staff       (20)     2810 2022-05-30 12:36:19.000000 snowddl-0.9.8/snowddl/resolver/primary_key.py
--rw-r--r--   0 vmarkov    (501) staff       (20)     4708 2022-08-15 17:42:29.000000 snowddl-0.9.8/snowddl/resolver/procedure.py
--rw-r--r--   0 vmarkov    (501) staff       (20)     4330 2022-02-17 14:03:21.000000 snowddl-0.9.8/snowddl/resolver/resource_monitor.py
--rw-r--r--   0 vmarkov    (501) staff       (20)     8299 2022-06-05 21:30:51.000000 snowddl-0.9.8/snowddl/resolver/row_access_policy.py
--rw-r--r--   0 vmarkov    (501) staff       (20)     3681 2022-06-05 20:46:57.000000 snowddl-0.9.8/snowddl/resolver/schema.py
--rw-r--r--   0 vmarkov    (501) staff       (20)     6253 2022-05-30 11:42:58.000000 snowddl-0.9.8/snowddl/resolver/schema_role.py
--rw-r--r--   0 vmarkov    (501) staff       (20)     2750 2022-01-30 19:42:27.000000 snowddl-0.9.8/snowddl/resolver/sequence.py
--rw-r--r--   0 vmarkov    (501) staff       (20)     4586 2022-07-13 15:52:58.000000 snowddl-0.9.8/snowddl/resolver/stage.py
--rw-r--r--   0 vmarkov    (501) staff       (20)     4273 2022-08-13 16:44:33.000000 snowddl-0.9.8/snowddl/resolver/stage_file.py
--rw-r--r--   0 vmarkov    (501) staff       (20)     3835 2022-01-29 18:55:37.000000 snowddl-0.9.8/snowddl/resolver/stream.py
--rw-r--r--   0 vmarkov    (501) staff       (20)    14403 2022-08-08 16:15:19.000000 snowddl-0.9.8/snowddl/resolver/table.py
--rw-r--r--   0 vmarkov    (501) staff       (20)     6621 2022-05-30 08:52:44.000000 snowddl-0.9.8/snowddl/resolver/tag.py
--rw-r--r--   0 vmarkov    (501) staff       (20)     4525 2022-02-08 11:55:24.000000 snowddl-0.9.8/snowddl/resolver/task.py
--rw-r--r--   0 vmarkov    (501) staff       (20)      339 2022-01-28 17:04:59.000000 snowddl-0.9.8/snowddl/resolver/tech_role.py
--rw-r--r--   0 vmarkov    (501) staff       (20)     2421 2022-01-30 19:42:27.000000 snowddl-0.9.8/snowddl/resolver/unique_key.py
--rw-r--r--   0 vmarkov    (501) staff       (20)    10354 2022-08-29 20:53:13.000000 snowddl-0.9.8/snowddl/resolver/user.py
--rw-r--r--   0 vmarkov    (501) staff       (20)     1887 2022-09-09 15:33:30.000000 snowddl-0.9.8/snowddl/resolver/user_role.py
--rw-r--r--   0 vmarkov    (501) staff       (20)     4352 2022-05-30 09:05:07.000000 snowddl-0.9.8/snowddl/resolver/view.py
--rw-r--r--   0 vmarkov    (501) staff       (20)     5708 2022-05-02 14:08:40.000000 snowddl-0.9.8/snowddl/resolver/warehouse.py
--rw-r--r--   0 vmarkov    (501) staff       (20)     1955 2022-05-30 11:32:05.000000 snowddl-0.9.8/snowddl/resolver/warehouse_role.py
--rw-r--r--   0 vmarkov    (501) staff       (20)     2619 2022-06-05 21:00:18.000000 snowddl-0.9.8/snowddl/schema_cache.py
--rw-r--r--   0 vmarkov    (501) staff       (20)      920 2022-07-26 15:58:33.000000 snowddl-0.9.8/snowddl/settings.py
--rw-r--r--   0 vmarkov    (501) staff       (20)       22 2022-10-11 15:25:49.000000 snowddl-0.9.8/snowddl/version.py
-drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-11 15:26:53.843995 snowddl-0.9.8/snowddl.egg-info/
--rw-r--r--   0 vmarkov    (501) staff       (20)     1786 2022-10-11 15:26:53.000000 snowddl-0.9.8/snowddl.egg-info/PKG-INFO
--rw-r--r--   0 vmarkov    (501) staff       (20)    12288 2022-10-11 15:26:53.000000 snowddl-0.9.8/snowddl.egg-info/SOURCES.txt
--rw-r--r--   0 vmarkov    (501) staff       (20)        1 2022-10-11 15:26:53.000000 snowddl-0.9.8/snowddl.egg-info/dependency_links.txt
--rw-r--r--   0 vmarkov    (501) staff       (20)      159 2022-10-11 15:26:53.000000 snowddl-0.9.8/snowddl.egg-info/entry_points.txt
--rw-r--r--   0 vmarkov    (501) staff       (20)       60 2022-10-11 15:26:53.000000 snowddl-0.9.8/snowddl.egg-info/requires.txt
--rw-r--r--   0 vmarkov    (501) staff       (20)        8 2022-10-11 15:26:53.000000 snowddl-0.9.8/snowddl.egg-info/top_level.txt
+drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-13 09:47:37.126435 snowddl-0.9.9/
+-rw-r--r--   0 vmarkov    (501) staff       (20)    11309 2022-01-27 15:42:20.000000 snowddl-0.9.9/LICENSE.txt
+-rw-r--r--   0 vmarkov    (501) staff       (20)       61 2022-01-27 16:29:40.000000 snowddl-0.9.9/MANIFEST.in
+-rw-r--r--   0 vmarkov    (501) staff       (20)     1786 2022-10-13 09:47:37.126258 snowddl-0.9.9/PKG-INFO
+-rw-r--r--   0 vmarkov    (501) staff       (20)     3601 2022-10-04 08:35:09.000000 snowddl-0.9.9/README.md
+-rw-r--r--   0 vmarkov    (501) staff       (20)       38 2022-10-13 09:47:37.126480 snowddl-0.9.9/setup.cfg
+-rw-r--r--   0 vmarkov    (501) staff       (20)     2499 2022-10-04 10:38:37.000000 snowddl-0.9.9/setup.py
+drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-13 09:47:37.074288 snowddl-0.9.9/snowddl/
+-rw-r--r--   0 vmarkov    (501) staff       (20)      380 2022-08-19 13:39:10.000000 snowddl-0.9.9/snowddl/__init__.py
+drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-13 09:47:37.069646 snowddl-0.9.9/snowddl/_config/
+drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-13 09:47:37.075841 snowddl-0.9.9/snowddl/_config/sample01_01/
+-rw-r--r--   0 vmarkov    (501) staff       (20)     1050 2022-05-12 16:00:34.000000 snowddl-0.9.9/snowddl/_config/sample01_01/business_role.yaml
+drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-13 09:47:37.068847 snowddl-0.9.9/snowddl/_config/sample01_01/snowddl_db/
+drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-13 09:47:37.076084 snowddl-0.9.9/snowddl/_config/sample01_01/snowddl_db/bookings/
+drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-13 09:47:37.076487 snowddl-0.9.9/snowddl/_config/sample01_01/snowddl_db/bookings/function/
+-rw-r--r--   0 vmarkov    (501) staff       (20)      305 2022-01-31 13:45:39.000000 snowddl-0.9.9/snowddl/_config/sample01_01/snowddl_db/bookings/function/lang(object).yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)      103 2022-01-31 12:37:22.000000 snowddl-0.9.9/snowddl/_config/sample01_01/snowddl_db/bookings/function/now().yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)       41 2022-01-31 11:51:07.000000 snowddl-0.9.9/snowddl/_config/sample01_01/snowddl_db/bookings/params.yaml
+drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-13 09:47:37.076643 snowddl-0.9.9/snowddl/_config/sample01_01/snowddl_db/bookings/procedure/
+-rw-r--r--   0 vmarkov    (501) staff       (20)      311 2022-02-01 17:44:32.000000 snowddl-0.9.9/snowddl/_config/sample01_01/snowddl_db/bookings/procedure/check_in(varchar,number,number,varchar).yaml
+drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-13 09:47:37.076795 snowddl-0.9.9/snowddl/_config/sample01_01/snowddl_db/bookings/sequence/
+-rw-r--r--   0 vmarkov    (501) staff       (20)       21 2022-01-31 12:00:29.000000 snowddl-0.9.9/snowddl/_config/sample01_01/snowddl_db/bookings/sequence/flights_id_seq.yaml
+drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-13 09:47:37.077912 snowddl-0.9.9/snowddl/_config/sample01_01/snowddl_db/bookings/table/
+-rw-r--r--   0 vmarkov    (501) staff       (20)      496 2022-01-31 13:10:50.000000 snowddl-0.9.9/snowddl/_config/sample01_01/snowddl_db/bookings/table/aircrafts_data.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)      637 2022-01-31 13:10:50.000000 snowddl-0.9.9/snowddl/_config/sample01_01/snowddl_db/bookings/table/airports_data.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)     1013 2022-01-31 11:06:29.000000 snowddl-0.9.9/snowddl/_config/sample01_01/snowddl_db/bookings/table/boarding_passes.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)      649 2022-01-31 12:23:15.000000 snowddl-0.9.9/snowddl/_config/sample01_01/snowddl_db/bookings/table/bookings.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)     2087 2022-01-31 13:46:08.000000 snowddl-0.9.9/snowddl/_config/sample01_01/snowddl_db/bookings/table/flights.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)      590 2022-01-31 11:26:43.000000 snowddl-0.9.9/snowddl/_config/sample01_01/snowddl_db/bookings/table/seats.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)      681 2022-01-31 11:30:32.000000 snowddl-0.9.9/snowddl/_config/sample01_01/snowddl_db/bookings/table/ticket_flights.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)      960 2022-01-31 11:34:08.000000 snowddl-0.9.9/snowddl/_config/sample01_01/snowddl_db/bookings/table/tickets.yaml
+drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-13 09:47:37.078485 snowddl-0.9.9/snowddl/_config/sample01_01/snowddl_db/bookings/view/
+-rw-r--r--   0 vmarkov    (501) staff       (20)      431 2022-01-31 13:34:28.000000 snowddl-0.9.9/snowddl/_config/sample01_01/snowddl_db/bookings/view/aircrafts.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)      663 2022-01-31 13:34:55.000000 snowddl-0.9.9/snowddl/_config/sample01_01/snowddl_db/bookings/view/airports.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)     1103 2022-01-31 13:37:38.000000 snowddl-0.9.9/snowddl/_config/sample01_01/snowddl_db/bookings/view/flights_v.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)     1377 2022-01-31 13:37:38.000000 snowddl-0.9.9/snowddl/_config/sample01_01/snowddl_db/bookings/view/routes.yaml
+drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-13 09:47:37.068786 snowddl-0.9.9/snowddl/_config/sample01_01/snowddl_db/sakila/
+drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-13 09:47:37.080770 snowddl-0.9.9/snowddl/_config/sample01_01/snowddl_db/sakila/table/
+-rw-r--r--   0 vmarkov    (501) staff       (20)      169 2022-01-29 19:17:21.000000 snowddl-0.9.9/snowddl/_config/sample01_01/snowddl_db/sakila/table/actor.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)      377 2022-01-31 13:44:58.000000 snowddl-0.9.9/snowddl/_config/sample01_01/snowddl_db/sakila/table/address.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)      143 2022-01-29 20:43:43.000000 snowddl-0.9.9/snowddl/_config/sample01_01/snowddl_db/sakila/table/category.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)      265 2022-01-31 13:44:58.000000 snowddl-0.9.9/snowddl/_config/sample01_01/snowddl_db/sakila/table/city.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)      135 2022-01-29 20:30:41.000000 snowddl-0.9.9/snowddl/_config/sample01_01/snowddl_db/sakila/table/country.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)      543 2022-01-31 13:44:58.000000 snowddl-0.9.9/snowddl/_config/sample01_01/snowddl_db/sakila/table/customer.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)      769 2022-01-31 13:44:58.000000 snowddl-0.9.9/snowddl/_config/sample01_01/snowddl_db/sakila/table/film.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)      311 2022-01-31 13:44:58.000000 snowddl-0.9.9/snowddl/_config/sample01_01/snowddl_db/sakila/table/film_actor.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)      324 2022-01-31 13:44:58.000000 snowddl-0.9.9/snowddl/_config/sample01_01/snowddl_db/sakila/table/film_category.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)      343 2022-01-31 13:44:58.000000 snowddl-0.9.9/snowddl/_config/sample01_01/snowddl_db/sakila/table/inventory.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)      143 2022-01-29 20:43:43.000000 snowddl-0.9.9/snowddl/_config/sample01_01/snowddl_db/sakila/table/language.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)      530 2022-01-31 13:44:58.000000 snowddl-0.9.9/snowddl/_config/sample01_01/snowddl_db/sakila/table/payment.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)      549 2022-01-31 13:44:58.000000 snowddl-0.9.9/snowddl/_config/sample01_01/snowddl_db/sakila/table/rental.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)      579 2022-01-31 13:44:58.000000 snowddl-0.9.9/snowddl/_config/sample01_01/snowddl_db/sakila/table/staff.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)      362 2022-01-31 13:44:58.000000 snowddl-0.9.9/snowddl/_config/sample01_01/snowddl_db/sakila/table/store.yaml
+drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-13 09:47:37.081685 snowddl-0.9.9/snowddl/_config/sample01_01/snowddl_db/sakila/view/
+-rw-r--r--   0 vmarkov    (501) staff       (20)      127 2022-02-02 20:30:32.000000 snowddl-0.9.9/snowddl/_config/sample01_01/snowddl_db/sakila/view/actor_list.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)      526 2022-01-29 19:43:23.000000 snowddl-0.9.9/snowddl/_config/sample01_01/snowddl_db/sakila/view/customer_list.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)      580 2022-01-29 19:44:18.000000 snowddl-0.9.9/snowddl/_config/sample01_01/snowddl_db/sakila/view/film_list.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)      384 2022-01-29 19:48:01.000000 snowddl-0.9.9/snowddl/_config/sample01_01/snowddl_db/sakila/view/sales_by_film_category.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)      577 2022-01-29 19:47:01.000000 snowddl-0.9.9/snowddl/_config/sample01_01/snowddl_db/sakila/view/sales_by_store.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)      447 2022-01-29 19:45:27.000000 snowddl-0.9.9/snowddl/_config/sample01_01/snowddl_db/sakila/view/staff_list.yaml
+drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-13 09:47:37.081823 snowddl-0.9.9/snowddl/_config/sample01_01/snowddl_db/sakila_sandbox/
+-rw-r--r--   0 vmarkov    (501) staff       (20)       97 2022-02-01 16:56:18.000000 snowddl-0.9.9/snowddl/_config/sample01_01/snowddl_db/sakila_sandbox/params.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)      605 2022-05-24 14:49:33.000000 snowddl-0.9.9/snowddl/_config/sample01_01/tech_role.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)     2144 2022-05-24 14:53:10.000000 snowddl-0.9.9/snowddl/_config/sample01_01/user.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)      406 2022-02-01 13:51:42.000000 snowddl-0.9.9/snowddl/_config/sample01_01/warehouse.yaml
+drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-13 09:47:37.082743 snowddl-0.9.9/snowddl/_config/sample01_02/
+-rw-r--r--   0 vmarkov    (501) staff       (20)     1019 2022-05-30 17:15:57.000000 snowddl-0.9.9/snowddl/_config/sample01_02/business_role.yaml
+drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-13 09:47:37.069578 snowddl-0.9.9/snowddl/_config/sample01_02/snowddl_db/
+drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-13 09:47:37.082941 snowddl-0.9.9/snowddl/_config/sample01_02/snowddl_db/bookings/
+drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-13 09:47:37.083487 snowddl-0.9.9/snowddl/_config/sample01_02/snowddl_db/bookings/function/
+-rw-r--r--   0 vmarkov    (501) staff       (20)      305 2022-01-31 13:45:39.000000 snowddl-0.9.9/snowddl/_config/sample01_02/snowddl_db/bookings/function/lang(object).yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)      103 2022-02-02 20:21:25.000000 snowddl-0.9.9/snowddl/_config/sample01_02/snowddl_db/bookings/function/now().yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)       41 2022-01-31 11:51:07.000000 snowddl-0.9.9/snowddl/_config/sample01_02/snowddl_db/bookings/params.yaml
+drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-13 09:47:37.083731 snowddl-0.9.9/snowddl/_config/sample01_02/snowddl_db/bookings/procedure/
+-rw-r--r--   0 vmarkov    (501) staff       (20)      293 2022-02-02 20:19:54.000000 snowddl-0.9.9/snowddl/_config/sample01_02/snowddl_db/bookings/procedure/check_in(varchar,number,number).yaml
+drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-13 09:47:37.084000 snowddl-0.9.9/snowddl/_config/sample01_02/snowddl_db/bookings/sequence/
+-rw-r--r--   0 vmarkov    (501) staff       (20)       59 2022-02-02 20:21:25.000000 snowddl-0.9.9/snowddl/_config/sample01_02/snowddl_db/bookings/sequence/flights_id_seq.yaml
+drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-13 09:47:37.085631 snowddl-0.9.9/snowddl/_config/sample01_02/snowddl_db/bookings/table/
+-rw-r--r--   0 vmarkov    (501) staff       (20)      496 2022-02-02 20:21:25.000000 snowddl-0.9.9/snowddl/_config/sample01_02/snowddl_db/bookings/table/aircrafts_data.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)      724 2022-02-02 20:23:58.000000 snowddl-0.9.9/snowddl/_config/sample01_02/snowddl_db/bookings/table/airports_data.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)      988 2022-02-02 20:22:27.000000 snowddl-0.9.9/snowddl/_config/sample01_02/snowddl_db/bookings/table/boarding_passes.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)      649 2022-01-31 12:23:15.000000 snowddl-0.9.9/snowddl/_config/sample01_02/snowddl_db/bookings/table/bookings.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)     2087 2022-02-02 20:21:25.000000 snowddl-0.9.9/snowddl/_config/sample01_02/snowddl_db/bookings/table/flights.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)      592 2022-02-02 20:22:27.000000 snowddl-0.9.9/snowddl/_config/sample01_02/snowddl_db/bookings/table/seats.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)      681 2022-02-02 20:21:25.000000 snowddl-0.9.9/snowddl/_config/sample01_02/snowddl_db/bookings/table/ticket_flights.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)      960 2022-01-31 11:34:08.000000 snowddl-0.9.9/snowddl/_config/sample01_02/snowddl_db/bookings/table/tickets.yaml
+drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-13 09:47:37.086555 snowddl-0.9.9/snowddl/_config/sample01_02/snowddl_db/bookings/view/
+-rw-r--r--   0 vmarkov    (501) staff       (20)      431 2022-02-14 21:45:55.000000 snowddl-0.9.9/snowddl/_config/sample01_02/snowddl_db/bookings/view/aircrafts.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)      741 2022-02-02 20:42:35.000000 snowddl-0.9.9/snowddl/_config/sample01_02/snowddl_db/bookings/view/airports.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)     1103 2022-01-31 13:37:38.000000 snowddl-0.9.9/snowddl/_config/sample01_02/snowddl_db/bookings/view/flights_v.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)     1377 2022-01-31 13:37:38.000000 snowddl-0.9.9/snowddl/_config/sample01_02/snowddl_db/bookings/view/routes.yaml
+drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-13 09:47:37.069478 snowddl-0.9.9/snowddl/_config/sample01_02/snowddl_db/sakila/
+drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-13 09:47:37.089838 snowddl-0.9.9/snowddl/_config/sample01_02/snowddl_db/sakila/table/
+-rw-r--r--   0 vmarkov    (501) staff       (20)      191 2022-02-02 20:29:39.000000 snowddl-0.9.9/snowddl/_config/sample01_02/snowddl_db/sakila/table/actor.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)      377 2022-01-31 13:44:58.000000 snowddl-0.9.9/snowddl/_config/sample01_02/snowddl_db/sakila/table/address.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)      143 2022-01-29 20:43:43.000000 snowddl-0.9.9/snowddl/_config/sample01_02/snowddl_db/sakila/table/category.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)      265 2022-01-31 13:44:58.000000 snowddl-0.9.9/snowddl/_config/sample01_02/snowddl_db/sakila/table/city.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)      135 2022-01-29 20:30:41.000000 snowddl-0.9.9/snowddl/_config/sample01_02/snowddl_db/sakila/table/country.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)      543 2022-01-31 13:44:58.000000 snowddl-0.9.9/snowddl/_config/sample01_02/snowddl_db/sakila/table/customer.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)      769 2022-01-31 13:44:58.000000 snowddl-0.9.9/snowddl/_config/sample01_02/snowddl_db/sakila/table/film.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)      311 2022-01-31 13:44:58.000000 snowddl-0.9.9/snowddl/_config/sample01_02/snowddl_db/sakila/table/film_actor.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)      324 2022-01-31 13:44:58.000000 snowddl-0.9.9/snowddl/_config/sample01_02/snowddl_db/sakila/table/film_category.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)      343 2022-01-31 13:44:58.000000 snowddl-0.9.9/snowddl/_config/sample01_02/snowddl_db/sakila/table/inventory.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)      143 2022-01-29 20:43:43.000000 snowddl-0.9.9/snowddl/_config/sample01_02/snowddl_db/sakila/table/language.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)      530 2022-01-31 13:44:58.000000 snowddl-0.9.9/snowddl/_config/sample01_02/snowddl_db/sakila/table/payment.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)      549 2022-01-31 13:44:58.000000 snowddl-0.9.9/snowddl/_config/sample01_02/snowddl_db/sakila/table/rental.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)      579 2022-01-31 13:44:58.000000 snowddl-0.9.9/snowddl/_config/sample01_02/snowddl_db/sakila/table/staff.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)      362 2022-01-31 13:44:58.000000 snowddl-0.9.9/snowddl/_config/sample01_02/snowddl_db/sakila/table/store.yaml
+drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-13 09:47:37.091177 snowddl-0.9.9/snowddl/_config/sample01_02/snowddl_db/sakila/view/
+-rw-r--r--   0 vmarkov    (501) staff       (20)      126 2022-02-02 20:30:32.000000 snowddl-0.9.9/snowddl/_config/sample01_02/snowddl_db/sakila/view/actor_list.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)      526 2022-01-29 19:43:23.000000 snowddl-0.9.9/snowddl/_config/sample01_02/snowddl_db/sakila/view/customer_list.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)      580 2022-01-29 19:44:18.000000 snowddl-0.9.9/snowddl/_config/sample01_02/snowddl_db/sakila/view/film_list.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)      384 2022-01-29 19:48:01.000000 snowddl-0.9.9/snowddl/_config/sample01_02/snowddl_db/sakila/view/sales_by_film_category.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)      577 2022-01-29 19:47:01.000000 snowddl-0.9.9/snowddl/_config/sample01_02/snowddl_db/sakila/view/sales_by_store.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)      447 2022-01-29 19:45:27.000000 snowddl-0.9.9/snowddl/_config/sample01_02/snowddl_db/sakila/view/staff_list.yaml
+drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-13 09:47:37.091354 snowddl-0.9.9/snowddl/_config/sample01_02/snowddl_db/sakila_sandbox/
+-rw-r--r--   0 vmarkov    (501) staff       (20)       97 2022-02-01 16:56:18.000000 snowddl-0.9.9/snowddl/_config/sample01_02/snowddl_db/sakila_sandbox/params.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)      518 2022-07-28 16:18:39.000000 snowddl-0.9.9/snowddl/_config/sample01_02/tech_role.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)     2086 2022-02-02 20:29:39.000000 snowddl-0.9.9/snowddl/_config/sample01_02/user.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)      404 2022-02-02 20:29:39.000000 snowddl-0.9.9/snowddl/_config/sample01_02/warehouse.yaml
+drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-13 09:47:37.092808 snowddl-0.9.9/snowddl/_config/sample02_01/
+drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-13 09:47:37.069765 snowddl-0.9.9/snowddl/_config/sample02_01/another_db/
+drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-13 09:47:37.069808 snowddl-0.9.9/snowddl/_config/sample02_01/another_db/another_schema/
+drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-13 09:47:37.093031 snowddl-0.9.9/snowddl/_config/sample02_01/another_db/another_schema/view/
+-rw-r--r--   0 vmarkov    (501) staff       (20)      212 2022-03-27 09:25:23.000000 snowddl-0.9.9/snowddl/_config/sample02_01/another_db/another_schema/view/test_view_1.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)      200 2022-02-17 12:10:30.000000 snowddl-0.9.9/snowddl/_config/sample02_01/network_policy.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)      337 2022-07-28 14:31:03.000000 snowddl-0.9.9/snowddl/_config/sample02_01/outbound_share.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)      139 2022-04-02 10:46:52.000000 snowddl-0.9.9/snowddl/_config/sample02_01/placeholder.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)      245 2022-02-17 14:07:52.000000 snowddl-0.9.9/snowddl/_config/sample02_01/resource_monitor.yaml
+drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-13 09:47:37.069912 snowddl-0.9.9/snowddl/_config/sample02_01/test_db/
+drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-13 09:47:37.070691 snowddl-0.9.9/snowddl/_config/sample02_01/test_db/test_schema/
+drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-13 09:47:37.093480 snowddl-0.9.9/snowddl/_config/sample02_01/test_db/test_schema/external_function/
+-rw-r--r--   0 vmarkov    (501) staff       (20)      171 2022-03-02 15:34:20.000000 snowddl-0.9.9/snowddl/_config/sample02_01/test_db/test_schema/external_function/local_echo(varchar).yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)      341 2022-03-02 16:36:18.000000 snowddl-0.9.9/snowddl/_config/sample02_01/test_db/test_schema/external_function/test_translator(varchar).yaml
+drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-13 09:47:37.094487 snowddl-0.9.9/snowddl/_config/sample02_01/test_db/test_schema/external_table/
+-rw-r--r--   0 vmarkov    (501) staff       (20)      369 2022-05-09 13:11:09.000000 snowddl-0.9.9/snowddl/_config/sample02_01/test_db/test_schema/external_table/test_ext_table_1.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)      336 2022-05-09 13:11:06.000000 snowddl-0.9.9/snowddl/_config/sample02_01/test_db/test_schema/external_table/test_ext_table_2.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)      371 2022-05-09 13:19:07.000000 snowddl-0.9.9/snowddl/_config/sample02_01/test_db/test_schema/external_table/test_ext_table_3.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)      356 2022-05-09 13:11:45.000000 snowddl-0.9.9/snowddl/_config/sample02_01/test_db/test_schema/external_table/test_ext_table_4.yaml
+drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-13 09:47:37.095246 snowddl-0.9.9/snowddl/_config/sample02_01/test_db/test_schema/file_format/
+-rw-r--r--   0 vmarkov    (501) staff       (20)       77 2022-02-10 12:48:07.000000 snowddl-0.9.9/snowddl/_config/sample02_01/test_db/test_schema/file_format/test_avro_format.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)      130 2022-02-10 12:37:46.000000 snowddl-0.9.9/snowddl/_config/sample02_01/test_db/test_schema/file_format/test_csv_format.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)       76 2022-02-10 12:37:46.000000 snowddl-0.9.9/snowddl/_config/sample02_01/test_db/test_schema/file_format/test_parquet_format.yaml
+drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-13 09:47:37.096717 snowddl-0.9.9/snowddl/_config/sample02_01/test_db/test_schema/function/
+-rw-r--r--   0 vmarkov    (501) staff       (20)      451 2022-05-09 13:02:38.000000 snowddl-0.9.9/snowddl/_config/sample02_01/test_db/test_schema/function/test1_xx_hash(varchar).yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)      245 2022-05-09 13:02:38.000000 snowddl-0.9.9/snowddl/_config/sample02_01/test_db/test_schema/function/test2_xx_hash(varchar).yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)      275 2022-06-15 18:56:33.000000 snowddl-0.9.9/snowddl/_config/sample02_01/test_db/test_schema/function/test_py_udf().yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)       82 2022-03-02 16:35:42.000000 snowddl-0.9.9/snowddl/_config/sample02_01/test_db/test_schema/function/test_req_translator(object).yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)       82 2022-03-02 16:35:42.000000 snowddl-0.9.9/snowddl/_config/sample02_01/test_db/test_schema/function/test_res_translator(object).yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)      112 2022-07-27 18:38:50.000000 snowddl-0.9.9/snowddl/_config/sample02_01/test_db/test_schema/function/test_secure_udf(varchar).yaml
+drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-13 09:47:37.097211 snowddl-0.9.9/snowddl/_config/sample02_01/test_db/test_schema/masking_policy/
+-rw-r--r--   0 vmarkov    (501) staff       (20)      177 2022-02-10 12:19:48.000000 snowddl-0.9.9/snowddl/_config/sample02_01/test_db/test_schema/masking_policy/test_masking_policy_1.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)      245 2022-02-10 12:19:48.000000 snowddl-0.9.9/snowddl/_config/sample02_01/test_db/test_schema/masking_policy/test_masking_policy_2.yaml
+drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-13 09:47:37.097452 snowddl-0.9.9/snowddl/_config/sample02_01/test_db/test_schema/materialized_view/
+-rw-r--r--   0 vmarkov    (501) staff       (20)       51 2022-02-10 12:09:31.000000 snowddl-0.9.9/snowddl/_config/sample02_01/test_db/test_schema/materialized_view/test_mat_view_1.yaml
+drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-13 09:47:37.097824 snowddl-0.9.9/snowddl/_config/sample02_01/test_db/test_schema/pipe/
+-rw-r--r--   0 vmarkov    (501) staff       (20)       77 2022-05-09 13:02:38.000000 snowddl-0.9.9/snowddl/_config/sample02_01/test_db/test_schema/pipe/test_pipe_1.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)      142 2022-05-09 13:02:38.000000 snowddl-0.9.9/snowddl/_config/sample02_01/test_db/test_schema/pipe/test_pipe_2.yaml
+drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-13 09:47:37.098536 snowddl-0.9.9/snowddl/_config/sample02_01/test_db/test_schema/procedure/
+-rw-r--r--   0 vmarkov    (501) staff       (20)      137 2022-02-10 12:51:24.000000 snowddl-0.9.9/snowddl/_config/sample02_01/test_db/test_schema/procedure/test1_proc(number).yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)      553 2022-06-27 10:17:56.000000 snowddl-0.9.9/snowddl/_config/sample02_01/test_db/test_schema/procedure/test2_proc(varchar).yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)      177 2022-06-27 10:07:58.000000 snowddl-0.9.9/snowddl/_config/sample02_01/test_db/test_schema/procedure/test3_proc().yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)      312 2022-06-27 10:47:45.000000 snowddl-0.9.9/snowddl/_config/sample02_01/test_db/test_schema/procedure/test4_proc().yaml
+drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-13 09:47:37.098929 snowddl-0.9.9/snowddl/_config/sample02_01/test_db/test_schema/row_access_policy/
+-rw-r--r--   0 vmarkov    (501) staff       (20)      152 2022-02-10 13:32:20.000000 snowddl-0.9.9/snowddl/_config/sample02_01/test_db/test_schema/row_access_policy/test_row_policy_1.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)      172 2022-02-10 13:34:07.000000 snowddl-0.9.9/snowddl/_config/sample02_01/test_db/test_schema/row_access_policy/test_row_policy_2.yaml
+drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-13 09:47:37.099303 snowddl-0.9.9/snowddl/_config/sample02_01/test_db/test_schema/stage/
+-rw-r--r--   0 vmarkov    (501) staff       (20)      109 2022-05-09 13:02:38.000000 snowddl-0.9.9/snowddl/_config/sample02_01/test_db/test_schema/stage/test_external_stage.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)      119 2022-02-22 12:18:39.000000 snowddl-0.9.9/snowddl/_config/sample02_01/test_db/test_schema/stage/test_internal_stage.yaml
+drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-13 09:47:37.099753 snowddl-0.9.9/snowddl/_config/sample02_01/test_db/test_schema/stream/
+-rw-r--r--   0 vmarkov    (501) staff       (20)       87 2022-02-10 12:03:54.000000 snowddl-0.9.9/snowddl/_config/sample02_01/test_db/test_schema/stream/test_stream_1.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)       76 2022-02-10 12:09:31.000000 snowddl-0.9.9/snowddl/_config/sample02_01/test_db/test_schema/stream/test_stream_2.yaml
+drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-13 09:47:37.100774 snowddl-0.9.9/snowddl/_config/sample02_01/test_db/test_schema/table/
+-rw-r--r--   0 vmarkov    (501) staff       (20)       95 2022-06-05 20:44:28.000000 snowddl-0.9.9/snowddl/_config/sample02_01/test_db/test_schema/table/test_table_1.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)       72 2022-02-10 11:53:23.000000 snowddl-0.9.9/snowddl/_config/sample02_01/test_db/test_schema/table/test_table_2.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)      189 2022-08-08 16:02:29.000000 snowddl-0.9.9/snowddl/_config/sample02_01/test_db/test_schema/table/test_table_3.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)      226 2022-08-08 16:17:12.000000 snowddl-0.9.9/snowddl/_config/sample02_01/test_db/test_schema/table/test_table_4.yaml
+drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-13 09:47:37.101388 snowddl-0.9.9/snowddl/_config/sample02_01/test_db/test_schema/task/
+-rw-r--r--   0 vmarkov    (501) staff       (20)       75 2022-02-10 13:09:38.000000 snowddl-0.9.9/snowddl/_config/sample02_01/test_db/test_schema/task/test_task_1.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)       80 2022-08-08 16:30:21.000000 snowddl-0.9.9/snowddl/_config/sample02_01/test_db/test_schema/task/test_task_2.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)       96 2022-08-08 16:30:21.000000 snowddl-0.9.9/snowddl/_config/sample02_01/test_db/test_schema/task/test_task_3.yaml
+-rw-r--r--   0 vmarkov    (501) staff       (20)      173 2022-02-22 12:18:39.000000 snowddl-0.9.9/snowddl/_config/sample02_01/warehouse.yaml
+drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-13 09:47:37.102448 snowddl-0.9.9/snowddl/app/
+-rw-r--r--   0 vmarkov    (501) staff       (20)       92 2022-06-05 17:29:09.000000 snowddl-0.9.9/snowddl/app/__init__.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)    15519 2022-08-23 09:44:54.000000 snowddl-0.9.9/snowddl/app/base.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)     5539 2022-08-23 14:53:35.000000 snowddl-0.9.9/snowddl/app/convert.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)     7744 2022-08-23 14:53:35.000000 snowddl-0.9.9/snowddl/app/singledb.py
+drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-13 09:47:37.105599 snowddl-0.9.9/snowddl/blueprint/
+-rw-r--r--   0 vmarkov    (501) staff       (20)     1749 2022-07-28 16:17:49.000000 snowddl-0.9.9/snowddl/blueprint/__init__.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)     8950 2022-08-08 16:27:12.000000 snowddl-0.9.9/snowddl/blueprint/blueprint.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)      703 2022-08-08 15:14:25.000000 snowddl-0.9.9/snowddl/blueprint/column.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)     2887 2022-10-04 08:35:33.000000 snowddl-0.9.9/snowddl/blueprint/data_type.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)      113 2022-02-10 16:03:51.000000 snowddl-0.9.9/snowddl/blueprint/edition.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)      353 2022-05-29 21:46:56.000000 snowddl-0.9.9/snowddl/blueprint/grant.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)     5604 2022-08-08 14:54:34.000000 snowddl-0.9.9/snowddl/blueprint/ident.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)     3253 2022-07-28 16:17:49.000000 snowddl-0.9.9/snowddl/blueprint/ident_builder.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)     5327 2022-07-28 13:20:21.000000 snowddl-0.9.9/snowddl/blueprint/object_type.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)      620 2022-05-29 22:22:13.000000 snowddl-0.9.9/snowddl/blueprint/reference.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)      313 2022-05-29 22:22:13.000000 snowddl-0.9.9/snowddl/blueprint/stage.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)     2935 2022-07-28 16:06:52.000000 snowddl-0.9.9/snowddl/config.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)     4027 2022-05-30 08:01:02.000000 snowddl-0.9.9/snowddl/context.py
+drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-13 09:47:37.107879 snowddl-0.9.9/snowddl/converter/
+-rw-r--r--   0 vmarkov    (501) staff       (20)      518 2022-10-05 14:51:29.000000 snowddl-0.9.9/snowddl/converter/__init__.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)      581 2022-02-21 10:26:09.000000 snowddl-0.9.9/snowddl/converter/_yaml.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)     3890 2022-08-13 16:43:51.000000 snowddl-0.9.9/snowddl/converter/abc_converter.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)      628 2022-05-30 12:51:04.000000 snowddl-0.9.9/snowddl/converter/abc_schema_object_converter.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)      858 2022-02-15 11:28:36.000000 snowddl-0.9.9/snowddl/converter/database.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)      884 2022-02-15 11:28:36.000000 snowddl-0.9.9/snowddl/converter/schema.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)     1654 2022-02-14 19:14:50.000000 snowddl-0.9.9/snowddl/converter/sequence.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)     6436 2022-10-11 15:05:29.000000 snowddl-0.9.9/snowddl/converter/table.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)     2887 2022-10-13 09:43:46.000000 snowddl-0.9.9/snowddl/converter/view.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)     3673 2022-08-19 18:36:34.000000 snowddl-0.9.9/snowddl/engine.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)      708 2022-01-20 18:29:46.000000 snowddl-0.9.9/snowddl/error.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)     5167 2022-08-19 18:36:34.000000 snowddl-0.9.9/snowddl/formatter.py
+drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-13 09:47:37.116006 snowddl-0.9.9/snowddl/parser/
+-rw-r--r--   0 vmarkov    (501) staff       (20)     2126 2022-07-27 15:52:54.000000 snowddl-0.9.9/snowddl/parser/__init__.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)     2366 2022-08-13 16:39:57.000000 snowddl-0.9.9/snowddl/parser/_parsed_file.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)     2290 2022-07-28 14:14:09.000000 snowddl-0.9.9/snowddl/parser/abc_parser.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)      774 2022-03-17 12:54:13.000000 snowddl-0.9.9/snowddl/parser/account_params.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)     4667 2022-07-28 14:23:01.000000 snowddl-0.9.9/snowddl/parser/business_role.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)     1197 2022-05-29 22:30:16.000000 snowddl-0.9.9/snowddl/parser/database.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)     3281 2022-07-26 19:08:25.000000 snowddl-0.9.9/snowddl/parser/external_function.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)     7538 2022-05-30 12:53:24.000000 snowddl-0.9.9/snowddl/parser/external_table.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)     1207 2022-05-30 12:51:04.000000 snowddl-0.9.9/snowddl/parser/file_format.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)     3939 2022-06-15 18:52:38.000000 snowddl-0.9.9/snowddl/parser/function.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)     1414 2022-07-26 18:21:20.000000 snowddl-0.9.9/snowddl/parser/inbound_share.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)     2638 2022-05-30 11:32:04.000000 snowddl-0.9.9/snowddl/parser/masking_policy.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)     1802 2022-05-29 22:48:19.000000 snowddl-0.9.9/snowddl/parser/materialized_view.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)     1452 2022-02-22 11:52:26.000000 snowddl-0.9.9/snowddl/parser/network_policy.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)     2996 2022-07-28 16:14:37.000000 snowddl-0.9.9/snowddl/parser/outbound_share.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)     2856 2022-05-30 11:32:04.000000 snowddl-0.9.9/snowddl/parser/pipe.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)     1393 2022-05-24 16:33:42.000000 snowddl-0.9.9/snowddl/parser/placeholder.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)     3902 2022-06-27 10:03:47.000000 snowddl-0.9.9/snowddl/parser/procedure.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)     1416 2022-02-22 13:46:12.000000 snowddl-0.9.9/snowddl/parser/resource_monitor.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)     2540 2022-05-30 11:32:05.000000 snowddl-0.9.9/snowddl/parser/row_access_policy.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)     3099 2022-05-30 11:32:04.000000 snowddl-0.9.9/snowddl/parser/schema.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)      950 2022-05-29 22:48:19.000000 snowddl-0.9.9/snowddl/parser/sequence.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)     3006 2022-05-30 11:32:04.000000 snowddl-0.9.9/snowddl/parser/stage.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)     1485 2022-05-30 11:32:04.000000 snowddl-0.9.9/snowddl/parser/stream.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)     8345 2022-08-08 15:14:25.000000 snowddl-0.9.9/snowddl/parser/table.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)     1985 2022-05-30 11:32:04.000000 snowddl-0.9.9/snowddl/parser/tag.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)     2466 2022-08-08 17:18:54.000000 snowddl-0.9.9/snowddl/parser/task.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)     2242 2022-07-28 16:17:49.000000 snowddl-0.9.9/snowddl/parser/tech_role.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)     4729 2022-05-30 12:51:04.000000 snowddl-0.9.9/snowddl/parser/user.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)     1795 2022-05-30 11:32:04.000000 snowddl-0.9.9/snowddl/parser/view.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)     1851 2022-05-29 22:48:49.000000 snowddl-0.9.9/snowddl/parser/warehouse.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)     1250 2022-08-19 18:40:50.000000 snowddl-0.9.9/snowddl/query_builder.py
+drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-13 09:47:37.125985 snowddl-0.9.9/snowddl/resolver/
+-rw-r--r--   0 vmarkov    (501) staff       (20)     3001 2022-07-27 18:00:28.000000 snowddl-0.9.9/snowddl/resolver/__init__.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)      963 2022-01-19 18:08:26.000000 snowddl-0.9.9/snowddl/resolver/_utils.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)     6870 2022-08-08 17:40:46.000000 snowddl-0.9.9/snowddl/resolver/abc_resolver.py
+-rw-rw-rw-   0 vmarkov    (501) staff       (20)     7876 2022-09-09 15:25:17.000000 snowddl-0.9.9/snowddl/resolver/abc_role_resolver.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)     1497 2022-06-05 20:46:57.000000 snowddl-0.9.9/snowddl/resolver/abc_schema_object_resolver.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)     1935 2022-02-01 17:00:20.000000 snowddl-0.9.9/snowddl/resolver/account_params.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)      355 2022-01-28 17:04:59.000000 snowddl-0.9.9/snowddl/resolver/business_role.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)     2937 2022-05-30 08:45:04.000000 snowddl-0.9.9/snowddl/resolver/database.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)     5079 2022-08-15 17:42:29.000000 snowddl-0.9.9/snowddl/resolver/external_function.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)     5484 2022-08-15 17:42:29.000000 snowddl-0.9.9/snowddl/resolver/external_table.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)     3431 2022-08-15 17:52:08.000000 snowddl-0.9.9/snowddl/resolver/file_format.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)     3825 2022-01-30 19:42:27.000000 snowddl-0.9.9/snowddl/resolver/foreign_key.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)     4926 2022-08-15 17:42:29.000000 snowddl-0.9.9/snowddl/resolver/function.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)     3275 2022-07-26 19:22:57.000000 snowddl-0.9.9/snowddl/resolver/inbound_share.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)     2070 2022-07-26 19:12:21.000000 snowddl-0.9.9/snowddl/resolver/inbound_share_role.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)     7690 2022-06-05 21:30:51.000000 snowddl-0.9.9/snowddl/resolver/masking_policy.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)     3331 2022-03-02 16:20:07.000000 snowddl-0.9.9/snowddl/resolver/materialized_view.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)     4022 2022-02-17 12:09:48.000000 snowddl-0.9.9/snowddl/resolver/network_policy.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)     5487 2022-07-28 16:24:43.000000 snowddl-0.9.9/snowddl/resolver/outbound_share.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)     5424 2022-05-09 13:02:38.000000 snowddl-0.9.9/snowddl/resolver/pipe.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)     2810 2022-05-30 12:36:19.000000 snowddl-0.9.9/snowddl/resolver/primary_key.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)     4708 2022-08-15 17:42:29.000000 snowddl-0.9.9/snowddl/resolver/procedure.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)     4330 2022-02-17 14:03:21.000000 snowddl-0.9.9/snowddl/resolver/resource_monitor.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)     8299 2022-06-05 21:30:51.000000 snowddl-0.9.9/snowddl/resolver/row_access_policy.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)     3681 2022-06-05 20:46:57.000000 snowddl-0.9.9/snowddl/resolver/schema.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)     6253 2022-05-30 11:42:58.000000 snowddl-0.9.9/snowddl/resolver/schema_role.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)     2750 2022-01-30 19:42:27.000000 snowddl-0.9.9/snowddl/resolver/sequence.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)     4586 2022-07-13 15:52:58.000000 snowddl-0.9.9/snowddl/resolver/stage.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)     4273 2022-08-13 16:44:33.000000 snowddl-0.9.9/snowddl/resolver/stage_file.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)     3835 2022-01-29 18:55:37.000000 snowddl-0.9.9/snowddl/resolver/stream.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)    14403 2022-08-08 16:15:19.000000 snowddl-0.9.9/snowddl/resolver/table.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)     6621 2022-05-30 08:52:44.000000 snowddl-0.9.9/snowddl/resolver/tag.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)     4525 2022-02-08 11:55:24.000000 snowddl-0.9.9/snowddl/resolver/task.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)      339 2022-01-28 17:04:59.000000 snowddl-0.9.9/snowddl/resolver/tech_role.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)     2421 2022-01-30 19:42:27.000000 snowddl-0.9.9/snowddl/resolver/unique_key.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)    10354 2022-08-29 20:53:13.000000 snowddl-0.9.9/snowddl/resolver/user.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)     1887 2022-09-09 15:33:30.000000 snowddl-0.9.9/snowddl/resolver/user_role.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)     4352 2022-05-30 09:05:07.000000 snowddl-0.9.9/snowddl/resolver/view.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)     5708 2022-05-02 14:08:40.000000 snowddl-0.9.9/snowddl/resolver/warehouse.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)     1955 2022-05-30 11:32:05.000000 snowddl-0.9.9/snowddl/resolver/warehouse_role.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)     2619 2022-06-05 21:00:18.000000 snowddl-0.9.9/snowddl/schema_cache.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)      920 2022-07-26 15:58:33.000000 snowddl-0.9.9/snowddl/settings.py
+-rw-r--r--   0 vmarkov    (501) staff       (20)       22 2022-10-13 09:46:55.000000 snowddl-0.9.9/snowddl/version.py
+drwxr-xr-x   0 vmarkov    (501) staff       (20)        0 2022-10-13 09:47:37.075088 snowddl-0.9.9/snowddl.egg-info/
+-rw-r--r--   0 vmarkov    (501) staff       (20)     1786 2022-10-13 09:47:36.000000 snowddl-0.9.9/snowddl.egg-info/PKG-INFO
+-rw-r--r--   0 vmarkov    (501) staff       (20)    12288 2022-10-13 09:47:36.000000 snowddl-0.9.9/snowddl.egg-info/SOURCES.txt
+-rw-r--r--   0 vmarkov    (501) staff       (20)        1 2022-10-13 09:47:36.000000 snowddl-0.9.9/snowddl.egg-info/dependency_links.txt
+-rw-r--r--   0 vmarkov    (501) staff       (20)      159 2022-10-13 09:47:36.000000 snowddl-0.9.9/snowddl.egg-info/entry_points.txt
+-rw-r--r--   0 vmarkov    (501) staff       (20)       60 2022-10-13 09:47:36.000000 snowddl-0.9.9/snowddl.egg-info/requires.txt
+-rw-r--r--   0 vmarkov    (501) staff       (20)        8 2022-10-13 09:47:36.000000 snowddl-0.9.9/snowddl.egg-info/top_level.txt
```

### Comparing `snowddl-0.9.8/LICENSE.txt` & `snowddl-0.9.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/PKG-INFO` & `snowddl-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snowddl
-Version: 0.9.8
+Version: 0.9.9
 Summary: Object management automation tool for Snowflake
 Home-page: https://github.com/littleK0i/snowddl
 Author: Vitaly Markov
 Author-email: wild.desu@gmail.com
 Keywords: snowflake database schema object change ddl sql create alter drop grant
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `snowddl-0.9.8/README.md` & `snowddl-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/setup.py` & `snowddl-0.9.9/setup.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/_config/sample01_01/business_role.yaml` & `snowddl-0.9.9/snowddl/_config/sample01_01/business_role.yaml`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/_config/sample01_01/snowddl_db/bookings/table/airports_data.yaml` & `snowddl-0.9.9/snowddl/_config/sample01_01/snowddl_db/bookings/table/airports_data.yaml`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/_config/sample01_01/snowddl_db/bookings/table/boarding_passes.yaml` & `snowddl-0.9.9/snowddl/_config/sample01_01/snowddl_db/bookings/table/boarding_passes.yaml`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/_config/sample01_01/snowddl_db/bookings/table/bookings.yaml` & `snowddl-0.9.9/snowddl/_config/sample01_01/snowddl_db/bookings/table/bookings.yaml`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/_config/sample01_01/snowddl_db/bookings/table/flights.yaml` & `snowddl-0.9.9/snowddl/_config/sample01_01/snowddl_db/bookings/table/flights.yaml`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/_config/sample01_01/snowddl_db/bookings/table/seats.yaml` & `snowddl-0.9.9/snowddl/_config/sample01_01/snowddl_db/bookings/table/seats.yaml`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/_config/sample01_01/snowddl_db/bookings/table/ticket_flights.yaml` & `snowddl-0.9.9/snowddl/_config/sample01_01/snowddl_db/bookings/table/ticket_flights.yaml`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/_config/sample01_01/snowddl_db/bookings/table/tickets.yaml` & `snowddl-0.9.9/snowddl/_config/sample01_01/snowddl_db/bookings/table/tickets.yaml`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/_config/sample01_01/snowddl_db/bookings/view/airports.yaml` & `snowddl-0.9.9/snowddl/_config/sample01_01/snowddl_db/bookings/view/airports.yaml`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/_config/sample01_01/snowddl_db/bookings/view/flights_v.yaml` & `snowddl-0.9.9/snowddl/_config/sample01_01/snowddl_db/bookings/view/flights_v.yaml`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/_config/sample01_01/snowddl_db/bookings/view/routes.yaml` & `snowddl-0.9.9/snowddl/_config/sample01_01/snowddl_db/bookings/view/routes.yaml`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/_config/sample01_01/snowddl_db/sakila/table/customer.yaml` & `snowddl-0.9.9/snowddl/_config/sample01_01/snowddl_db/sakila/table/customer.yaml`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/_config/sample01_01/snowddl_db/sakila/table/film.yaml` & `snowddl-0.9.9/snowddl/_config/sample01_01/snowddl_db/sakila/table/film.yaml`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/_config/sample01_01/snowddl_db/sakila/table/payment.yaml` & `snowddl-0.9.9/snowddl/_config/sample01_01/snowddl_db/sakila/table/payment.yaml`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/_config/sample01_01/snowddl_db/sakila/table/rental.yaml` & `snowddl-0.9.9/snowddl/_config/sample01_01/snowddl_db/sakila/table/rental.yaml`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/_config/sample01_01/snowddl_db/sakila/table/staff.yaml` & `snowddl-0.9.9/snowddl/_config/sample01_01/snowddl_db/sakila/table/staff.yaml`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/_config/sample01_01/snowddl_db/sakila/view/customer_list.yaml` & `snowddl-0.9.9/snowddl/_config/sample01_01/snowddl_db/sakila/view/customer_list.yaml`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/_config/sample01_01/snowddl_db/sakila/view/film_list.yaml` & `snowddl-0.9.9/snowddl/_config/sample01_01/snowddl_db/sakila/view/film_list.yaml`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/_config/sample01_01/snowddl_db/sakila/view/sales_by_store.yaml` & `snowddl-0.9.9/snowddl/_config/sample01_01/snowddl_db/sakila/view/sales_by_store.yaml`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/_config/sample01_01/tech_role.yaml` & `snowddl-0.9.9/snowddl/_config/sample01_01/tech_role.yaml`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/_config/sample01_01/user.yaml` & `snowddl-0.9.9/snowddl/_config/sample01_01/user.yaml`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/_config/sample01_02/business_role.yaml` & `snowddl-0.9.9/snowddl/_config/sample01_02/business_role.yaml`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/_config/sample01_02/snowddl_db/bookings/table/airports_data.yaml` & `snowddl-0.9.9/snowddl/_config/sample01_02/snowddl_db/bookings/table/airports_data.yaml`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/_config/sample01_02/snowddl_db/bookings/table/boarding_passes.yaml` & `snowddl-0.9.9/snowddl/_config/sample01_02/snowddl_db/bookings/table/boarding_passes.yaml`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/_config/sample01_02/snowddl_db/bookings/table/bookings.yaml` & `snowddl-0.9.9/snowddl/_config/sample01_02/snowddl_db/bookings/table/bookings.yaml`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/_config/sample01_02/snowddl_db/bookings/table/flights.yaml` & `snowddl-0.9.9/snowddl/_config/sample01_02/snowddl_db/bookings/table/flights.yaml`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/_config/sample01_02/snowddl_db/bookings/table/seats.yaml` & `snowddl-0.9.9/snowddl/_config/sample01_02/snowddl_db/bookings/table/seats.yaml`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/_config/sample01_02/snowddl_db/bookings/table/ticket_flights.yaml` & `snowddl-0.9.9/snowddl/_config/sample01_02/snowddl_db/bookings/table/ticket_flights.yaml`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/_config/sample01_02/snowddl_db/bookings/table/tickets.yaml` & `snowddl-0.9.9/snowddl/_config/sample01_02/snowddl_db/bookings/table/tickets.yaml`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/_config/sample01_02/snowddl_db/bookings/view/airports.yaml` & `snowddl-0.9.9/snowddl/_config/sample01_02/snowddl_db/bookings/view/airports.yaml`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/_config/sample01_02/snowddl_db/bookings/view/flights_v.yaml` & `snowddl-0.9.9/snowddl/_config/sample01_02/snowddl_db/bookings/view/flights_v.yaml`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/_config/sample01_02/snowddl_db/bookings/view/routes.yaml` & `snowddl-0.9.9/snowddl/_config/sample01_02/snowddl_db/bookings/view/routes.yaml`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/_config/sample01_02/snowddl_db/sakila/table/customer.yaml` & `snowddl-0.9.9/snowddl/_config/sample01_02/snowddl_db/sakila/table/customer.yaml`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/_config/sample01_02/snowddl_db/sakila/table/film.yaml` & `snowddl-0.9.9/snowddl/_config/sample01_02/snowddl_db/sakila/table/film.yaml`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/_config/sample01_02/snowddl_db/sakila/table/payment.yaml` & `snowddl-0.9.9/snowddl/_config/sample01_02/snowddl_db/sakila/table/payment.yaml`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/_config/sample01_02/snowddl_db/sakila/table/rental.yaml` & `snowddl-0.9.9/snowddl/_config/sample01_02/snowddl_db/sakila/table/rental.yaml`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/_config/sample01_02/snowddl_db/sakila/table/staff.yaml` & `snowddl-0.9.9/snowddl/_config/sample01_02/snowddl_db/sakila/table/staff.yaml`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/_config/sample01_02/snowddl_db/sakila/view/customer_list.yaml` & `snowddl-0.9.9/snowddl/_config/sample01_02/snowddl_db/sakila/view/customer_list.yaml`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/_config/sample01_02/snowddl_db/sakila/view/film_list.yaml` & `snowddl-0.9.9/snowddl/_config/sample01_02/snowddl_db/sakila/view/film_list.yaml`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/_config/sample01_02/snowddl_db/sakila/view/sales_by_store.yaml` & `snowddl-0.9.9/snowddl/_config/sample01_02/snowddl_db/sakila/view/sales_by_store.yaml`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/_config/sample01_02/tech_role.yaml` & `snowddl-0.9.9/snowddl/_config/sample01_02/tech_role.yaml`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/_config/sample01_02/user.yaml` & `snowddl-0.9.9/snowddl/_config/sample01_02/user.yaml`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/_config/sample02_01/test_db/test_schema/procedure/test2_proc(varchar).yaml` & `snowddl-0.9.9/snowddl/_config/sample02_01/test_db/test_schema/procedure/test2_proc(varchar).yaml`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/app/base.py` & `snowddl-0.9.9/snowddl/app/base.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/app/convert.py` & `snowddl-0.9.9/snowddl/app/convert.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/app/singledb.py` & `snowddl-0.9.9/snowddl/app/singledb.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/blueprint/__init__.py` & `snowddl-0.9.9/snowddl/blueprint/__init__.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/blueprint/blueprint.py` & `snowddl-0.9.9/snowddl/blueprint/blueprint.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/blueprint/column.py` & `snowddl-0.9.9/snowddl/blueprint/column.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/blueprint/data_type.py` & `snowddl-0.9.9/snowddl/blueprint/data_type.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/blueprint/ident.py` & `snowddl-0.9.9/snowddl/blueprint/ident.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/blueprint/ident_builder.py` & `snowddl-0.9.9/snowddl/blueprint/ident_builder.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/blueprint/object_type.py` & `snowddl-0.9.9/snowddl/blueprint/object_type.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/blueprint/reference.py` & `snowddl-0.9.9/snowddl/blueprint/reference.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/config.py` & `snowddl-0.9.9/snowddl/config.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/context.py` & `snowddl-0.9.9/snowddl/context.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/converter/__init__.py` & `snowddl-0.9.9/snowddl/converter/__init__.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/converter/_yaml.py` & `snowddl-0.9.9/snowddl/converter/_yaml.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/converter/abc_converter.py` & `snowddl-0.9.9/snowddl/converter/abc_converter.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/converter/abc_schema_object_converter.py` & `snowddl-0.9.9/snowddl/converter/abc_schema_object_converter.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/converter/database.py` & `snowddl-0.9.9/snowddl/converter/database.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/converter/schema.py` & `snowddl-0.9.9/snowddl/converter/schema.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/converter/sequence.py` & `snowddl-0.9.9/snowddl/converter/sequence.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/converter/table.py` & `snowddl-0.9.9/snowddl/converter/table.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/converter/view.py` & `snowddl-0.9.9/snowddl/converter/view.py`

 * *Files 9% similar despite different names*

```diff
@@ -68,9 +68,14 @@
     def _get_text(self, row):
         # TODO: replace with better implementation when available
         cur = self.engine.execute_meta("SELECT GET_DDL('VIEW', {ident}) AS view_ddl", {
             "ident": f"{row['database']}.{row['schema']}.{row['name']}"
         })
 
         view_ddl = cur.fetchone()['VIEW_DDL']
+        view_text = view_text_re.sub(r'\1', view_ddl).strip(' \n\r\t()')
 
-        return view_text_re.sub(r'\1', view_ddl).strip(' \n\r\t')
+        # Remove trailing spaces from each line to prevent output formatting issues
+        # https://github.com/yaml/pyyaml/issues/411
+        view_text = '\n'.join(l.rstrip(' ') for l in view_text.split('\n'))
+
+        return view_text
```

### Comparing `snowddl-0.9.8/snowddl/engine.py` & `snowddl-0.9.9/snowddl/engine.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/error.py` & `snowddl-0.9.9/snowddl/error.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/formatter.py` & `snowddl-0.9.9/snowddl/formatter.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/parser/__init__.py` & `snowddl-0.9.9/snowddl/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/parser/_parsed_file.py` & `snowddl-0.9.9/snowddl/parser/_parsed_file.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/parser/abc_parser.py` & `snowddl-0.9.9/snowddl/parser/abc_parser.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/parser/account_params.py` & `snowddl-0.9.9/snowddl/parser/account_params.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/parser/business_role.py` & `snowddl-0.9.9/snowddl/parser/business_role.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/parser/database.py` & `snowddl-0.9.9/snowddl/parser/database.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/parser/external_function.py` & `snowddl-0.9.9/snowddl/parser/external_function.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/parser/external_table.py` & `snowddl-0.9.9/snowddl/parser/external_table.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/parser/file_format.py` & `snowddl-0.9.9/snowddl/parser/file_format.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/parser/function.py` & `snowddl-0.9.9/snowddl/parser/function.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/parser/inbound_share.py` & `snowddl-0.9.9/snowddl/parser/inbound_share.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/parser/masking_policy.py` & `snowddl-0.9.9/snowddl/parser/masking_policy.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/parser/materialized_view.py` & `snowddl-0.9.9/snowddl/parser/materialized_view.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/parser/network_policy.py` & `snowddl-0.9.9/snowddl/parser/network_policy.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/parser/outbound_share.py` & `snowddl-0.9.9/snowddl/parser/outbound_share.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/parser/pipe.py` & `snowddl-0.9.9/snowddl/parser/pipe.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/parser/placeholder.py` & `snowddl-0.9.9/snowddl/parser/placeholder.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/parser/procedure.py` & `snowddl-0.9.9/snowddl/parser/procedure.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/parser/resource_monitor.py` & `snowddl-0.9.9/snowddl/parser/resource_monitor.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/parser/row_access_policy.py` & `snowddl-0.9.9/snowddl/parser/row_access_policy.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/parser/schema.py` & `snowddl-0.9.9/snowddl/parser/schema.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/parser/sequence.py` & `snowddl-0.9.9/snowddl/parser/sequence.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/parser/stage.py` & `snowddl-0.9.9/snowddl/parser/stage.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/parser/stream.py` & `snowddl-0.9.9/snowddl/parser/stream.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/parser/table.py` & `snowddl-0.9.9/snowddl/parser/table.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/parser/tag.py` & `snowddl-0.9.9/snowddl/parser/tag.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/parser/task.py` & `snowddl-0.9.9/snowddl/parser/task.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/parser/tech_role.py` & `snowddl-0.9.9/snowddl/parser/tech_role.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/parser/user.py` & `snowddl-0.9.9/snowddl/parser/user.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/parser/view.py` & `snowddl-0.9.9/snowddl/parser/view.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/parser/warehouse.py` & `snowddl-0.9.9/snowddl/parser/warehouse.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/query_builder.py` & `snowddl-0.9.9/snowddl/query_builder.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/resolver/__init__.py` & `snowddl-0.9.9/snowddl/resolver/__init__.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/resolver/_utils.py` & `snowddl-0.9.9/snowddl/resolver/_utils.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/resolver/abc_resolver.py` & `snowddl-0.9.9/snowddl/resolver/abc_resolver.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/resolver/abc_role_resolver.py` & `snowddl-0.9.9/snowddl/resolver/abc_role_resolver.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/resolver/abc_schema_object_resolver.py` & `snowddl-0.9.9/snowddl/resolver/abc_schema_object_resolver.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/resolver/account_params.py` & `snowddl-0.9.9/snowddl/resolver/account_params.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/resolver/database.py` & `snowddl-0.9.9/snowddl/resolver/database.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/resolver/external_function.py` & `snowddl-0.9.9/snowddl/resolver/external_function.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/resolver/external_table.py` & `snowddl-0.9.9/snowddl/resolver/external_table.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/resolver/file_format.py` & `snowddl-0.9.9/snowddl/resolver/file_format.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/resolver/foreign_key.py` & `snowddl-0.9.9/snowddl/resolver/foreign_key.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/resolver/function.py` & `snowddl-0.9.9/snowddl/resolver/function.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/resolver/inbound_share.py` & `snowddl-0.9.9/snowddl/resolver/inbound_share.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/resolver/inbound_share_role.py` & `snowddl-0.9.9/snowddl/resolver/inbound_share_role.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/resolver/masking_policy.py` & `snowddl-0.9.9/snowddl/resolver/masking_policy.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/resolver/materialized_view.py` & `snowddl-0.9.9/snowddl/resolver/materialized_view.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/resolver/network_policy.py` & `snowddl-0.9.9/snowddl/resolver/network_policy.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/resolver/outbound_share.py` & `snowddl-0.9.9/snowddl/resolver/outbound_share.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/resolver/pipe.py` & `snowddl-0.9.9/snowddl/resolver/pipe.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/resolver/primary_key.py` & `snowddl-0.9.9/snowddl/resolver/primary_key.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/resolver/procedure.py` & `snowddl-0.9.9/snowddl/resolver/procedure.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/resolver/resource_monitor.py` & `snowddl-0.9.9/snowddl/resolver/resource_monitor.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/resolver/row_access_policy.py` & `snowddl-0.9.9/snowddl/resolver/row_access_policy.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/resolver/schema.py` & `snowddl-0.9.9/snowddl/resolver/schema.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/resolver/schema_role.py` & `snowddl-0.9.9/snowddl/resolver/schema_role.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/resolver/sequence.py` & `snowddl-0.9.9/snowddl/resolver/sequence.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/resolver/stage.py` & `snowddl-0.9.9/snowddl/resolver/stage.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/resolver/stage_file.py` & `snowddl-0.9.9/snowddl/resolver/stage_file.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/resolver/stream.py` & `snowddl-0.9.9/snowddl/resolver/stream.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/resolver/table.py` & `snowddl-0.9.9/snowddl/resolver/table.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/resolver/tag.py` & `snowddl-0.9.9/snowddl/resolver/tag.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/resolver/task.py` & `snowddl-0.9.9/snowddl/resolver/task.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/resolver/unique_key.py` & `snowddl-0.9.9/snowddl/resolver/unique_key.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/resolver/user.py` & `snowddl-0.9.9/snowddl/resolver/user.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/resolver/user_role.py` & `snowddl-0.9.9/snowddl/resolver/user_role.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/resolver/view.py` & `snowddl-0.9.9/snowddl/resolver/view.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/resolver/warehouse.py` & `snowddl-0.9.9/snowddl/resolver/warehouse.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/resolver/warehouse_role.py` & `snowddl-0.9.9/snowddl/resolver/warehouse_role.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/schema_cache.py` & `snowddl-0.9.9/snowddl/schema_cache.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl/settings.py` & `snowddl-0.9.9/snowddl/settings.py`

 * *Files identical despite different names*

### Comparing `snowddl-0.9.8/snowddl.egg-info/PKG-INFO` & `snowddl-0.9.9/snowddl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snowddl
-Version: 0.9.8
+Version: 0.9.9
 Summary: Object management automation tool for Snowflake
 Home-page: https://github.com/littleK0i/snowddl
 Author: Vitaly Markov
 Author-email: wild.desu@gmail.com
 Keywords: snowflake database schema object change ddl sql create alter drop grant
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `snowddl-0.9.8/snowddl.egg-info/SOURCES.txt` & `snowddl-0.9.9/snowddl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

