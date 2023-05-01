# Comparing `tmp/trytond_stock-6.6.3.tar.gz` & `tmp/trytond_stock-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_stock-6.6.3.tar", last modified: Sat Apr  1 22:10:03 2023, max compression
+gzip compressed data, was "trytond_stock-6.8.0.tar", last modified: Mon May  1 11:53:16 2023, max compression
```

## Comparing `trytond_stock-6.6.3.tar` & `trytond_stock-6.8.0.tar`

### file list

```diff
@@ -1,194 +1,194 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-04-01 22:10:03.509330 trytond_stock-6.6.3/
--rw-r--r--   0 ced       (1000) ced       (1000)    10309 2023-04-01 22:09:58.000000 trytond_stock-6.6.3/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      826 2023-04-01 22:09:58.000000 trytond_stock-6.6.3/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2643 2023-04-01 22:10:03.509330 trytond_stock-6.6.3/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      445 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2614 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     9530 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/configuration.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2011 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/configuration.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    46101 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/customer_return_restocking_list.fodt
--rw-r--r--   0 ced       (1000) ced       (1000)    48755 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/delivery_note.fodt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-04-01 22:10:03.492663 trytond_stock-6.6.3/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2082 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/doc/conf.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-04-01 22:10:03.499330 trytond_stock-6.6.3/doc/design/
--rw-r--r--   0 ced       (1000) ced       (1000)      635 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/doc/design/configuration.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      199 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/doc/design/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1535 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/doc/design/inventory.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2218 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/doc/design/location.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2037 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/doc/design/move.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     1102 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/doc/design/period.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3305 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/doc/design/product.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     7779 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/doc/design/shipment.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      445 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      288 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/doc/reference.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       90 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/doc/releases.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2431 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/doc/setup.rst
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-04-01 22:10:03.499330 trytond_stock-6.6.3/doc/usage/
--rw-r--r--   0 ced       (1000) ced       (1000)      243 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/doc/usage/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      567 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/doc/usage/period.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4193 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/doc/usage/quantity.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4669 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/doc/usage/shipment.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2344 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/doc/usage/value.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      825 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/exceptions.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-04-01 22:10:03.499330 trytond_stock-6.6.3/icons/
--rw-r--r--   0 ced       (1000) ced       (1000)    11357 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/icons/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      416 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/icons/tryton-shipment-in.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      426 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/icons/tryton-shipment-out.svg
--rw-r--r--   0 ced       (1000) ced       (1000)      241 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/icons/tryton-stock.svg
--rw-r--r--   0 ced       (1000) ced       (1000)    49545 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/internal_shipment.fodt
--rw-r--r--   0 ced       (1000) ced       (1000)    23478 2023-03-12 09:26:19.000000 trytond_stock-6.6.3/inventory.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8965 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/inventory.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1025 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/ir.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-04-01 22:10:03.432663 trytond_stock-6.6.3/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)    91409 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)    96063 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)    82156 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)    98043 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)    96958 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)    81052 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)    89854 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)   102088 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)    82130 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)    97445 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    92393 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)    80321 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)    84327 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)    89189 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)    86477 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    96350 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    85105 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    87027 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)    92647 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)    91532 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)    85855 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)    82049 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)    77247 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)    90483 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)    28144 2022-12-19 12:03:07.000000 trytond_stock-6.6.3/location.py
--rw-r--r--   0 ced       (1000) ced       (1000)    10457 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/location.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     7746 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    67189 2023-01-02 20:25:44.000000 trytond_stock-6.6.3/move.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8526 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/move.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     6302 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/party.py
--rw-r--r--   0 ced       (1000) ced       (1000)     4507 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/party.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     6992 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/period.py
--rw-r--r--   0 ced       (1000) ced       (1000)     6018 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/period.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    45878 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/picking_list.fodt
--rw-r--r--   0 ced       (1000) ced       (1000)    49427 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)    22458 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1810 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/res.py
--rw-r--r--   0 ced       (1000) ced       (1000)      715 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/res.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-04-01 22:10:03.509330 trytond_stock-6.6.3/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4545 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)   110554 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/shipment.py
--rw-r--r--   0 ced       (1000) ced       (1000)    53918 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/shipment.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2918 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/stock.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    23276 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/stock_reporting_margin.py
--rw-r--r--   0 ced       (1000) ced       (1000)    32870 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/stock_reporting_margin.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    45405 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/supplier_restocking_list.fodt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-04-01 22:10:03.449330 trytond_stock-6.6.3/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     8364 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/tests/scenario_stock_average_cost_price.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     7588 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/tests/scenario_stock_inventory.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3541 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/tests/scenario_stock_inventory_count.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2731 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/tests/scenario_stock_inventory_empty_quantity.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2052 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/tests/scenario_stock_move_in_future.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3899 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/tests/scenario_stock_product_quantities_by_warehouse.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     5255 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/tests/scenario_stock_recompute_average_cost_price.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3123 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/tests/scenario_stock_recompute_average_cost_price_production.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     5152 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/tests/scenario_stock_reporting.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     7823 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/tests/scenario_stock_reporting_margin.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2433 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/tests/scenario_stock_shipment_in_return.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2441 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/tests/scenario_stock_shipment_in_same_storage_input.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     4588 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/tests/scenario_stock_shipment_internal.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     3350 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/tests/scenario_stock_shipment_internal_transit.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     8720 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/tests/scenario_stock_shipment_out.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2487 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/tests/scenario_stock_shipment_out_return_same_storage_input.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     2528 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/tests/scenario_stock_shipment_out_same_storage_output.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    69197 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      296 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/tests/test_scenario.py
--rw-r--r--   0 ced       (1000) ced       (1000)      518 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      304 2023-01-02 22:23:20.000000 trytond_stock-6.6.3/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-04-01 22:10:03.505997 trytond_stock-6.6.3/trytond_stock.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2643 2023-04-01 22:10:02.000000 trytond_stock-6.6.3/trytond_stock.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     9605 2023-04-01 22:10:03.000000 trytond_stock-6.6.3/trytond_stock.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-04-01 22:10:02.000000 trytond_stock-6.6.3/trytond_stock.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       48 2023-04-01 22:10:02.000000 trytond_stock-6.6.3/trytond_stock.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-01-02 22:23:09.000000 trytond_stock-6.6.3/trytond_stock.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      196 2023-04-01 22:10:02.000000 trytond_stock-6.6.3/trytond_stock.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-04-01 22:10:02.000000 trytond_stock-6.6.3/trytond_stock.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-04-01 22:10:03.492663 trytond_stock-6.6.3/view/
--rw-r--r--   0 ced       (1000) ced       (1000)     1128 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/view/configuration_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      456 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/view/inventory_count_quantity_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      248 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/view/inventory_count_search_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      892 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/view/inventory_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      538 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/view/inventory_line_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      331 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/view/inventory_line_list_simple.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      457 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/view/inventory_line_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      367 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/view/inventory_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1135 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/view/location_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      448 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/view/location_lead_time_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      339 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/view/location_lead_time_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      298 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/view/location_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      614 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/view/location_quantity_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      364 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/view/location_quantity_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      315 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/view/location_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1621 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/view/move_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      421 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/view/move_list_shipment.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      421 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/view/move_list_shipment_in.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      657 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/view/move_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      267 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/view/move_tree_simple.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      373 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/view/party_address_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      314 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/view/party_address_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      372 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/view/party_contact_mechanism_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      304 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/view/party_contact_mechanism_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      903 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/view/party_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      450 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/view/period_cache_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      308 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/view/period_cache_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      502 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/view/period_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      289 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/view/period_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      315 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/view/product_by_location_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      500 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/view/product_cost_price_revision_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      360 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/view/product_cost_price_revision_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      306 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/view/product_modify_cost_price_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      328 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/view/product_quantities_warehouse_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      360 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/view/product_quantities_warehouse_graph.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      307 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/view/product_quantities_warehouse_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      505 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/view/product_quantities_warehouse_move_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      315 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/view/products_by_locations_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      432 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/view/products_by_locations_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      238 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/view/recompute_cost_price_start_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      292 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/view/reporting_margin_category_graph_amount.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      292 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/view/reporting_margin_category_graph_margin.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      292 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/view/reporting_margin_category_graph_profit.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      512 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/view/reporting_margin_category_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      414 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/view/reporting_margin_category_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      644 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/view/reporting_margin_context_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      310 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/view/reporting_margin_main_graph_amount.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      302 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/view/reporting_margin_main_graph_margin.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      280 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/view/reporting_margin_main_graph_profit.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      447 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/view/reporting_margin_main_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      312 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/view/reporting_margin_main_time_series_graph_amount.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      304 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/view/reporting_margin_main_time_series_graph_margin.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      282 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/view/reporting_margin_main_time_series_graph_profit.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      411 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/view/reporting_margin_main_time_series_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      291 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/view/reporting_margin_product_graph_amount.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      291 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/view/reporting_margin_product_graph_margin.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      291 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/view/reporting_margin_product_graph_profit.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      348 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/view/reporting_margin_product_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      305 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/view/reporting_margin_product_time_series_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      399 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/view/shipment_assign_partial_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1600 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/view/shipment_in_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1469 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/view/shipment_in_return_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      611 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/view/shipment_in_return_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      606 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/view/shipment_in_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1951 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/view/shipment_internal_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      590 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/view/shipment_internal_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1768 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/view/shipment_out_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1582 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/view/shipment_out_return_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      606 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/view/shipment_out_return_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      607 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/view/shipment_out_tree.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      359 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/view/user_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      398 2022-12-19 12:02:58.000000 trytond_stock-6.6.3/view/user_form_preferences.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:53:16.061099 trytond_stock-6.8.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)    10347 2023-05-01 11:08:59.000000 trytond_stock-6.8.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      826 2023-05-01 11:08:59.000000 trytond_stock-6.8.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-01-16 14:00:21.000000 trytond_stock-6.8.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2645 2023-05-01 11:53:16.057765 trytond_stock-6.8.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      445 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2614 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     9561 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/configuration.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2011 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/configuration.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    46098 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/customer_return_restocking_list.fodt
+-rw-r--r--   0 ced       (1000) ced       (1000)    48755 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/delivery_note.fodt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:53:16.047765 trytond_stock-6.8.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2221 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/doc/conf.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:53:16.051099 trytond_stock-6.8.0/doc/design/
+-rw-r--r--   0 ced       (1000) ced       (1000)      635 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/doc/design/configuration.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      199 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/doc/design/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1535 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/doc/design/inventory.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2218 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/doc/design/location.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2037 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/doc/design/move.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1102 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/doc/design/period.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3305 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/doc/design/product.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     7779 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/doc/design/shipment.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      445 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      288 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/doc/reference.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       90 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/doc/releases.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2311 2023-04-21 08:36:08.000000 trytond_stock-6.8.0/doc/setup.rst
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:53:16.054432 trytond_stock-6.8.0/doc/usage/
+-rw-r--r--   0 ced       (1000) ced       (1000)      243 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/doc/usage/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      567 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/doc/usage/period.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4193 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/doc/usage/quantity.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4669 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/doc/usage/shipment.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2344 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/doc/usage/value.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      825 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/exceptions.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:53:16.054432 trytond_stock-6.8.0/icons/
+-rw-r--r--   0 ced       (1000) ced       (1000)    11357 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/icons/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      416 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/icons/tryton-shipment-in.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      426 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/icons/tryton-shipment-out.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)      241 2023-01-16 14:00:21.000000 trytond_stock-6.8.0/icons/tryton-stock.svg
+-rw-r--r--   0 ced       (1000) ced       (1000)    49542 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/internal_shipment.fodt
+-rw-r--r--   0 ced       (1000) ced       (1000)    23444 2023-04-21 08:36:08.000000 trytond_stock-6.8.0/inventory.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8965 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/inventory.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1025 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/ir.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:53:16.024432 trytond_stock-6.8.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)    91409 2023-04-29 08:02:46.000000 trytond_stock-6.8.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    96063 2023-04-29 08:02:46.000000 trytond_stock-6.8.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    82156 2023-04-29 08:02:46.000000 trytond_stock-6.8.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    98088 2023-04-30 10:46:36.000000 trytond_stock-6.8.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    96959 2023-04-30 10:46:36.000000 trytond_stock-6.8.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    81052 2023-04-29 08:02:46.000000 trytond_stock-6.8.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    89803 2023-04-30 10:46:36.000000 trytond_stock-6.8.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)   102088 2023-04-29 08:02:46.000000 trytond_stock-6.8.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    82130 2023-04-29 08:02:46.000000 trytond_stock-6.8.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    97445 2023-04-29 08:02:46.000000 trytond_stock-6.8.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    92393 2023-04-29 08:02:46.000000 trytond_stock-6.8.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    80321 2023-04-29 08:02:46.000000 trytond_stock-6.8.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    84327 2023-04-29 08:02:46.000000 trytond_stock-6.8.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    89189 2023-04-29 08:02:46.000000 trytond_stock-6.8.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    86477 2023-04-29 08:02:46.000000 trytond_stock-6.8.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    96348 2023-04-30 10:46:36.000000 trytond_stock-6.8.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    85105 2023-04-29 08:02:46.000000 trytond_stock-6.8.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    87027 2023-04-29 08:02:46.000000 trytond_stock-6.8.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    93899 2023-04-30 10:46:36.000000 trytond_stock-6.8.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    91532 2023-04-29 08:02:46.000000 trytond_stock-6.8.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    85855 2023-04-29 08:02:46.000000 trytond_stock-6.8.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    82049 2023-04-29 08:02:46.000000 trytond_stock-6.8.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    77247 2023-04-29 08:02:46.000000 trytond_stock-6.8.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    90483 2023-04-29 08:02:46.000000 trytond_stock-6.8.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)    28636 2023-04-30 10:46:36.000000 trytond_stock-6.8.0/location.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    10457 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/location.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     7746 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    68212 2023-04-21 08:36:08.000000 trytond_stock-6.8.0/move.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8526 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/move.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     6302 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/party.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     4507 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/party.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     6992 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/period.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     6018 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/period.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    45875 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/picking_list.fodt
+-rw-r--r--   0 ced       (1000) ced       (1000)    49968 2023-04-28 07:46:16.000000 trytond_stock-6.8.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    22458 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1810 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/res.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      715 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/res.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-05-01 11:53:16.061099 trytond_stock-6.8.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4519 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)   115590 2023-04-21 08:36:08.000000 trytond_stock-6.8.0/shipment.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    53918 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/shipment.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2918 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/stock.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    23733 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/stock_reporting_margin.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    32870 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/stock_reporting_margin.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    45402 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/supplier_restocking_list.fodt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:53:16.034432 trytond_stock-6.8.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     8304 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/tests/scenario_stock_average_cost_price.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     7532 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/tests/scenario_stock_inventory.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3365 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/tests/scenario_stock_inventory_count.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2675 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/tests/scenario_stock_inventory_empty_quantity.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     1995 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/tests/scenario_stock_move_in_future.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3841 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/tests/scenario_stock_product_quantities_by_warehouse.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     5199 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/tests/scenario_stock_recompute_average_cost_price.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3123 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/tests/scenario_stock_recompute_average_cost_price_production.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     5077 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/tests/scenario_stock_reporting.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     7934 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/tests/scenario_stock_reporting_margin.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2376 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/tests/scenario_stock_shipment_in_return.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2441 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/tests/scenario_stock_shipment_in_same_storage_input.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     4539 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/tests/scenario_stock_shipment_internal.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     3350 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/tests/scenario_stock_shipment_internal_transit.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     8630 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/tests/scenario_stock_shipment_out.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2487 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/tests/scenario_stock_shipment_out_return_same_storage_input.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     2528 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/tests/scenario_stock_shipment_out_same_storage_output.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    69197 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      296 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/tests/test_scenario.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      562 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      304 2023-05-01 11:08:53.000000 trytond_stock-6.8.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:53:16.057765 trytond_stock-6.8.0/trytond_stock.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2645 2023-05-01 11:53:15.000000 trytond_stock-6.8.0/trytond_stock.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     9605 2023-05-01 11:53:15.000000 trytond_stock-6.8.0/trytond_stock.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-05-01 11:53:15.000000 trytond_stock-6.8.0/trytond_stock.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       48 2023-05-01 11:53:15.000000 trytond_stock-6.8.0/trytond_stock.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:02.000000 trytond_stock-6.8.0/trytond_stock.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      196 2023-05-01 11:53:15.000000 trytond_stock-6.8.0/trytond_stock.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-05-01 11:53:15.000000 trytond_stock-6.8.0/trytond_stock.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-05-01 11:53:16.044432 trytond_stock-6.8.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1128 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/view/configuration_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      456 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/view/inventory_count_quantity_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      248 2023-01-16 14:00:21.000000 trytond_stock-6.8.0/view/inventory_count_search_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      892 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/view/inventory_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      538 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/view/inventory_line_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      331 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/view/inventory_line_list_simple.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      457 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/view/inventory_line_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      367 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/view/inventory_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1135 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/view/location_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      448 2023-01-16 14:00:21.000000 trytond_stock-6.8.0/view/location_lead_time_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      339 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/view/location_lead_time_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      298 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/view/location_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      614 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/view/location_quantity_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      364 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/view/location_quantity_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      315 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/view/location_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1621 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/view/move_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      421 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/view/move_list_shipment.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      467 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/view/move_list_shipment_in.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      657 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/view/move_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      267 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/view/move_tree_simple.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      373 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/view/party_address_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      314 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/view/party_address_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      372 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/view/party_contact_mechanism_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      304 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/view/party_contact_mechanism_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      903 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/view/party_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      450 2023-01-16 14:00:21.000000 trytond_stock-6.8.0/view/period_cache_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      308 2023-01-16 14:00:21.000000 trytond_stock-6.8.0/view/period_cache_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      502 2023-01-16 14:00:21.000000 trytond_stock-6.8.0/view/period_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      289 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/view/period_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      315 2023-01-16 14:00:21.000000 trytond_stock-6.8.0/view/product_by_location_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      500 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/view/product_cost_price_revision_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      360 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/view/product_cost_price_revision_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      306 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/view/product_modify_cost_price_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      328 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/view/product_quantities_warehouse_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      360 2023-01-16 14:00:21.000000 trytond_stock-6.8.0/view/product_quantities_warehouse_graph.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      307 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/view/product_quantities_warehouse_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      505 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/view/product_quantities_warehouse_move_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      315 2023-01-16 14:00:21.000000 trytond_stock-6.8.0/view/products_by_locations_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      432 2023-04-28 07:46:16.000000 trytond_stock-6.8.0/view/products_by_locations_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      238 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/view/recompute_cost_price_start_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      292 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/view/reporting_margin_category_graph_amount.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      292 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/view/reporting_margin_category_graph_margin.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      292 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/view/reporting_margin_category_graph_profit.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      512 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/view/reporting_margin_category_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      414 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/view/reporting_margin_category_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      644 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/view/reporting_margin_context_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      310 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/view/reporting_margin_main_graph_amount.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      302 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/view/reporting_margin_main_graph_margin.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      280 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/view/reporting_margin_main_graph_profit.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      447 2023-04-28 07:46:16.000000 trytond_stock-6.8.0/view/reporting_margin_main_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      312 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/view/reporting_margin_main_time_series_graph_amount.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      304 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/view/reporting_margin_main_time_series_graph_margin.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      282 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/view/reporting_margin_main_time_series_graph_profit.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      411 2023-04-28 07:46:16.000000 trytond_stock-6.8.0/view/reporting_margin_main_time_series_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      291 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/view/reporting_margin_product_graph_amount.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      291 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/view/reporting_margin_product_graph_margin.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      291 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/view/reporting_margin_product_graph_profit.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      348 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/view/reporting_margin_product_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      305 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/view/reporting_margin_product_time_series_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      399 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/view/shipment_assign_partial_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1781 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/view/shipment_in_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1469 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/view/shipment_in_return_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      611 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/view/shipment_in_return_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      606 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/view/shipment_in_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1951 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/view/shipment_internal_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      590 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/view/shipment_internal_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1951 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/view/shipment_out_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     1763 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/view/shipment_out_return_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      606 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/view/shipment_out_return_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      607 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/view/shipment_out_tree.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      359 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/view/user_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      398 2023-04-15 07:12:15.000000 trytond_stock-6.8.0/view/user_form_preferences.xml
```

### Comparing `trytond_stock-6.6.3/CHANGELOG` & `trytond_stock-6.8.0/CHANGELOG`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 
-Version 6.6.3 - 2023-04-01
---------------------------
-* Bug fixes (see mercurial logs for details)
-
-Version 6.6.2 - 2023-01-02
---------------------------
-* Bug fixes (see mercurial logs for details)
-
-Version 6.6.1 - 2022-11-17
+Version 6.8.0 - 2023-05-01
 --------------------------
 * Bug fixes (see mercurial logs for details)
+* Add stock invert context to compute quantity
+* Remove support for Python 3.7
+* Add support for Python 3.11
+* Allow searching reporting records by name
+* Assign all possible shipments when trying
+* Store warehouse locations on shipments
 
 Version 6.6.0 - 2022-10-31
 --------------------------
 * Bug fixes (see mercurial logs for details)
 * Limit transit only between different warehouses
 * Remove default currency on move
 * Allow cancelling move done
```

### Comparing `trytond_stock-6.6.3/COPYRIGHT` & `trytond_stock-6.8.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.6.3/LICENSE` & `trytond_stock-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.6.3/PKG-INFO` & `trytond_stock-6.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond_stock
-Version: 6.6.3
+Version: 6.8.0
 Summary: Tryton module for stock and inventory
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/projects/modules-stock/
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/stock
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton stock
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
@@ -39,21 +39,21 @@
 Classifier: Natural Language :: Russian
 Classifier: Natural Language :: Slovenian
 Classifier: Natural Language :: Spanish
 Classifier: Natural Language :: Turkish
 Classifier: Natural Language :: Ukrainian
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: sparklines
 Provides-Extra: test
 License-File: LICENSE
 
 ############
 Stock Module
 ############
```

### Comparing `trytond_stock-6.6.3/__init__.py` & `trytond_stock-6.8.0/__init__.py`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.6.3/configuration.py` & `trytond_stock-6.8.0/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 sequences = ['shipment_in_sequence', 'shipment_in_return_sequence',
     'shipment_out_sequence', 'shipment_out_return_sequence',
     'shipment_internal_sequence', 'inventory_sequence']
 shipment_internal_transit = fields.Many2One(
     'stock.location', "Internal Shipment Transit", required=True,
     domain=[
         ('type', '=', 'storage'),
+        ('parent', '=', None),
         ],
     help="The default location used for stock that is in transit between "
     "warehouses.")
 
 
 def default_func(field_name):
     @classmethod
```

### Comparing `trytond_stock-6.6.3/configuration.xml` & `trytond_stock-6.8.0/configuration.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.6.3/customer_return_restocking_list.fodt` & `trytond_stock-6.8.0/customer_return_restocking_list.fodt`

 * *Files 0% similar despite different names*

#### Comparing `trytond_stock-6.6.3/customer_return_restocking_list.fodt` & `trytond_stock-6.8.0/customer_return_restocking_list.fodt`

```diff
@@ -522,15 +522,15 @@
               <text:p text:style-name="P9">Quantity</text:p>
             </table:table-cell>
           </table:table-row>
         </table:table-header-rows>
         <table:table-row>
           <table:table-cell table:style-name="Table1.A4" table:number-columns-spanned="2" office:value-type="string">
             <text:p text:style-name="P10">
-              <text:placeholder text:placeholder-type="text">&lt;for each=&quot;move in moves[shipment.id]&quot;&gt;</text:placeholder>
+              <text:placeholder text:placeholder-type="text">&lt;for each=&quot;move in moves(shipment)&quot;&gt;</text:placeholder>
             </text:p>
           </table:table-cell>
           <table:covered-table-cell/>
           <table:table-cell table:style-name="Table1.C4" office:value-type="string">
             <text:p text:style-name="P10"/>
           </table:table-cell>
           <table:table-cell table:style-name="Table1.D4" office:value-type="string">
```

### Comparing `trytond_stock-6.6.3/delivery_note.fodt` & `trytond_stock-6.8.0/delivery_note.fodt`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.6.3/doc/conf.py` & `trytond_stock-6.8.0/doc/conf.py`

 * *Files 18% similar despite different names*

```diff
@@ -29,15 +29,18 @@
         stdout=subprocess.PIPE, check=True, cwd=module_dir)
     info['name'] = result.stdout.decode('utf-8').strip()
 
     result = subprocess.run(
         [sys.executable, 'setup.py', '--version'],
         stdout=subprocess.PIPE, check=True, cwd=module_dir)
     version = result.stdout.decode('utf-8').strip()
-    if 'dev' in version:
+    major_version, minor_version, _ = version.split('.', 2)
+    major_version = int(major_version)
+    minor_version = int(minor_version)
+    if minor_version % 2:
         info['series'] = 'latest'
     else:
         info['series'] = '.'.join(version.split('.', 2)[:2])
 
     for key in {'depends', 'extras_depend'}:
         info[key] = info.get(key, '').strip().splitlines()
     info['modules'] = set(info['depends'] + info['extras_depend'])
```

### Comparing `trytond_stock-6.6.3/doc/design/configuration.rst` & `trytond_stock-6.8.0/doc/design/configuration.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.6.3/doc/design/inventory.rst` & `trytond_stock-6.8.0/doc/design/inventory.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.6.3/doc/design/location.rst` & `trytond_stock-6.8.0/doc/design/location.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.6.3/doc/design/move.rst` & `trytond_stock-6.8.0/doc/design/move.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.6.3/doc/design/period.rst` & `trytond_stock-6.8.0/doc/design/period.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.6.3/doc/design/product.rst` & `trytond_stock-6.8.0/doc/design/product.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.6.3/doc/design/shipment.rst` & `trytond_stock-6.8.0/doc/design/shipment.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.6.3/doc/setup.rst` & `trytond_stock-6.8.0/doc/setup.rst`

 * *Files 10% similar despite different names*

```diff
@@ -41,24 +41,21 @@
 In order to ensure the value of your stock is correctly calculated, and to
 show that this stock has (at some point in the past) come from a supplier,
 you must enter this initial stock in the correct way.
 
 The right way of doing this is to create a set of individual
 `Stock Moves <model-stock.move>`.
 These moves can be created in the view that is opened from the
-|Inventory & Stock --> Moves|__ main menu item.
+:menuselection:`Inventory & Stock --> Moves` main menu item.
 Each of the stock moves should move some stock of a `Product <concept-product>`
 from a supplier `Location <model-stock.location>` to the appropriate storage
 location.
 These stock moves must have their unit prices set to their product's cost
 price.
 
-.. |Inventory & Stock --> Moves| replace:: :menuselection:`Inventory & Stock --> Moves`
-__ https://demo.tryton.org/model/stock.move
-
 .. note::
 
    As these moves are for your initial stock they have no origin, and
    when you try and do these moves Tryton will warn you about this.
    Because this is for your initial stock this is not a problem, and you
    can safely go ahead and finish doing the moves.
```

### Comparing `trytond_stock-6.6.3/doc/usage/period.rst` & `trytond_stock-6.8.0/doc/usage/period.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.6.3/doc/usage/quantity.rst` & `trytond_stock-6.8.0/doc/usage/quantity.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.6.3/doc/usage/shipment.rst` & `trytond_stock-6.8.0/doc/usage/shipment.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.6.3/doc/usage/value.rst` & `trytond_stock-6.8.0/doc/usage/value.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.6.3/exceptions.py` & `trytond_stock-6.8.0/exceptions.py`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.6.3/icons/LICENSE` & `trytond_stock-6.8.0/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.6.3/internal_shipment.fodt` & `trytond_stock-6.8.0/internal_shipment.fodt`

 * *Files 0% similar despite different names*

#### Comparing `trytond_stock-6.6.3/internal_shipment.fodt` & `trytond_stock-6.8.0/internal_shipment.fodt`

```diff
@@ -555,15 +555,15 @@
               <text:p text:style-name="P9">Quantity</text:p>
             </table:table-cell>
           </table:table-row>
         </table:table-header-rows>
         <table:table-row>
           <table:table-cell table:style-name="Table1.A4" table:number-columns-spanned="2" office:value-type="string">
             <text:p text:style-name="Table_20_Contents">
-              <text:placeholder text:placeholder-type="text">&lt;for each=&quot;move in moves[shipment.id]&quot;&gt;</text:placeholder>
+              <text:placeholder text:placeholder-type="text">&lt;for each=&quot;move in moves(shipment)&quot;&gt;</text:placeholder>
             </text:p>
           </table:table-cell>
           <table:covered-table-cell/>
           <table:table-cell table:style-name="Table1.C4" office:value-type="string">
             <text:p text:style-name="P10"/>
           </table:table-cell>
           <table:table-cell table:style-name="Table1.D4" office:value-type="string">
```

### Comparing `trytond_stock-6.6.3/inventory.py` & `trytond_stock-6.8.0/inventory.py`

 * *Files 1% similar despite different names*

```diff
@@ -408,16 +408,15 @@
     @fields.depends('product')
     def on_change_product(self):
         if self.product:
             self.uom = self.product.default_uom
 
     @fields.depends('inventory', '_parent_inventory.location')
     def on_change_with_inventory_location(self, name=None):
-        if self.inventory and self.inventory.location:
-            return self.inventory.location.id
+        return self.inventory.location if self.inventory else None
 
     @classmethod
     def search_inventory_location(cls, name, clause):
         nested = clause[0][len(name):]
         return [('inventory.' + name + nested, *clause[1:])]
 
     @fields.depends('inventory', '_parent_inventory.date')
```

### Comparing `trytond_stock-6.6.3/inventory.xml` & `trytond_stock-6.8.0/inventory.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.6.3/ir.py` & `trytond_stock-6.8.0/ir.py`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.6.3/locale/bg.po` & `trytond_stock-6.8.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.6.3/locale/ca.po` & `trytond_stock-6.8.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.6.3/locale/cs.po` & `trytond_stock-6.8.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.6.3/locale/de.po` & `trytond_stock-6.8.0/locale/de.po`

 * *Files 0% similar despite different names*

```diff
@@ -316,15 +316,15 @@
 
 msgctxt "field:stock.location,parent:"
 msgid "Parent"
 msgstr "Übergeordnet (Lagerort)"
 
 msgctxt "field:stock.location,picking_location:"
 msgid "Picking"
-msgstr "Lagerort Picking"
+msgstr "Lagerort Kommissionierung"
 
 msgctxt "field:stock.location,quantity:"
 msgid "Quantity"
 msgstr "Menge"
 
 msgctxt "field:stock.location,quantity_uom:"
 msgid "Quantity UOM"
@@ -1677,15 +1677,15 @@
 
 msgctxt "model:ir.action,name:act_move_form"
 msgid "Moves"
 msgstr "Warenbewegungen"
 
 msgctxt "model:ir.action,name:act_period_list"
 msgid "Periods"
-msgstr "Lagerperioden"
+msgstr "Anwesenheitszeiträume"
 
 msgctxt "model:ir.action,name:act_product_cost_price_revision"
 msgid "Cost Price Revision"
 msgstr "Einstandspreisänderung"
 
 msgctxt "model:ir.action,name:act_product_moves"
 msgid "Stock Moves"
@@ -1773,15 +1773,15 @@
 
 msgctxt "model:ir.action,name:report_shipment_out_delivery_note"
 msgid "Delivery Note"
 msgstr "Lieferschein"
 
 msgctxt "model:ir.action,name:report_shipment_out_picking_list"
 msgid "Picking List"
-msgstr "Pickliste"
+msgstr "Kommissionierliste"
 
 msgctxt "model:ir.action,name:report_shipment_out_return_restocking_list"
 msgid "Restocking List"
 msgstr "Einlagerungsliste"
 
 msgctxt "model:ir.action,name:wizard_inventory_count"
 msgid "Count"
@@ -2537,15 +2537,15 @@
 
 msgctxt "model:ir.ui.menu,name:menu_move_form"
 msgid "Moves"
 msgstr "Warenbewegungen"
 
 msgctxt "model:ir.ui.menu,name:menu_period_list"
 msgid "Periods"
-msgstr "Lagerperioden"
+msgstr "Anwesenheitszeiträume"
 
 msgctxt "model:ir.ui.menu,name:menu_reporting"
 msgid "Reporting"
 msgstr "Auswertungen"
 
 msgctxt "model:ir.ui.menu,name:menu_reporting_margin"
 msgid "Margins"
@@ -2921,15 +2921,15 @@
 
 msgctxt "report:stock.shipment.out.picking_list:"
 msgid "From Location"
 msgstr "Von Lagerort"
 
 msgctxt "report:stock.shipment.out.picking_list:"
 msgid "Picking List"
-msgstr "Pickliste"
+msgstr "Kommissionierliste"
 
 msgctxt "report:stock.shipment.out.picking_list:"
 msgid "Planned Date:"
 msgstr "Geplantes Datum:"
 
 msgctxt "report:stock.shipment.out.picking_list:"
 msgid "Product"
```

### Comparing `trytond_stock-6.6.3/locale/es.po` & `trytond_stock-6.8.0/locale/es.po`

 * *Files 0% similar despite different names*

```diff
@@ -3023,15 +3023,15 @@
 
 msgctxt "selection:stock.inventory,state:"
 msgid "Cancelled"
 msgstr "Cancelado"
 
 msgctxt "selection:stock.inventory,state:"
 msgid "Done"
-msgstr "Finalizar"
+msgstr "Finalizado"
 
 msgctxt "selection:stock.inventory,state:"
 msgid "Draft"
 msgstr "Borrador"
 
 msgctxt "selection:stock.inventory.count.search,search:"
 msgid "Product"
```

### Comparing `trytond_stock-6.6.3/locale/es_419.po` & `trytond_stock-6.8.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.6.3/locale/et.po` & `trytond_stock-6.8.0/locale/et.po`

 * *Files 1% similar despite different names*

```diff
@@ -2,99 +2,90 @@
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:party.address,delivery:"
 msgid "Delivery"
 msgstr "Tarne"
 
-#, fuzzy
 msgctxt "field:party.address,warehouses:"
 msgid "Warehouses"
-msgstr "Ladu"
+msgstr "Laod"
 
-#, fuzzy
 msgctxt "field:party.contact_mechanism,delivery:"
 msgid "Delivery"
 msgstr "Tarne"
 
 msgctxt "field:party.party,customer_location:"
 msgid "Customer Location"
 msgstr "Kliendi asukoht"
 
-#, fuzzy
 msgctxt "field:party.party,delivered_to_warehouses:"
 msgid "Delivered to Warehouses"
-msgstr "Ladu"
+msgstr "Tarnitakse ladudesse"
 
 msgctxt "field:party.party,locations:"
 msgid "Locations"
 msgstr "Asukohad"
 
 msgctxt "field:party.party,supplier_location:"
 msgid "Supplier Location"
 msgstr "Hankija asukoht"
 
-#, fuzzy
 msgctxt "field:party.party-delivered_to-stock.location,location:"
 msgid "Location"
 msgstr "Asukoht"
 
-#, fuzzy
 msgctxt "field:party.party-delivered_to-stock.location,party:"
 msgid "Party"
-msgstr "Osapool"
+msgstr "Partner"
 
 msgctxt "field:party.party.location,customer_location:"
 msgid "Customer Location"
 msgstr "Kliendi asukoht"
 
 msgctxt "field:party.party.location,party:"
 msgid "Party"
-msgstr "Osapool"
+msgstr "Partner"
 
 msgctxt "field:party.party.location,supplier_location:"
 msgid "Supplier Location"
 msgstr "Hankija asukoht"
 
 msgctxt "field:product.by_location.context,forecast_date:"
 msgid "At Date"
 msgstr "Kuupäeval"
 
 msgctxt "field:product.by_location.context,stock_date_end:"
 msgid "At Date"
 msgstr "Kuupäeval"
 
-#, fuzzy
 msgctxt "field:product.cost_price.revision,company:"
 msgid "Company"
 msgstr "Ettevõte"
 
-#, fuzzy
 msgctxt "field:product.cost_price.revision,cost_price:"
 msgid "New Cost Price"
-msgstr "Kuluväärtus"
+msgstr "Uus omahind"
 
-#, fuzzy
 msgctxt "field:product.cost_price.revision,date:"
 msgid "Date"
 msgstr "Kuupäev"
 
 msgctxt "field:product.cost_price.revision,product:"
 msgid "Variant"
-msgstr ""
+msgstr "Variant"
 
 #, fuzzy
 msgctxt "field:product.cost_price.revision,template:"
 msgid "Product"
 msgstr "Toode"
 
-#, fuzzy
 msgctxt "field:product.modify_cost_price.start,cost_price:"
 msgid "New Cost Price"
-msgstr "Kuluväärtus"
+msgstr "Uus omahind"
 
 #, fuzzy
 msgctxt "field:product.modify_cost_price.start,date:"
 msgid "Date"
 msgstr "Kuupäev"
 
 msgctxt "field:product.product,cost_value:"
@@ -107,15 +98,15 @@
 
 msgctxt "field:product.product,quantity:"
 msgid "Quantity"
 msgstr "Kogus"
 
 msgctxt "field:product.recompute_cost_price.start,from_:"
 msgid "From"
-msgstr ""
+msgstr "Alates"
 
 msgctxt "field:product.template,cost_value:"
 msgid "Cost Value"
 msgstr "Kuluväärtus"
 
 msgctxt "field:product.template,forecast_quantity:"
 msgid "Forecast Quantity"
@@ -2549,15 +2540,15 @@
 
 msgctxt "model:ir.ui.menu,name:menu_configuration"
 msgid "Configuration"
 msgstr "Seadistus"
 
 msgctxt "model:ir.ui.menu,name:menu_inventory_form"
 msgid "Inventories"
-msgstr "Kaubad"
+msgstr "Inventuurid"
 
 msgctxt "model:ir.ui.menu,name:menu_location_form"
 msgid "Locations"
 msgstr "Asukohad"
 
 msgctxt "model:ir.ui.menu,name:menu_location_form2"
 msgid "Locations"
```

### Comparing `trytond_stock-6.6.3/locale/fa.po` & `trytond_stock-6.8.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.6.3/locale/fi.po` & `trytond_stock-6.8.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.6.3/locale/fr.po` & `trytond_stock-6.8.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.6.3/locale/hu.po` & `trytond_stock-6.8.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.6.3/locale/id.po` & `trytond_stock-6.8.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.6.3/locale/it.po` & `trytond_stock-6.8.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.6.3/locale/lo.po` & `trytond_stock-6.8.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.6.3/locale/lt.po` & `trytond_stock-6.8.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.6.3/locale/nl.po` & `trytond_stock-6.8.0/locale/nl.po`

 * *Files 0% similar despite different names*

```diff
@@ -2264,15 +2264,15 @@
 
 msgctxt "model:ir.model.button,string:move_draft_button"
 msgid "Reset to Draft"
 msgstr "Terug naar concept"
 
 msgctxt "model:ir.model.button,string:period_close_button"
 msgid "Close"
-msgstr "Afsluiten"
+msgstr "Sluiten"
 
 msgctxt "model:ir.model.button,string:period_draft_button"
 msgid "Draft"
 msgstr "Concept"
 
 msgctxt "model:ir.model.button,string:shipment_in_cancel_button"
 msgid "Cancel"
```

### Comparing `trytond_stock-6.6.3/locale/pl.po` & `trytond_stock-6.8.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.6.3/locale/pt.po` & `trytond_stock-6.8.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.6.3/locale/ro.po` & `trytond_stock-6.8.0/locale/ro.po`

 * *Files 2% similar despite different names*

```diff
@@ -2,46 +2,42 @@
 msgid ""
 msgstr "Content-Type: text/plain; charset=utf-8\n"
 
 msgctxt "field:party.address,delivery:"
 msgid "Delivery"
 msgstr "Livrare"
 
-#, fuzzy
 msgctxt "field:party.address,warehouses:"
 msgid "Warehouses"
-msgstr "Depozit"
+msgstr "Depozite"
 
 msgctxt "field:party.contact_mechanism,delivery:"
 msgid "Delivery"
 msgstr "Livrare"
 
 msgctxt "field:party.party,customer_location:"
 msgid "Customer Location"
 msgstr "Locaţia Client"
 
-#, fuzzy
 msgctxt "field:party.party,delivered_to_warehouses:"
 msgid "Delivered to Warehouses"
-msgstr "Depozit Curent"
+msgstr "Livrat la Depozite"
 
 msgctxt "field:party.party,locations:"
 msgid "Locations"
 msgstr "Locaţii"
 
 msgctxt "field:party.party,supplier_location:"
 msgid "Supplier Location"
 msgstr "Locaţia Furnizor"
 
-#, fuzzy
 msgctxt "field:party.party-delivered_to-stock.location,location:"
 msgid "Location"
 msgstr "Locație"
 
-#, fuzzy
 msgctxt "field:party.party-delivered_to-stock.location,party:"
 msgid "Party"
 msgstr "Parte"
 
 msgctxt "field:party.party.location,customer_location:"
 msgid "Customer Location"
 msgstr "Locaţia Client"
@@ -272,15 +268,15 @@
 
 msgctxt "field:stock.location,address:"
 msgid "Address"
 msgstr "Adresa"
 
 msgctxt "field:stock.location,allow_pickup:"
 msgid "Allow Pickup"
-msgstr ""
+msgstr "Permite Ridicare"
 
 msgctxt "field:stock.location,childs:"
 msgid "Children"
 msgstr "Copii"
 
 msgctxt "field:stock.location,code:"
 msgid "Code"
@@ -831,15 +827,14 @@
 msgid "Supplier"
 msgstr "Furnizor"
 
 msgctxt "field:stock.shipment.in.return,to_location:"
 msgid "To Location"
 msgstr "Spre Locație"
 
-#, fuzzy
 msgctxt "field:stock.shipment.in.return,warehouse:"
 msgid "Warehouse"
 msgstr "Depozit"
 
 msgctxt "field:stock.shipment.internal,assigned_by:"
 msgid "Received By"
 msgstr "Primit De"
@@ -996,15 +991,14 @@
 msgid "Warehouse Storage"
 msgstr "Depozit Depozitare"
 
 msgctxt "field:stock.shipment.out.return,company:"
 msgid "Company"
 msgstr "Companie"
 
-#, fuzzy
 msgctxt "field:stock.shipment.out.return,contact_address:"
 msgid "Contact Address"
 msgstr "Adresa de Contact"
 
 msgctxt "field:stock.shipment.out.return,customer:"
 msgid "Customer"
 msgstr "Client"
@@ -1595,15 +1589,14 @@
 msgid "Where the stock is sent from."
 msgstr "De unde este trimis stocul."
 
 msgctxt "help:stock.shipment.out.return,company:"
 msgid "The company the shipment is associated with."
 msgstr "Compania cu care este asociată expedierea."
 
-#, fuzzy
 msgctxt "help:stock.shipment.out.return,contact_address:"
 msgid "The address the customer can be contacted at."
 msgstr "Adresa la care poate fi contactat clientul."
 
 msgctxt "help:stock.shipment.out.return,customer:"
 msgid "The party that purchased the stock."
 msgstr "Partea care a achiziţionat stocul."
@@ -2008,45 +2001,56 @@
 
 msgctxt "model:ir.message,text:msg_inventory_location_missing_lost_found"
 msgid ""
 "To confirm the inventory \"%(inventory)s\" you must set a lost and found on "
 "a parent of location \"%(location)s\"."
 msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_inventory_missing_empty_quantity"
 msgid ""
 "To confirm the inventory \"%(inventory)s\" you must select an option for "
 "empty quantity."
 msgstr ""
+"Pentru a confirma inventarul \"%(inventory)s\" este necesară o selecție "
+"pentru cantitate zero."
 
 msgctxt "model:ir.message,text:msg_location_child_of_warehouse"
 msgid ""
 "To set location \"%(location)s\" as storage/input/output of warehouse "
 "\"%(warehouse)s\", it must be in the warehouse."
 msgstr ""
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_location_inactive_not_empty"
 msgid "To inactivate location \"%(location)s\", you must empty it."
-msgstr ""
+msgstr "Locația \"%(location)s\" trebuie să fie goală pentru a fi dezactivată."
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_location_invalid_type_for_moves"
 msgid ""
 "You cannot change the type of location \"%(location)s\" to \"%(type)s\"\n"
 "because the type does not support moves and location has existing moves."
 msgstr ""
+"Nu se poate schimba tipul de locație \"%(location)s\" la \"%(type)s\"\n"
+"deoarece acest tip nu suportă mutări, iar locația are mutări existente."
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_move_delete_draft_cancel"
 msgid ""
 "To delete stock move \"%(move)s\" you must cancel it or reset its state to "
 "draft."
 msgstr ""
+"Pentru a șterge mutarea de stoc \"%(move)s\" este necesar să o anulați sau "
+"să ii resetați starea la Ciornă."
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_move_effective_date_in_the_future"
 msgid "The moves \"%(moves)s\" have effective dates in the future."
-msgstr ""
+msgstr "Mutările \"%(moves)s\" au date efective în viitor."
 
 msgctxt "model:ir.message,text:msg_move_from_to_location"
 msgid "The source and destination of stock move must be different."
 msgstr "Sursa şi destinaţia unei mişcări de stoc trebuie sa fie diferite."
 
 msgctxt "model:ir.message,text:msg_move_internal_quantity_positive"
 msgid "Internal move quantity must be positive."
@@ -2059,67 +2063,82 @@
 "de draft."
 
 msgctxt "model:ir.message,text:msg_move_modify_cancelled"
 msgid "You cannot modify stock move \"%(move)s\" because it is cancelled."
 msgstr ""
 "Nu se poate modifica mişcarea de stoc \"%(move)s\" pentru că este anulată."
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_move_modify_done"
 msgid "You cannot modify stock move \"%(move)s\" because it is done."
 msgstr ""
+"Nu se poate modifica mutarea de stoc \"%(move)s\" deoarece a fost deja "
+"efectuată."
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_move_modify_period_close"
 msgid "To modify stock move \"%(move)s\" you must reopen period \"%(period)s\"."
 msgstr ""
+"Pentru a modifica mutarea de stoc \"%(move)s\" trebuie să redeschideți "
+"perioada \"%(period)s\"."
 
+#, fuzzy
 msgctxt "model:ir.message,text:msg_move_no_origin"
 msgid "Stock moves \"%(moves)s\" have no origin."
-msgstr ""
+msgstr "Mutările de stoc \"%(moves)s\" nu au origine."
 
 msgctxt "model:ir.message,text:msg_move_quantity_positive"
 msgid "Move quantity must be positive."
 msgstr "Cantitatea de mișcare trebuie să fie pozitivă."
 
 msgctxt "model:ir.message,text:msg_period_close_assigned_move"
 msgid "You cannot close periods with assigned moves in it."
 msgstr "Nu puteți închide perioadele cu mutări atribuite."
 
 msgctxt "model:ir.message,text:msg_period_close_date"
 msgid "You cannot close periods with a date in the future or today."
 msgstr ""
+"Nu se pot închide perioade cu date din viitor sau cu data zilei in curs."
 
 msgctxt "model:ir.message,text:msg_product_change_cost_price"
 msgid ""
 "You cannot change the cost price of a product which is associated with stock moves.\n"
 "You must use the \"Modify Cost Price\" wizard."
 msgstr ""
 
 msgctxt "model:ir.message,text:msg_product_change_default_uom"
 msgid ""
 "You cannot change the default UOM of a product which is associated with "
 "stock moves."
 msgstr ""
+"Nu se poate schimba Unitatea de Masură implicită a unui produs asociat cu "
+"mutari de stoc."
 
 msgctxt "model:ir.message,text:msg_product_change_type"
 msgid ""
 "You cannot change the type of a product which is associated with stock "
 "moves."
 msgstr ""
+"Nu se poate schimba tipul unui produs care este asociat cu mutări de stoc."
 
 msgctxt "model:ir.message,text:msg_product_location_quantity"
 msgid ""
 "The product \"%(product)s\" has still some quantities in locations "
 "\"%(locations)s\" for company \"%(company)s\"."
 msgstr ""
+"Încă există cantități de produs \"%(product)s\" în locațiile "
+"\"%(locations)s\" pentru compania \"%(company)s\"."
 
 msgctxt "model:ir.message,text:msg_product_location_quantity_description"
 msgid ""
 "It is recommended to clear the stock from the storage locations before "
 "deactivating the product."
 msgstr ""
+"Este recomandată lichidarea stocurilor din locațiile de depozitare înaintea "
+"dezactivării produsului."
 
 msgctxt "model:ir.message,text:msg_shipment_delete_cancel"
 msgid "To delete shipment \"%(shipment)s\" you must cancel it."
 msgstr ""
 
 #, fuzzy
 msgctxt "model:ir.message,text:msg_shipment_pack_inventory_done"
```

### Comparing `trytond_stock-6.6.3/locale/ru.po` & `trytond_stock-6.8.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.6.3/locale/sl.po` & `trytond_stock-6.8.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.6.3/locale/tr.po` & `trytond_stock-6.8.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.6.3/locale/uk.po` & `trytond_stock-6.8.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.6.3/locale/zh_CN.po` & `trytond_stock-6.8.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.6.3/location.py` & `trytond_stock-6.8.0/location.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 from trytond.cache import Cache
 from trytond.i18n import gettext
 from trytond.model import (
     DeactivableMixin, Index, MatchMixin, Model, ModelSQL, ModelView, fields,
     sequence_ordered, tree)
 from trytond.modules.product import price_digits, round_price
 from trytond.pool import Pool
-from trytond.pyson import Eval, If
+from trytond.pyson import Eval, If, TimeDelta
 from trytond.tools import grouped_slice
-from trytond.transaction import Transaction
+from trytond.transaction import Transaction, inactive_records
 
 from .exceptions import LocationValidationError
 
 
 class WarehouseWasteLocation(ModelSQL):
     "Warehouse Waste Location"
     __name__ = 'stock.location.waste'
@@ -55,15 +55,15 @@
         ('storage', 'Storage'),
         ('production', 'Production'),
         ('drop', 'Drop'),
         ('view', 'View'),
         ], "Location type")
     type_string = type.translated('type')
     parent = fields.Many2One(
-        "stock.location", "Parent",
+        "stock.location", "Parent", ondelete='CASCADE',
         left="left", right="right",
         help="Used to add structure above the location.")
     left = fields.Integer('Left', required=True)
     right = fields.Integer('Right', required=True)
     childs = fields.One2Many("stock.location", "parent", "Children",
         help="Used to add structure below the location.")
     flat_childs = fields.Boolean(
@@ -285,16 +285,15 @@
         if locations is None:
             locations = cls.search([])
         if not locations:
             return []
         location_ids = list(map(int, locations))
         # Use root to compute for all companies
         # and ensures inactive locations are in the query
-        with Transaction().set_user(0), \
-                Transaction().set_context(active_test=False):
+        with Transaction().set_user(0), inactive_records():
             query = Move.compute_quantities_query(
                 location_ids, with_childs=True)
             quantities = Move.compute_quantities(
                 query, location_ids, with_childs=True)
             empty = set(location_ids)
             product_ids = [q[1] for q in quantities.keys()]
             consumables = {
@@ -330,19 +329,19 @@
 
     @staticmethod
     def default_type():
         return 'storage'
 
     @classmethod
     def check_xml_record(cls, records, values):
-        return True
+        pass
 
     def get_warehouse(self, name):
         # Order by descending left to get the first one in the tree
-        with Transaction().set_context(active_test=False):
+        with inactive_records():
             locations = self.search([
                     ('parent', 'parent_of', [self.id]),
                     ('type', '=', 'warehouse'),
                     ], order=[('left', 'DESC')])
         if locations:
             return locations[0].id
 
@@ -570,16 +569,24 @@
                 if location not in childs:
                     raise LocationValidationError(
                         gettext('stock.msg_location_child_of_warehouse',
                             location=location.rec_name,
                             warehouse=warehouse.rec_name))
 
     @classmethod
-    def delete(cls, *args):
-        super().delete(*args)
+    def delete(cls, locations):
+        # Delete also required children as CASCADING is done separately
+        extra_locations = []
+        for location in locations:
+            extra_locations.extend(filter(None, [
+                        location.input_location,
+                        location.output_location,
+                        location.storage_location,
+                        ]))
+        super().delete(locations + extra_locations)
         cls._default_warehouse_cache.clear()
 
     @classmethod
     def copy(cls, locations, default=None):
         if default is None:
             default = {}
         else:
@@ -743,15 +750,20 @@
             ])
     warehouse_to = fields.Many2One('stock.location', 'Warehouse To',
         ondelete='CASCADE',
         domain=[
             ('type', '=', 'warehouse'),
             ('id', '!=', Eval('warehouse_from', -1)),
             ])
-    lead_time = fields.TimeDelta('Lead Time',
+    lead_time = fields.TimeDelta(
+        "Lead Time",
+        domain=['OR',
+            ('lead_time', '=', None),
+            ('lead_time', '>=', TimeDelta()),
+            ],
         help="The time it takes to move stock between the warehouses.")
 
     @classmethod
     def get_lead_time(cls, pattern):
         for record in cls.search([]):
             if record.match(pattern):
                 return record.lead_time
```

### Comparing `trytond_stock-6.6.3/location.xml` & `trytond_stock-6.8.0/location.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.6.3/message.xml` & `trytond_stock-6.8.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.6.3/move.py` & `trytond_stock-6.8.0/move.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from trytond.model import (
     Check, Index, Model, ModelSQL, ModelView, Workflow, fields)
 from trytond.model.exceptions import AccessError
 from trytond.modules.product import price_digits, round_price
 from trytond.pool import Pool
 from trytond.pyson import Bool, Eval, If
 from trytond.tools import grouped_slice, reduce_ids
-from trytond.transaction import Transaction
+from trytond.transaction import Transaction, without_check_access
 
 from .exceptions import MoveFutureWarning, MoveOriginWarning
 
 STATES = {
     'readonly': Eval('state').in_(['cancelled', 'assigned', 'done']),
 }
 LOCATION_DOMAIN = [
@@ -420,16 +420,15 @@
         if self.product:
             if (not self.uom
                     or self.uom.category != self.product.default_uom.category):
                 self.uom = self.product.default_uom
 
     @fields.depends('product')
     def on_change_with_product_uom_category(self, name=None):
-        if self.product:
-            return self.product.default_uom_category.id
+        return self.product.default_uom_category if self.product else None
 
     @classmethod
     def get_unit_price_company(cls, moves, name):
         pool = Pool()
         Currency = pool.get('currency.currency')
         Uom = pool.get('product.uom')
         Date = pool.get('ir.date')
@@ -538,32 +537,32 @@
         return [(None, '')] + [(m, get_name(m)) for m in models]
 
     @property
     def origin_name(self):
         return self.origin.rec_name if self.origin else None
 
     @classmethod
+    @without_check_access
     def check_period_closed(cls, moves):
         Period = Pool().get('stock.period')
-        with Transaction().set_context(_check_access=False):
-            for company, moves in groupby(moves, lambda m: m.company):
-                periods = Period.search([
-                        ('state', '=', 'closed'),
-                        ('company', '=', company.id),
-                        ], order=[('date', 'DESC')], limit=1)
-                if periods:
-                    period, = periods
-                    for move in moves:
-                        date = (move.effective_date if move.effective_date
-                            else move.planned_date)
-                        if date and date <= period.date:
-                            raise AccessError(
-                                gettext('stock.msg_move_modify_period_close',
-                                    move=move.rec_name,
-                                    period=period.rec_name))
+        for company, moves in groupby(moves, lambda m: m.company):
+            periods = Period.search([
+                    ('state', '=', 'closed'),
+                    ('company', '=', company.id),
+                    ], order=[('date', 'DESC')], limit=1)
+            if periods:
+                period, = periods
+                for move in moves:
+                    date = (move.effective_date if move.effective_date
+                        else move.planned_date)
+                    if date and date <= period.date:
+                        raise AccessError(
+                            gettext('stock.msg_move_modify_period_close',
+                                move=move.rec_name,
+                                period=period.rec_name))
 
     def get_rec_name(self, name):
         pool = Pool()
         Lang = pool.get('ir.lang')
         lang = Lang.get()
         return (lang.format_number_symbol(
                 self.quantity, self.uom, digits=self.uom.digits)
@@ -779,21 +778,23 @@
         with Transaction().set_context(company=moves[0].company.id):
             context['stock_date_end'] = Date.today()
         context['company'] = moves[0].company.id
         return context
 
     def _do(self):
         "Return cost_price and a list of moves to save"
+        cost_price_method = self.product.get_multivalue(
+            'cost_price_method', **self._cost_price_pattern)
         if (self.from_location.type in ('supplier', 'production')
                 and self.to_location.type == 'storage'
-                and self.product.cost_price_method == 'average'):
+                and cost_price_method == 'average'):
             return self._compute_product_cost_price('in'), []
         elif (self.to_location.type == 'supplier'
                 and self.from_location.type == 'storage'
-                and self.product.cost_price_method == 'average'):
+                and cost_price_method == 'average'):
             return self._compute_product_cost_price('out'), []
         return None, []
 
     @classmethod
     @ModelView.button
     @Workflow.transition('cancelled')
     def cancel(cls, moves):
@@ -1008,17 +1009,28 @@
                 if p is None or k == p:
                     continue
                 else:
                     return False
             else:
                 return True
 
+        def default_values(values):
+            def get_value(name):
+                def get_default(data):
+                    return values[data['id']][name]
+                return get_default
+            default = {}
+            for name in set().union(*(v.keys() for v in values.values())):
+                default[name] = get_value(name)
+            return default
+
         child_locations = {}
         to_write = []
         to_assign = []
+        to_copy = defaultdict(list)
         success = True
         for move in moves:
             if move.state != 'draft':
                 if move.state == 'staging':
                     success = False
                 continue
             pbl = pblc[move.company.id]
@@ -1076,21 +1088,34 @@
                 values = dict(get_values(key, 'from_location'))
                 values['quantity'] = move.uom.round(qty)
                 if first:
                     to_write.extend([[move], values])
                     to_assign.append(move)
                     first = False
                 else:
-                    with Transaction().set_context(_stock_move_split=True):
-                        to_assign.extend(cls.copy([move], default=values))
+                    to_copy[move].append(values)
 
                 qty_default_uom = Uom.compute_qty(move.uom, qty,
                         move.product.default_uom, round=False)
 
                 pbl[key] = pbl.get(key, 0.0) - qty_default_uom
+
+        with Transaction().set_context(_stock_move_split=True):
+            while to_copy:
+                moves_to_copy = []
+                values = {}
+                for move, vlist in list(to_copy.items()):
+                    if vlist:
+                        moves_to_copy.append(move)
+                        values[move.id] = vlist.pop(0)
+                    else:
+                        del to_copy[move]
+                to_assign.extend(cls.copy(
+                        moves_to_copy,
+                        default=default_values(values)))
         if to_write:
             cls.write(*to_write)
         if to_assign:
             cls.assign(to_assign)
         return success
 
     @classmethod
@@ -1151,14 +1176,15 @@
                 two dates, (ignored if stock_date_end is missing).
             stock_assign: if set compute also the assigned outgoing moves as
                 done at the stock_date_end except for delta which is at the
                 planned date.
             forecast: if set compute the forecast quantity.
             stock_destinations: A list of location ids. If set, restrict the
                 computation to moves from and to those locations.
+            stock_invert: if set invert the quantity.
         If with_childs, it computes also for child locations.
         grouping is a tuple of Move (or Product if prefixed by 'product.' or
             'date') field names and defines how stock moves are grouped.
         grouping_filter is a tuple of values, for the Move's field at the same
             position in grouping tuple, used to filter which moves are used to
             compute quantities. It must be None or have the same number of
             elements than grouping. If no grouping_filter is provided it
@@ -1513,17 +1539,20 @@
                     where=(period_cache.period
                         == (period.id if period else None))
                     & where_period
                     & period_cache.location.in_(location_query)
                     & dest_clause_period),
                 all_=True)
         query_keys = [Column(query, key).as_(key) for key in grouping]
+        quantity = Sum(query.quantity)
+        if context.get('stock_invert'):
+            quantity *= -1
         columns = ([query.location.as_('location')]
             + query_keys
-            + [Sum(query.quantity).as_('quantity')])
+            + [quantity.as_('quantity')])
         query = query.select(*columns,
             group_by=[query.location] + query_keys)
         return query
 
     @classmethod
     def compute_quantities(cls, query, location_ids, with_childs=False,
             grouping=('product',), grouping_filter=None):
```

### Comparing `trytond_stock-6.6.3/move.xml` & `trytond_stock-6.8.0/move.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.6.3/party.py` & `trytond_stock-6.8.0/party.py`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.6.3/party.xml` & `trytond_stock-6.8.0/party.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.6.3/period.py` & `trytond_stock-6.8.0/period.py`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.6.3/period.xml` & `trytond_stock-6.8.0/period.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.6.3/picking_list.fodt` & `trytond_stock-6.8.0/picking_list.fodt`

 * *Files 0% similar despite different names*

#### Comparing `trytond_stock-6.6.3/picking_list.fodt` & `trytond_stock-6.8.0/picking_list.fodt`

```diff
@@ -519,15 +519,15 @@
               <text:p text:style-name="P11">Quantity</text:p>
             </table:table-cell>
           </table:table-row>
         </table:table-header-rows>
         <table:table-row>
           <table:table-cell table:style-name="Table1.A4" table:number-columns-spanned="2" office:value-type="string">
             <text:p text:style-name="Table_20_Contents">
-              <text:placeholder text:placeholder-type="text">&lt;for each=&quot;move in moves[shipment.id]&quot;&gt;</text:placeholder>
+              <text:placeholder text:placeholder-type="text">&lt;for each=&quot;move in moves(shipment)&quot;&gt;</text:placeholder>
             </text:p>
           </table:table-cell>
           <table:covered-table-cell/>
           <table:table-cell table:style-name="Table1.C4" office:value-type="string">
             <text:p text:style-name="Table_20_Contents"/>
           </table:table-cell>
           <table:table-cell table:style-name="Table1.D4" office:value-type="string">
```

### Comparing `trytond_stock-6.6.3/product.py` & `trytond_stock-6.8.0/product.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,16 @@
 from trytond.i18n import gettext
 from trytond.model import Index, ModelSQL, ModelView, fields
 from trytond.model.exceptions import AccessError
 from trytond.modules.product import price_digits, round_price
 from trytond.pool import Pool, PoolMeta
 from trytond.pyson import Bool, Eval, If, PYSONEncoder
 from trytond.tools import decistmt, grouped_slice
-from trytond.transaction import Transaction
+from trytond.tools import timezone as tz
+from trytond.transaction import Transaction, without_check_access
 from trytond.wizard import (
     Button, StateAction, StateTransition, StateView, Wizard)
 
 from .exceptions import ProductCostPriceError, ProductStockWarning
 from .move import StockMixin
 from .shipment import ShipmentAssignMixin
 
@@ -48,16 +49,15 @@
         return False
 
     @functools.wraps(func)
     def decorator(cls, *args):
         pool = Pool()
         Template = pool.get('product.template')
         transaction = Transaction()
-        if (transaction.user != 0
-                and transaction.context.get('_check_access')):
+        if transaction.user and transaction.check_access:
             actions = iter(args)
             for records, values in zip(actions, actions):
                 for field, msg in Template._modify_no_move:
                     if field in values:
                         if find_moves(cls, records):
                             raise AccessError(gettext(msg))
                         # No moves for those records
@@ -129,15 +129,15 @@
 
         to_check = []
         actions = iter(args)
         for products, values in zip(actions, actions):
             if not values.get('active', True):
                 to_check.extend(products)
         if to_check:
-            with Transaction().set_context(_check_access=False):
+            with without_check_access():
                 locations = Location.search([('type', '=', 'storage')])
                 location_ids = list(map(int, locations))
                 for company in Company.search([]):
                     for sub_products in grouped_slice(to_check):
                         product2locations = get_product_locations(
                             company, location_ids, sub_products)
                         raise_warning(company, product2locations)
@@ -213,21 +213,35 @@
     @classmethod
     def search_quantity(cls, name, domain=None):
         location_ids = Transaction().context.get('locations')
         return cls._search_quantity(name, location_ids, domain)
 
     @classmethod
     def get_cost_value(cls, products, name):
+        pool = Pool()
+        Company = pool.get('company.company')
         cost_values = {p.id: None for p in products}
         context = {}
         trans_context = Transaction().context
         if trans_context.get('stock_date_end'):
             # Use the last cost_price of the day
             context['_datetime'] = datetime.datetime.combine(
                 trans_context['stock_date_end'], datetime.time.max)
+            company = trans_context.get('company')
+            if company:
+                company = Company(company)
+                if company.timezone:
+                    timezone = tz.ZoneInfo(company.timezone)
+                    try:
+                        context['_datetime'] = (
+                            context['_datetime']
+                            .replace(tzinfo=timezone)
+                            .astimezone(tz.UTC))
+                    except OverflowError:
+                        pass
             # The date could be before the product creation
             products = [p for p in products
                 if p.create_date <= context['_datetime']]
         with Transaction().set_context(context):
             for product in cls.browse(products):
                 # The product may not have a cost price
                 if product.cost_price is not None:
@@ -334,23 +348,22 @@
         if updated:
             Move.write(updated, {'unit_price_updated': False})
 
         if costs:
             cls.update_cost_price(costs)
 
     @classmethod
+    @without_check_access
     def update_cost_price(cls, costs):
         "Update cost price of products from costs re-computation dictionary"
         to_write = []
         for cost, products in costs.items():
             to_write.append(products)
             to_write.append({'cost_price': cost})
-
-        with Transaction().set_context(_check_access=False):
-            cls.write(*to_write)
+        cls.write(*to_write)
 
     def recompute_cost_price_fixed(self, start=None):
         return self.cost_price
 
     @classmethod
     def _domain_moves_cost(cls):
         "Returns the domain for moves to use in cost computation"
```

### Comparing `trytond_stock-6.6.3/product.xml` & `trytond_stock-6.8.0/product.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.6.3/res.py` & `trytond_stock-6.8.0/res.py`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.6.3/res.xml` & `trytond_stock-6.8.0/res.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.6.3/setup.py` & `trytond_stock-6.8.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,18 +16,15 @@
         'r', encoding='utf-8').read()
     content = re.sub(
         r'(?m)^\.\. toctree::\r?\n((^$|^\s.*$)\r?\n)*', '', content)
     return content
 
 
 def get_require_version(name):
-    if minor_version % 2:
-        require = '%s >= %s.%s.dev0, < %s.%s'
-    else:
-        require = '%s >= %s.%s, < %s.%s'
+    require = '%s >= %s.%s, < %s.%s'
     require %= (name, major_version, minor_version,
         major_version, minor_version + 1)
     return require
 
 
 config = ConfigParser()
 config.read_file(open(os.path.join(os.path.dirname(__file__), 'tryton.cfg')))
@@ -37,38 +34,41 @@
         info[key] = info[key].strip().splitlines()
 version = info.get('version', '0.0.1')
 major_version, minor_version, _ = version.split('.', 2)
 major_version = int(major_version)
 minor_version = int(minor_version)
 name = 'trytond_stock'
 
-download_url = 'http://downloads.tryton.org/%s.%s/' % (
-    major_version, minor_version)
+if minor_version % 2:
+    download_url = ''
+else:
+    download_url = 'http://downloads.tryton.org/%s.%s/' % (
+        major_version, minor_version)
 
 requires = ['python-sql >= 1.3.0', 'simpleeval']
 for dep in info.get('depends', []):
     if not re.match(r'(ir|res)(\W|$)', dep):
         requires.append(get_require_version('trytond_%s' % dep))
 requires.append(get_require_version('trytond'))
 
 tests_require = [get_require_version('proteus')]
 
 setup(name=name,
     version=version,
     description='Tryton module for stock and inventory',
     long_description=read('README.rst'),
     author='Tryton',
-    author_email='bugs@tryton.org',
+    author_email='foundation@tryton.org',
     url='http://www.tryton.org/',
     download_url=download_url,
     project_urls={
         "Bug Tracker": 'https://bugs.tryton.org/',
         "Documentation": 'https://docs.tryton.org/projects/modules-stock/',
         "Forum": 'https://www.tryton.org/forum',
-        "Source Code": 'https://hg.tryton.org/modules/stock',
+        "Source Code": 'https://code.tryton.org/tryton',
         },
     keywords='tryton stock',
     package_dir={'trytond.modules.stock': '.'},
     packages=(
         ['trytond.modules.stock']
         + ['trytond.modules.stock.%s' % p for p in find_packages()]
         ),
@@ -106,23 +106,23 @@
         'Natural Language :: Russian',
         'Natural Language :: Slovenian',
         'Natural Language :: Spanish',
         'Natural Language :: Turkish',
         'Natural Language :: Ukrainian',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: Implementation :: CPython',
         'Topic :: Office/Business',
         ],
     license='GPL-3',
-    python_requires='>=3.7',
+    python_requires='>=3.8',
     install_requires=requires,
     extras_require={
         'sparklines': ['pygal'],
         'test': tests_require,
         },
     zip_safe=False,
     entry_points="""
```

### Comparing `trytond_stock-6.6.3/shipment.py` & `trytond_stock-6.8.0/shipment.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 # This file is part of Tryton.  The COPYRIGHT file at the top level of
 # this repository contains the full copyright notices and license terms.
 import datetime
-import functools
 from collections import defaultdict
 from functools import partial
 from itertools import groupby
 
 from sql import Null
 from sql.conditionals import Coalesce
 from sql.functions import CharLength
 
 from trytond.i18n import gettext
 from trytond.model import (
-    Index, ModelSQL, ModelView, Workflow, dualmethod, fields)
+    Index, ModelSQL, ModelView, Workflow, dualmethod, fields, sort)
 from trytond.model.exceptions import AccessError
 from trytond.modules.company import CompanyReport
 from trytond.modules.company.model import employee_field, set_employee
 from trytond.pool import Pool
 from trytond.pyson import Bool, Eval, Id, If
 from trytond.transaction import Transaction
 from trytond.wizard import Button, StateTransition, StateView, Wizard
@@ -60,24 +59,34 @@
 
     @dualmethod
     @ModelView.button
     def assign_force(cls, shipments):
         cls.assign(shipments)
 
     @dualmethod
-    def assign_ignore(cls, shipments):
+    def assign_ignore(cls, shipments, moves=None):
         pool = Pool()
         Move = pool.get('stock.move')
-        Move.write([
-                m for s in shipments for m in s.assign_moves
-                if m.assignation_required
-                and m.state in {'staging', 'draft'}], {
+        assign_moves = {
+            m for s in shipments for m in s.assign_moves
+            if m.assignation_required and m.state in {'staging', 'draft'}}
+        if moves is None:
+            moves = list(assign_moves)
+        else:
+            moves = [m for m in moves if m in assign_moves]
+        Move.write(moves, {
                 'quantity': 0,
                 })
-        cls.assign(shipments)
+        to_assign = [
+            s for s in shipments
+            if all(
+                m.state not in {'staging', 'draft'}
+                for m in s.assign_moves if m.assignation_required)]
+        if to_assign:
+            cls.assign(to_assign)
 
     @classmethod
     def _get_assign_domain(cls):
         pool = Pool()
         Date = pool.get('ir.date')
         context = Transaction().context
         return [
@@ -169,42 +178,67 @@
     warehouse = fields.Many2One('stock.location', "Warehouse",
         required=True, domain=[('type', '=', 'warehouse')],
         states={
             'readonly': (Eval('state').in_(['cancelled', 'done'])
                 | Eval('incoming_moves', [0]) | Eval('inventory_moves', [0])),
             },
         help="Where the stock is received.")
-    warehouse_input = fields.Function(fields.Many2One('stock.location',
-            'Warehouse Input'),
-        'on_change_with_warehouse_input')
-    warehouse_storage = fields.Function(fields.Many2One('stock.location',
-            'Warehouse Storage'),
-        'on_change_with_warehouse_storage')
+    warehouse_input = fields.Many2One(
+        'stock.location', "Warehouse Input", required=True,
+        domain=[
+            ('type', '=', 'storage'),
+            If(Eval('state') == 'draft',
+                ('parent', 'child_of', [Eval('warehouse', -1)]),
+                ()),
+            ],
+        states={
+            'readonly': Eval('state') != 'draft',
+            })
+    warehouse_storage = fields.Many2One(
+        'stock.location', "Warehouse Storage", required=True,
+        domain=[
+            ('type', '=', 'storage'),
+            If(Eval('state') == 'draft',
+                ('parent', 'child_of', [Eval('warehouse', -1)]),
+                ()),
+            ],
+        states={
+            'readonly': Eval('state') != 'draft',
+            })
     incoming_moves = fields.Function(fields.One2Many('stock.move', 'shipment',
             'Incoming Moves',
             add_remove=[
                 ('shipment', '=', None),
-                ('from_location', '=', Eval('supplier_location')),
                 ('state', '=', 'draft'),
                 If(Eval('warehouse_input') == Eval('warehouse_storage'),
                     ('to_location', 'child_of',
                         [Eval('warehouse_input', -1)], 'parent'),
                     ('to_location', '=', Eval('warehouse_input'))),
                 ],
+            order=[
+                ('product', 'ASC'),
+                ('id', 'ASC'),
+                ],
+            search_order=[
+                ('planned_date', 'ASC NULLS LAST'),
+                ('id', 'ASC')
+                ],
             domain=[
-                ('from_location', '=', Eval('supplier_location')),
+                If(Eval('state') == 'draft',
+                    ('from_location', '=', Eval('supplier_location')),
+                    ()),
                 If(Eval('warehouse_input') == Eval('warehouse_storage'),
                     ('to_location', 'child_of',
                         [Eval('warehouse_input', -1)], 'parent'),
                     ('to_location', '=', Eval('warehouse_input'))),
                 ('company', '=', Eval('company')),
                 ],
             states={
                 'readonly': (
-                    Eval('state').in_(['received', 'done', 'cancelled'])
+                    (Eval('state') != 'draft')
                     | ~Eval('warehouse') | ~Eval('supplier')),
                 },
             help="The moves that bring the stock into the warehouse."),
         'get_incoming_moves', setter='set_incoming_moves')
     inventory_moves = fields.Function(fields.One2Many('stock.move', 'shipment',
             'Inventory Moves',
             domain=[
@@ -215,14 +249,19 @@
                             [Eval('warehouse_storage', -1)], 'parent'),
                         ('to_location.waste_warehouses', '=',
                             Eval('warehouse')),
                         ],
                     [],),
                 ('company', '=', Eval('company')),
                 ],
+            order=[
+                ('to_location', 'ASC'),
+                ('product', 'ASC'),
+                ('id', 'ASC'),
+                ],
             states={
                 'readonly': Eval('state').in_(['draft', 'done', 'cancelled']),
                 'invisible': (
                     Eval('warehouse_input') == Eval('warehouse_storage')),
                 },
             help="The moves that put the stock away into the storage area."),
         'get_inventory_moves', setter='set_inventory_moves')
@@ -282,29 +321,46 @@
                     'invisible': Eval('state') != 'received',
                     'depends': ['state'],
                     },
                 })
 
     @classmethod
     def __register__(cls, module_name):
+        pool = Pool()
+        Location = pool.get('stock.location')
         cursor = Transaction().connection.cursor()
         table = cls.__table_handler__(module_name)
         sql_table = cls.__table__()
+        location = Location.__table__()
 
         # Migration from 3.8: rename code into number
         if table.column_exist('code'):
             table.column_rename('code', 'number')
 
         super(ShipmentIn, cls).__register__(module_name)
 
         # Migration from 5.6: rename state cancel to cancelled
         cursor.execute(*sql_table.update(
                 [sql_table.state], ['cancelled'],
                 where=sql_table.state == 'cancel'))
 
+        # Migration from 6.6: fill warehouse locations
+        cursor.execute(*sql_table.update(
+                [sql_table.warehouse_input],
+                location.select(
+                    location.input_location,
+                    where=location.id == sql_table.warehouse),
+                where=sql_table.warehouse_input == Null))
+        cursor.execute(*sql_table.update(
+                [sql_table.warehouse_storage],
+                location.select(
+                    location.storage_location,
+                    where=location.id == sql_table.warehouse),
+                where=sql_table.warehouse_storage == Null))
+
     @classmethod
     def order_number(cls, tables):
         table, _ = tables[None]
         return [CharLength(table.number), table.number]
 
     @classmethod
     def order_effective_date(cls, tables):
@@ -320,74 +376,55 @@
         return 'draft'
 
     @classmethod
     def default_warehouse(cls):
         Location = Pool().get('stock.location')
         return Location.get_default_warehouse()
 
+    @fields.depends('warehouse')
+    def on_change_warehouse(self):
+        if self.warehouse:
+            self.warehouse_input = self.warehouse.input_location
+            self.warehouse_storage = self.warehouse.storage_location
+        else:
+            self.warehouse_input = self.warehouse_storage = None
+
     @staticmethod
     def default_company():
         return Transaction().context.get('company')
 
     @fields.depends('supplier')
     def on_change_supplier(self):
         self.contact_address = None
         if self.supplier:
             self.contact_address = self.supplier.address_get()
 
     @fields.depends('supplier')
     def on_change_with_supplier_location(self, name=None):
-        if self.supplier and self.supplier.supplier_location:
-            return self.supplier.supplier_location.id
-
-    @classmethod
-    def default_warehouse_input(cls):
-        warehouse = cls.default_warehouse()
-        if warehouse:
-            return cls(warehouse=warehouse).on_change_with_warehouse_input()
-
-    @fields.depends('warehouse')
-    def on_change_with_warehouse_input(self, name=None):
-        if self.warehouse:
-            return self.warehouse.input_location.id
-
-    @classmethod
-    def default_warehouse_storage(cls):
-        warehouse = cls.default_warehouse()
-        if warehouse:
-            return cls(warehouse=warehouse).on_change_with_warehouse_storage()
-
-    @fields.depends('warehouse')
-    def on_change_with_warehouse_storage(self, name=None):
-        if self.warehouse:
-            return self.warehouse.storage_location.id
+        return self.supplier.supplier_location if self.supplier else None
 
     def get_incoming_moves(self, name):
-        moves = []
+        moves = sort(self.moves, self.__class__.incoming_moves.order)
         if self.warehouse_input == self.warehouse_storage:
-            return [m.id for m in self.moves]
-        for move in self.moves:
-            if move.to_location == self.warehouse_input:
-                moves.append(move.id)
-        return moves
+            return [m.id for m in moves]
+        else:
+            return [
+                m.id for m in moves if m.to_location == self.warehouse_input]
 
     @classmethod
     def set_incoming_moves(cls, shipments, name, value):
         if not value:
             return
         cls.write(shipments, {
                 'moves': value,
                 })
 
     def get_inventory_moves(self, name):
-        moves = []
-        for move in self.moves:
-            if move.from_location == self.warehouse_input:
-                moves.append(move.id)
-        return moves
+        moves = sort(self.moves, self.__class__.inventory_moves.order)
+        return [m.id for m in moves if m.from_location == self.warehouse_input]
 
     @classmethod
     def set_inventory_moves(cls, shipments, name, value):
         if not value:
             return
         cls.write(shipments, {
                 'moves': value,
@@ -459,16 +496,14 @@
 
     @classmethod
     def copy(cls, shipments, default=None):
         if default is None:
             default = {}
         else:
             default = default.copy()
-        default.setdefault('inventory_moves', None)
-        default.setdefault('incoming_moves', None)
         default.setdefault('number', None)
         default.setdefault('received_by', None)
         default.setdefault('done_by', None)
         return super(ShipmentIn, cls).copy(shipments, default=default)
 
     def _get_inventory_move(self, incoming_move):
         'Return inventory move for the incoming move'
@@ -659,14 +694,19 @@
                             [Eval('from_location', -1)], 'parent'),
                         ('to_location', 'child_of',
                             [Eval('to_location', -1)], 'parent'),
                         ],
                     [])),
             ('company', '=', Eval('company')),
             ],
+        order=[
+            ('from_location', 'ASC'),
+            ('product', 'ASC'),
+            ('id', 'ASC'),
+            ],
         help="The moves that return the stock to the supplier.")
     origins = fields.Function(fields.Char('Origins'), 'get_origins')
     assigned_by = employee_field("Assigned By")
     done_by = employee_field("Done By")
     state = fields.Selection([
         ('draft', 'Draft'),
         ('waiting', 'Waiting'),
@@ -775,16 +815,15 @@
     def on_change_supplier(self):
         if self.supplier:
             self.delivery_address = self.supplier.address_get('delivery')
             self.to_location = self.supplier.supplier_location
 
     @fields.depends('from_location')
     def on_change_with_warehouse(self, name=None):
-        if self.from_location and self.from_location.warehouse:
-            return self.from_location.warehouse.id
+        return self.from_location.warehouse if self.from_location else None
 
     @property
     def _move_planned_date(self):
         '''
         Return the planned date for the moves
         '''
         return self.planned_date
@@ -943,15 +982,25 @@
                 _with_childs = True
             else:
                 _with_childs = with_childs
             if not Move.assign_try(moves, with_childs=_with_childs):
                 success = False
         if success:
             cls.assign(shipments)
-        return success
+        else:
+            to_assign = []
+            for shipment in shipments:
+                if any(
+                        m.state in {'staging', 'draft'}
+                        for m in shipment.assign_moves
+                        if m.assignation_required):
+                    continue
+                to_assign.append(shipment)
+            if to_assign:
+                cls.assign(to_assign)
 
     @classmethod
     def _get_reschedule_domain(cls, date):
         return [
             ('state', '=', 'waiting'),
             ('planned_date', '<', date),
             ]
@@ -1022,25 +1071,52 @@
         help="The customer's identifier for the shipment.")
     warehouse = fields.Many2One('stock.location', "Warehouse", required=True,
         states={
             'readonly': ((Eval('state') != 'draft')
                 | Eval('outgoing_moves', [0]) | Eval('inventory_moves', [0])),
             }, domain=[('type', '=', 'warehouse')],
         help="Where the stock is sent from.")
-    warehouse_storage = fields.Function(fields.Many2One('stock.location',
-            'Warehouse Storage'), 'on_change_with_warehouse_storage')
-    warehouse_output = fields.Function(fields.Many2One('stock.location',
-            'Warehouse Output'), 'on_change_with_warehouse_output')
+    warehouse_storage = fields.Many2One(
+        'stock.location', "Warehouse Storage", required=True,
+        domain=[
+            ('type', '=', 'storage'),
+            If(Eval('state') == 'draft',
+                ('parent', 'child_of', [Eval('warehouse', -1)]),
+                ()),
+            ],
+        states={
+            'readonly': Eval('state') != 'draft',
+            })
+    warehouse_output = fields.Many2One(
+        'stock.location', "Warehouse Output", required=True,
+        domain=[
+            ('type', '=', 'storage'),
+            If(Eval('state') == 'draft',
+                ('parent', 'child_of', [Eval('warehouse', -1)]),
+                ()),
+            ],
+        states={
+            'readonly': Eval('state') != 'draft',
+            })
     outgoing_moves = fields.Function(fields.One2Many('stock.move', 'shipment',
             'Outgoing Moves',
             domain=[
-                ('from_location', '=', Eval('warehouse_output')),
-                ('to_location', '=', Eval('customer_location')),
+                If(Eval('warehouse_output') == Eval('warehouse_storage'),
+                    ('from_location', 'child_of',
+                        [Eval('warehouse_output', -1)], 'parent'),
+                    ('from_location', '=', Eval('warehouse_output'))),
+                If(~Eval('state').in_(['done', 'cancelled']),
+                    ('to_location', '=', Eval('customer_location')),
+                    ()),
                 ('company', '=', Eval('company')),
                 ],
+            order=[
+                ('product', 'ASC'),
+                ('id', 'ASC'),
+                ],
             states={
                 'readonly': (Eval('state').in_(
                         If(Eval('warehouse_storage')
                             == Eval('warehouse_output'),
                             ['done', 'cancelled'],
                             ['waiting', 'packed', 'done', 'cancelled'],
                             ))
@@ -1054,14 +1130,19 @@
                 If(Eval('state').in_(['waiting']),
                     ('from_location', 'child_of',
                         [Eval('warehouse_storage', -1)], 'parent'),
                     ()),
                 ('to_location', '=', Eval('warehouse_output')),
                 ('company', '=', Eval('company')),
                 ],
+            order=[
+                ('from_location', 'ASC'),
+                ('product', 'ASC'),
+                ('id', 'ASC'),
+                ],
             states={
                 'readonly': Eval('state').in_(
                     ['draft', 'assigned', 'packed', 'done', 'cancelled']),
                 'invisible': (
                     Eval('warehouse_storage') == Eval('warehouse_output')),
                 },
             help="The moves that pick the stock from the storage area."),
@@ -1182,17 +1263,20 @@
                     },
                 'assign_try': {},
                 'assign_force': {},
                 })
 
     @classmethod
     def __register__(cls, module_name):
+        pool = Pool()
+        Location = pool.get('stock.location')
         cursor = Transaction().connection.cursor()
         table = cls.__table_handler__(module_name)
         sql_table = cls.__table__()
+        location = Location.__table__()
 
         # Migration from 3.8: rename code into number
         if table.column_exist('code'):
             table.column_rename('code', 'number')
 
         # Migration from 5.6: rename assigned_by into picked_by
         if table.column_exist('assigned_by'):
@@ -1201,14 +1285,28 @@
         super(ShipmentOut, cls).__register__(module_name)
 
         # Migration from 5.6: rename state cancel to cancelled
         cursor.execute(*sql_table.update(
                 [sql_table.state], ['cancelled'],
                 where=sql_table.state == 'cancel'))
 
+        # Migration from 6.6: fill warehouse locations
+        cursor.execute(*sql_table.update(
+                [sql_table.warehouse_storage],
+                location.select(
+                    location.storage_location,
+                    where=location.id == sql_table.warehouse),
+                where=sql_table.warehouse_storage == Null))
+        cursor.execute(*sql_table.update(
+                [sql_table.warehouse_output],
+                location.select(
+                    location.output_location,
+                    where=location.id == sql_table.warehouse),
+                where=sql_table.warehouse_output == Null))
+
     @classmethod
     def order_number(cls, tables):
         table, _ = tables[None]
         return [CharLength(table.number), table.number]
 
     @classmethod
     def order_effective_date(cls, tables):
@@ -1224,75 +1322,58 @@
         Location = Pool().get('stock.location')
         return Location.get_default_warehouse()
 
     @staticmethod
     def default_company():
         return Transaction().context.get('company')
 
+    @fields.depends('warehouse')
+    def on_change_warehouse(self):
+        if self.warehouse:
+            if self.warehouse.picking_location:
+                self.warehouse_storage = self.warehouse.picking_location
+            else:
+                self.warehouse_storage = self.warehouse.storage_location
+            self.warehouse_output = self.warehouse.output_location
+        else:
+            self.warehouse_storage = self.warehouse_output = None
+
     @fields.depends('customer', 'warehouse')
     def on_change_customer(self):
         self.delivery_address = None
         if self.customer:
             with Transaction().set_context(
                     warehouse=self.warehouse.id if self.warehouse else None):
                 self.delivery_address = self.customer.address_get(
                     type='delivery')
 
     @fields.depends('customer')
     def on_change_with_customer_location(self, name=None):
-        if self.customer:
-            return self.customer.customer_location.id
-
-    @classmethod
-    def default_warehouse_storage(cls):
-        warehouse = cls.default_warehouse()
-        if warehouse:
-            return cls(warehouse=warehouse).on_change_with_warehouse_storage()
-
-    @fields.depends('warehouse')
-    def on_change_with_warehouse_storage(self, name=None):
-        if self.warehouse:
-            if self.warehouse.picking_location:
-                location = self.warehouse.picking_location
-            else:
-                location = self.warehouse.storage_location
-            return location.id
-
-    @classmethod
-    def default_warehouse_output(cls):
-        warehouse = cls.default_warehouse()
-        if warehouse:
-            return cls(warehouse=warehouse).on_change_with_warehouse_output()
-
-    @fields.depends('warehouse')
-    def on_change_with_warehouse_output(self, name=None):
-        if self.warehouse:
-            return self.warehouse.output_location.id
+        return self.customer.customer_location if self.customer else None
 
     def get_outgoing_moves(self, name):
-        moves = []
-        for move in self.moves:
-            if move.from_location == self.warehouse_output:
-                moves.append(move.id)
-        return moves
+        moves = sort(self.moves, self.__class__.outgoing_moves.order)
+        if self.warehouse_output == self.warehouse_storage:
+            return [m.id for m in moves]
+        else:
+            return [
+                m.id for m in moves
+                if m.from_location == self.warehouse_output]
 
     @classmethod
     def set_outgoing_moves(cls, shipments, name, value):
         if not value:
             return
         cls.write(shipments, {
                 'moves': value,
                 })
 
     def get_inventory_moves(self, name):
-        moves = []
-        for move in self.moves:
-            if move.to_location == self.warehouse_output:
-                moves.append(move.id)
-        return moves
+        moves = sort(self.moves, self.__class__.inventory_moves.order)
+        return [m.id for m in moves if m.to_location == self.warehouse_output]
 
     @classmethod
     def set_inventory_moves(cls, shipments, name, value):
         if not value:
             return
         cls.write(shipments, {
                 'moves': value,
@@ -1582,16 +1663,14 @@
 
     @classmethod
     def copy(cls, shipments, default=None):
         if default is None:
             default = {}
         else:
             default = default.copy()
-        default.setdefault('inventory_moves', None)
-        default.setdefault('outgoing_moves', None)
         default.setdefault('number', None)
         default.setdefault('picked_by', None)
         default.setdefault('packed_by', None)
         default.setdefault('done_by', None)
         return super(ShipmentOut, cls).copy(shipments, default=default)
 
     @classmethod
@@ -1634,17 +1713,25 @@
     def assign_try(cls, shipments):
         Move = Pool().get('stock.move')
         to_assign = [
             m for s in shipments for m in s.assign_moves
             if m.assignation_required]
         if Move.assign_try(to_assign):
             cls.assign(shipments)
-            return True
         else:
-            return False
+            to_assign = []
+            for shipment in shipments:
+                if any(
+                        m.state in {'staging', 'draft'}
+                        for m in shipment.assign_moves
+                        if m.assignation_required):
+                    continue
+                to_assign.append(shipment)
+            if to_assign:
+                cls.assign(to_assign)
 
     @classmethod
     def _get_reschedule_domain(cls, date):
         return [
             ('state', '=', 'waiting'),
             ('planned_date', '<', date),
             ]
@@ -1705,28 +1792,52 @@
         help="The customer's identifier for the shipment.")
     warehouse = fields.Many2One('stock.location', "Warehouse", required=True,
         states={
             'readonly': ((Eval('state') != 'draft')
                 | Eval('incoming_moves', [0]) | Eval('inventory_moves', [0])),
             }, domain=[('type', '=', 'warehouse')],
         help="Where the stock is returned.")
-    warehouse_storage = fields.Function(fields.Many2One('stock.location',
-            'Warehouse Storage'), 'on_change_with_warehouse_storage')
-    warehouse_input = fields.Function(fields.Many2One('stock.location',
-            'Warehouse Input'), 'on_change_with_warehouse_input')
+    warehouse_storage = fields.Many2One(
+        'stock.location', "Warehouse Storage", required=True,
+        domain=[
+            ('type', '=', 'storage'),
+            If(Eval('state') == 'draft',
+                ('parent', 'child_of', [Eval('warehouse', -1)]),
+                ()),
+            ],
+        states={
+            'readonly': Eval('state') != 'draft',
+            })
+    warehouse_input = fields.Many2One(
+        'stock.location', "Warehouse Input", required=True,
+        domain=[
+            ('type', '=', 'storage'),
+            If(Eval('state') == 'draft',
+                ('parent', 'child_of', [Eval('warehouse', -1)]),
+                ()),
+            ],
+        states={
+            'readonly': Eval('state') != 'draft',
+            })
     incoming_moves = fields.Function(fields.One2Many('stock.move', 'shipment',
             'Incoming Moves',
             domain=[
-                ('from_location', '=', Eval('customer_location')),
+                If(Eval('state') == 'draft',
+                    ('from_location', '=', Eval('customer_location')),
+                    ()),
                 If(Eval('warehouse_input') == Eval('warehouse_storage'),
                     ('to_location', 'child_of',
                         [Eval('warehouse_input', -1)], 'parent'),
                     ('to_location', '=', Eval('warehouse_input'))),
                 ('company', '=', Eval('company')),
                 ],
+            order=[
+                ('product', 'ASC'),
+                ('id', 'ASC'),
+                ],
             states={
                 'readonly': ((Eval('state') != 'draft')
                     | ~Eval('warehouse') | ~Eval('customer')),
                 },
             help="The moves that bring the stock into the warehouse."),
         'get_incoming_moves', setter='set_incoming_moves')
     inventory_moves = fields.Function(fields.One2Many('stock.move', 'shipment',
@@ -1739,14 +1850,19 @@
                             [Eval('warehouse_storage', -1)], 'parent'),
                         ('to_location.waste_warehouses', '=',
                             Eval('warehouse')),
                         ],
                     []),
                 ('company', '=', Eval('company')),
                 ],
+            order=[
+                ('to_location', 'ASC'),
+                ('product', 'ASC'),
+                ('id', 'ASC'),
+                ],
             states={
                 'readonly': Eval('state').in_(['draft', 'cancelled', 'done']),
                 'invisible': (
                     Eval('warehouse_input') == Eval('warehouse_storage')),
                 },
             help="The moves that put the stock away into the storage area."),
         'get_inventory_moves', setter='set_inventory_moves')
@@ -1808,17 +1924,20 @@
                     'invisible': Eval('state') != 'received',
                     'depends': ['state'],
                     },
                 })
 
     @classmethod
     def __register__(cls, module_name):
+        pool = Pool()
+        Location = pool.get('stock.location')
         cursor = Transaction().connection.cursor()
         table = cls.__table_handler__(module_name)
         sql_table = cls.__table__()
+        location = Location.__table__()
 
         # Migration from 3.8: rename code into number
         if table.column_exist('code'):
             table.column_rename('code', 'number')
 
         # Migration from 6.4: rename delivery_address to contact_address
         table.column_rename('delivery_address', 'contact_address')
@@ -1829,14 +1948,28 @@
         cursor.execute(*sql_table.update(
                 [sql_table.state], ['cancelled'],
                 where=sql_table.state == 'cancel'))
 
         # Migration from 6.4: remove required on contact_address
         table.not_null_action('contact_address', 'remove')
 
+        # Migration from 6.6: fill warehouse locations
+        cursor.execute(*sql_table.update(
+                [sql_table.warehouse_input],
+                location.select(
+                    location.input_location,
+                    where=location.id == sql_table.warehouse),
+                where=sql_table.warehouse_input == Null))
+        cursor.execute(*sql_table.update(
+                [sql_table.warehouse_storage],
+                location.select(
+                    location.storage_location,
+                    where=location.id == sql_table.warehouse),
+                where=sql_table.warehouse_storage == Null))
+
     @classmethod
     def order_number(cls, tables):
         table, _ = tables[None]
         return [CharLength(table.number), table.number]
 
     @classmethod
     def order_effective_date(cls, tables):
@@ -1848,74 +1981,56 @@
         return 'draft'
 
     @classmethod
     def default_warehouse(cls):
         Location = Pool().get('stock.location')
         return Location.get_default_warehouse()
 
+    @fields.depends('warehouse')
+    def on_change_warehouse(self):
+        if self.warehouse:
+            self.warehouse_input = self.warehouse.input_location
+            self.warehouse_storage = self.warehouse.storage_location
+        else:
+            self.warehouse_input = self.warehouse_storage = None
+
     @staticmethod
     def default_company():
         return Transaction().context.get('company')
 
     @fields.depends('customer')
     def on_change_customer(self):
         self.contact_address = None
         if self.customer:
             self.contact_address = self.customer.address_get()
 
     @fields.depends('customer')
     def on_change_with_customer_location(self, name=None):
-        if self.customer:
-            return self.customer.customer_location.id
-
-    @classmethod
-    def default_warehouse_storage(cls):
-        warehouse = cls.default_warehouse()
-        if warehouse:
-            return cls(warehouse=warehouse).on_change_with_warehouse_storage()
-
-    @fields.depends('warehouse')
-    def on_change_with_warehouse_storage(self, name=None):
-        if self.warehouse:
-            return self.warehouse.storage_location.id
-
-    @classmethod
-    def default_warehouse_input(cls):
-        warehouse = cls.default_warehouse()
-        if warehouse:
-            return cls(warehouse=warehouse).on_change_with_warehouse_input()
-
-    @fields.depends('warehouse')
-    def on_change_with_warehouse_input(self, name=None):
-        if self.warehouse:
-            return self.warehouse.input_location.id
+        return self.customer.customer_location if self.customer else None
 
     def get_incoming_moves(self, name):
-        moves = []
+        moves = sort(self.moves, self.__class__.incoming_moves.order)
         if self.warehouse_input == self.warehouse_storage:
-            return [m.id for m in self.moves]
-        for move in self.moves:
-            if move.to_location == self.warehouse_input:
-                moves.append(move.id)
-        return moves
+            return [m.id for m in moves]
+        else:
+            return [
+                m.id for m in moves
+                if m.to_location == self.warehouse_input]
 
     @classmethod
     def set_incoming_moves(cls, shipments, name, value):
         if not value:
             return
         cls.write(shipments, {
                 'moves': value,
                 })
 
     def get_inventory_moves(self, name):
-        moves = []
-        for move in self.moves:
-            if move.from_location == self.warehouse_input:
-                moves.append(move.id)
-        return moves
+        moves = sort(self.moves, self.__class__.inventory_moves.order)
+        return [m.id for m in moves if m.from_location == self.warehouse_input]
 
     @classmethod
     def set_inventory_moves(cls, shipments, name, value):
         if not value:
             return
         cls.write(shipments, {
                 'moves': value,
@@ -1981,16 +2096,14 @@
         cls._set_move_planned_date(sum(args[::2], []))
 
     @classmethod
     def copy(cls, shipments, default=None):
         if default is None:
             default = {}
         default = default.copy()
-        default.setdefault('inventory_moves', None)
-        default.setdefault('incoming_moves', None)
         default.setdefault('number', None)
         default.setdefault('received_by', None)
         default.setdefault('done_by', None)
         return super(ShipmentOutReturn, cls).copy(shipments, default=default)
 
     @classmethod
     def delete(cls, shipments):
@@ -2205,28 +2318,38 @@
                                 ('to_location', 'child_of',
                                     [Eval('to_location', -1)], 'parent'),
                                 ],
                             ]),
                     [])),
             ('company', '=', Eval('company')),
             ],
+        order=[
+            ('from_location', 'ASC'),
+            ('product', 'ASC'),
+            ('id', 'ASC'),
+            ],
         help="The moves that perform the shipment.")
     outgoing_moves = fields.Function(fields.One2Many('stock.move', 'shipment',
             'Outgoing Moves',
             domain=[
                 If(Eval('state').in_(['request', 'draft']), [
                         ('from_location', 'child_of',
                             [Eval('from_location', -1)], 'parent'),
                         If(~Eval('transit_location'),
                             ('to_location', 'child_of',
                                 [Eval('to_location', -1)], 'parent'),
                             ('to_location', '=', Eval('transit_location'))),
                         ],
                     []),
                 ],
+            order=[
+                ('from_location', 'ASC'),
+                ('product', 'ASC'),
+                ('id', 'ASC'),
+                ],
             states={
                 'readonly': Eval('state').in_(
                     ['assigned', 'shipped', 'done', 'cancelled']),
                 'invisible': (~Eval('transit_location')
                     | Eval('state').in_(['request', 'draft'])),
                 },
             help="The moves that send the stock out."),
@@ -2240,14 +2363,19 @@
                                 [Eval('from_location', -1)], 'parent'),
                             ('from_location', '=', Eval('transit_location'))),
                         ('to_location', 'child_of',
                             [Eval('to_location', -1)], 'parent'),
                         ],
                     []),
                 ],
+            order=[
+                ('to_location', 'ASC'),
+                ('product', 'ASC'),
+                ('id', 'ASC'),
+                ],
             states={
                 'readonly': Eval('state').in_(['done', 'cancelled']),
                 'invisible': (~Eval('transit_location')
                     | Eval('state').in_(['request', 'draft'])),
                 },
             help="The moves that receive the stock in."),
         'get_incoming_moves', setter='set_moves')
@@ -2398,20 +2526,19 @@
         if (self.from_location
                 and self.to_location
                 and self.from_location.warehouse != self.to_location.warehouse
                 and self.from_location.warehouse
                 and self.to_location.warehouse):
             return Config(1).get_multivalue(
                 'shipment_internal_transit',
-                company=self.company.id if self.company else None).id
+                company=self.company.id if self.company else None)
 
     @fields.depends('from_location')
     def on_change_with_warehouse(self, name=None):
-        if self.from_location and self.from_location.warehouse:
-            return self.from_location.warehouse.id
+        return self.from_location.warehouse if self.from_location else None
 
     @fields.depends(
         'planned_date', 'from_location', 'to_location',
         methods=['on_change_with_transit_location'])
     def on_change_with_planned_start_date(self, pattern=None):
         pool = Pool()
         LocationLeadTime = pool.get('stock.location.lead_time')
@@ -2429,30 +2556,29 @@
                 else None)
             lead_time = LocationLeadTime.get_lead_time(pattern)
             if lead_time:
                 return self.planned_date - lead_time
         return self.planned_date
 
     def get_outgoing_moves(self, name):
+        moves = sort(self.moves, self.__class__.outgoing_moves.order)
         if not self.transit_location:
-            return [m.id for m in self.moves]
-        moves = []
-        for move in self.moves:
-            if move.to_location == self.transit_location:
-                moves.append(move.id)
-        return moves
+            return [m.id for m in moves]
+        else:
+            return [
+                m.id for m in moves if m.to_location == self.transit_location]
 
     def get_incoming_moves(self, name):
+        moves = sort(self.moves, self.__class__.incoming_moves.order)
         if not self.transit_location:
-            return [m.id for m in self.moves]
-        moves = []
-        for move in self.moves:
-            if move.from_location == self.transit_location:
-                moves.append(move.id)
-        return moves
+            return [m.id for m in moves]
+        else:
+            return [
+                m.id for m in moves
+                if m.from_location == self.transit_location]
 
     @classmethod
     def set_moves(cls, shipments, name, value):
         if not value:
             return
         cls.write(shipments, {
                 'moves': value,
@@ -2733,19 +2859,27 @@
     @dualmethod
     @ModelView.button
     def assign_try(cls, shipments):
         Move = Pool().get('stock.move')
         to_assign = [
             m for s in shipments for m in s.assign_moves
             if m.assignation_required]
-        if not to_assign or Move.assign_try(to_assign):
+        if Move.assign_try(to_assign):
             cls.assign(shipments)
-            return True
         else:
-            return False
+            to_assign = []
+            for shipment in shipments:
+                if any(
+                        m.state in {'staging', 'draft'}
+                        for m in shipment.assign_moves
+                        if m.assignation_required):
+                    continue
+                to_assign.append(shipment)
+            if to_assign:
+                cls.assign(to_assign)
 
     @property
     def _move_planned_date(self):
         '''
         Return the planned date for incoming moves and inventory_moves
         '''
         return self.planned_start_date, self.planned_date
@@ -2830,15 +2964,16 @@
                 }),
             ])
     cancel = StateTransition()
     force = StateTransition()
     ignore = StateTransition()
 
     def transition_start(self):
-        if self.record.assign_try():
+        self.record.assign_try()
+        if self.record.state == 'assigned':
             return 'end'
         else:
             return 'partial'
 
     def default_partial(self, fields):
         values = {}
         if 'moves' in fields:
@@ -2852,15 +2987,15 @@
         return 'end'
 
     def transition_force(self):
         self.record.assign_force()
         return 'end'
 
     def transition_ignore(self):
-        self.record.assign_ignore()
+        self.record.assign_ignore(self.partial.moves)
         return 'end'
 
 
 class AssignPartial(ModelView):
     "Assign Shipment"
     __name__ = 'stock.shipment.assign.partial'
     moves = fields.Many2Many(
@@ -2886,91 +3021,89 @@
             return super(ShipmentReport, cls).execute(ids, data)
 
     @classmethod
     def moves(cls, shipment):
         raise NotImplementedError
 
     @classmethod
+    def moves_order(cls, shipment):
+        return []
+
+    @classmethod
     def get_context(cls, shipments, header, data):
         report_context = super().get_context(shipments, header, data)
-
-        compare_context = cls.get_compare_context(shipments, data)
-        sorted_moves = {}
-        for shipment in shipments:
-            sorted_moves[shipment.id] = sorted(
-                cls.moves(shipment),
-                key=functools.partial(cls.get_compare_key, compare_context))
-        report_context['moves'] = sorted_moves
-
+        report_context['moves'] = cls.moves
         return report_context
 
-    @classmethod
-    def get_compare_context(cls, shipments, data):
-        from_location_ids = set()
-        to_location_ids = set()
-        for shipment in shipments:
-            for move in cls.moves(shipment):
-                from_location_ids.add(move.from_location.id)
-                to_location_ids.add(move.to_location.id)
-
-        return {
-            'from_location_ids': list(from_location_ids),
-            'to_location_ids': list(to_location_ids),
-            }
-
-    @staticmethod
-    def get_compare_key(compare_context, move):
-        from_location_ids = compare_context['from_location_ids']
-        to_location_ids = compare_context['to_location_ids']
-        return [from_location_ids.index(move.from_location.id),
-                to_location_ids.index(move.to_location.id)]
-
 
 class PickingList(ShipmentReport):
     'Picking List'
     __name__ = 'stock.shipment.out.picking_list'
 
     @classmethod
     def moves(cls, shipment):
         if shipment.warehouse_storage == shipment.warehouse_output:
-            return shipment.outgoing_moves
+            moves = shipment.outgoing_moves
         else:
-            return shipment.inventory_moves
+            moves = shipment.inventory_moves
+        return sort(moves, cls.moves_order(shipment))
+
+    @classmethod
+    def moves_order(cls, shipment):
+        return shipment.__class__.inventory_moves.order
 
 
 class SupplierRestockingList(ShipmentReport):
     'Supplier Restocking List'
     __name__ = 'stock.shipment.in.restocking_list'
 
     @classmethod
     def moves(cls, shipment):
         if shipment.warehouse_input == shipment.warehouse_storage:
-            return shipment.incoming_moves
+            moves = shipment.incoming_moves
         else:
-            return shipment.inventory_moves
+            moves = shipment.inventory_moves
+        return sort(moves, cls.moves_order(shipment))
+
+    @classmethod
+    def moves_order(cls, shipment):
+        return shipment.__class__.inventory_moves.order
 
 
 class CustomerReturnRestockingList(ShipmentReport):
     'Customer Return Restocking List'
     __name__ = 'stock.shipment.out.return.restocking_list'
 
     @classmethod
     def moves(cls, shipment):
         if shipment.warehouse_input == shipment.warehouse_storage:
-            return shipment.incoming_moves
+            moves = shipment.incoming_moves
         else:
-            return shipment.inventory_moves
+            moves = shipment.inventory_moves
+        return sort(moves, cls.moves_order(shipment))
+
+    @classmethod
+    def moves_order(cls, shipment):
+        return shipment.__class__.inventory_moves.order
 
 
 class InteralShipmentReport(ShipmentReport):
     'Interal Shipment Report'
     __name__ = 'stock.shipment.internal.report'
 
     @classmethod
     def moves(cls, shipment):
         if shipment.transit_location:
             if shipment.state == 'shipped':
-                return shipment.incoming_moves
+                moves = shipment.incoming_moves
             else:
-                return shipment.outgoing_moves
+                moves = shipment.outgoing_moves
+        else:
+            moves = shipment.moves
+        return sort(moves, cls.moves_order(shipment))
+
+    @classmethod
+    def moves_order(cls, shipment):
+        if shipment.state == 'shipped':
+            return shipment.__class__.incoming_moves.order
         else:
-            return shipment.moves
+            return shipment.__class__.outgoing_moves.order
```

### Comparing `trytond_stock-6.6.3/shipment.xml` & `trytond_stock-6.8.0/shipment.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.6.3/stock.xml` & `trytond_stock-6.8.0/stock.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.6.3/stock_reporting_margin.py` & `trytond_stock-6.8.0/stock_reporting_margin.py`

 * *Files 3% similar despite different names*

```diff
@@ -409,14 +409,18 @@
         template = tables['move.product.template']
         return super()._group_by(tables, withs) + [
             move.product, template.default_uom]
 
     def get_rec_name(self, name):
         return self.product.rec_name
 
+    @classmethod
+    def search_rec_name(cls, name, clause):
+        return [('product.rec_name', *clause[1:])]
+
     def get_quantity(self, name):
         return self.unit.round(self.internal_quantity)
 
 
 class Product(ProductMixin, Abstract, ModelView):
     "Stock Reporting Margin per Product"
     __name__ = 'stock.reporting.margin.product'
@@ -496,14 +500,18 @@
         where = super()._where(tables, withs)
         where &= template_category.category != Null
         return where
 
     def get_rec_name(self, name):
         return self.category.rec_name if self.category else None
 
+    @classmethod
+    def search_rec_name(cls, name, clause):
+        return [('category.rec_name', *clause[1:])]
+
 
 class Category(CategoryMixin, Abstract, ModelView):
     "Stock Reporting Margin per Category"
     __name__ = 'stock.reporting.margin.category'
 
     time_series = fields.One2Many(
         'stock.reporting.margin.category.time_series', 'category',
@@ -525,15 +533,16 @@
     __name__ = 'stock.reporting.margin.category.time_series'
 
 
 class CategoryTree(ModelSQL, ModelView):
     "Stock Reporting Margin per Category"
     __name__ = 'stock.reporting.margin.category.tree'
 
-    name = fields.Function(fields.Char("Name"), 'get_name')
+    name = fields.Function(
+        fields.Char("Name"), 'get_name', searcher='search_name')
     parent = fields.Many2One('stock.reporting.margin.category.tree', "Parent")
     children = fields.One2Many(
         'stock.reporting.margin.category.tree', 'parent', "Children")
     cost = fields.Function(Monetary(
             lazy_gettext('stock.msg_stock_reporting_cost'),
             currency='currency', digits='currency'),
         'get_total')
@@ -570,14 +579,20 @@
     def get_name(cls, categories, name):
         pool = Pool()
         Category = pool.get('product.category')
         categories = Category.browse(categories)
         return {c.id: c.name for c in categories}
 
     @classmethod
+    def search_name(cls, name, clause):
+        pool = Pool()
+        Category = pool.get('product.category')
+        return [('id', 'in', Category.search([clause], query=True))]
+
+    @classmethod
     def order_name(cls, tables):
         pool = Pool()
         Category = pool.get('product.category')
         table, _ = tables[None]
         if 'category' not in tables:
             category = Category.__table__()
             tables['category'] = {
```

### Comparing `trytond_stock-6.6.3/stock_reporting_margin.xml` & `trytond_stock-6.8.0/stock_reporting_margin.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.6.3/supplier_restocking_list.fodt` & `trytond_stock-6.8.0/supplier_restocking_list.fodt`

 * *Files 0% similar despite different names*

#### Comparing `trytond_stock-6.6.3/supplier_restocking_list.fodt` & `trytond_stock-6.8.0/supplier_restocking_list.fodt`

```diff
@@ -511,15 +511,15 @@
               <text:p text:style-name="P9">Quantity</text:p>
             </table:table-cell>
           </table:table-row>
         </table:table-header-rows>
         <table:table-row>
           <table:table-cell table:style-name="Table1.A4" table:number-columns-spanned="2" office:value-type="string">
             <text:p text:style-name="Table_20_Contents">
-              <text:placeholder text:placeholder-type="text">&lt;for each=&quot;move in moves[shipment.id]&quot;&gt;</text:placeholder>
+              <text:placeholder text:placeholder-type="text">&lt;for each=&quot;move in moves(shipment)&quot;&gt;</text:placeholder>
             </text:p>
           </table:table-cell>
           <table:covered-table-cell/>
           <table:table-cell table:style-name="Table1.C4" office:value-type="string">
             <text:p text:style-name="Table_20_Contents"/>
           </table:table-cell>
           <table:table-cell table:style-name="Table1.D4" office:value-type="string">
```

### Comparing `trytond_stock-6.6.3/tests/scenario_stock_average_cost_price.rst` & `trytond_stock-6.8.0/tests/scenario_stock_average_cost_price.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 ========================
 Stock Average Cost Price
 ========================
 
 Imports::
 
-    >>> import datetime
-    >>> from dateutil.relativedelta import relativedelta
+    >>> import datetime as dt
     >>> from decimal import Decimal
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
-    >>> today = datetime.date.today()
+
+    >>> today = dt.date.today()
+    >>> next_day = today + dt.timedelta(days=1)
 
 Activate modules::
 
     >>> config = activate_modules('stock')
 
 Create company::
 
@@ -143,25 +144,25 @@
     >>> product.cost_price
     Decimal('175.0000')
 
 Reduce Cost Price by 80%, to force to write recomputed price later::
 
     >>> modify_cost_price = Wizard('product.modify_cost_price', [product])
     >>> modify_cost_price.form.cost_price = 'cost_price * 0.8'
-    >>> modify_cost_price.form.date = today + datetime.timedelta(days=1)
+    >>> modify_cost_price.form.date = next_day
     >>> modify_cost_price.execute('modify')
     >>> product.cost_price
     Decimal('140.0000')
 
 Increase Cost Price by 10% using Template wizard::
 
     >>> modify_cost_price = Wizard(
     ...     'product.modify_cost_price', [product.template])
     >>> modify_cost_price.form.cost_price = 'cost_price * 1.1'
-    >>> modify_cost_price.form.date = today + datetime.timedelta(days=1)
+    >>> modify_cost_price.form.date = next_day
     >>> modify_cost_price.execute('modify')
     >>> product.reload()
     >>> product.cost_price
     Decimal('154.0000')
 
 Send one product we don't have in stock::
```

### Comparing `trytond_stock-6.6.3/tests/scenario_stock_inventory.rst` & `trytond_stock-6.8.0/tests/scenario_stock_inventory.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ========================
 Stock Inventory Scenario
 ========================
 
 Imports::
 
-    >>> import datetime
-    >>> from dateutil.relativedelta import relativedelta
+    >>> import datetime as dt
     >>> from decimal import Decimal
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
-    >>> today = datetime.date.today()
+
+    >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('stock')
 
 Create company::
```

### Comparing `trytond_stock-6.6.3/tests/scenario_stock_inventory_count.rst` & `trytond_stock-6.8.0/tests/scenario_stock_inventory_count.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 ==============================
 Stock Inventory Count Scenario
 ==============================
 
 Imports::
 
-    >>> import datetime
-    >>> from dateutil.relativedelta import relativedelta
     >>> from decimal import Decimal
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
-    >>> today = datetime.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('stock')
 
 Create company::
 
@@ -64,16 +61,15 @@
     >>> inventory = Inventory()
     >>> inventory.location = storage_loc
     >>> inventory.empty_quantity = 'keep'
     >>> inventory.save()
 
 Count inventory::
 
-    >>> _ = inventory.click('do_count')
-    >>> count = Wizard('stock.inventory.count', [inventory])
+    >>> count = inventory.click('do_count')
 
     >>> count.form.search = product
 
     >>> count.execute('quantity')  # doctest: +IGNORE_EXCEPTION_DETAIL
     Traceback (most recent call last):
         ...
     InventoryCountWarning: ...
```

### Comparing `trytond_stock-6.6.3/tests/scenario_stock_inventory_empty_quantity.rst` & `trytond_stock-6.8.0/tests/scenario_stock_inventory_empty_quantity.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 =======================================
 Stock Inventory Scenario Empty Quantity
 =======================================
 
 Imports::
 
-    >>> import datetime
-    >>> from dateutil.relativedelta import relativedelta
+    >>> import datetime as dt
     >>> from decimal import Decimal
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
-    >>> today = datetime.date.today()
+
+    >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('stock')
 
 Create company::
```

### Comparing `trytond_stock-6.6.3/tests/scenario_stock_move_in_future.rst` & `trytond_stock-6.8.0/tests/scenario_stock_move_in_future.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 =============================
 Stock Move In Future Scenario
 =============================
 
 Imports::
 
-    >>> import datetime
-    >>> from dateutil.relativedelta import relativedelta
+    >>> import datetime as dt
     >>> from decimal import Decimal
     >>> from proteus import Model
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import (
     ...     create_company, get_company)
-    >>> today = datetime.date.today()
-    >>> tomorrow = today + relativedelta(days=1)
+
+    >>> today = dt.date.today()
+    >>> tomorrow = today + dt.timedelta(days=1)
 
 Activate modules::
 
     >>> config = activate_modules('stock')
 
 Create company::
```

### Comparing `trytond_stock-6.6.3/tests/scenario_stock_product_quantities_by_warehouse.rst` & `trytond_stock-6.8.0/tests/scenario_stock_product_quantities_by_warehouse.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 =====================================
 Stock Product Quantities by Warehouse
 =====================================
 
 Imports::
 
-    >>> import datetime
-    >>> from dateutil.relativedelta import relativedelta
+    >>> import datetime as dt
     >>> from decimal import Decimal
     >>> from proteus import Model, Wizard, Report
     >>> from trytond import backend
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
-    >>> today = datetime.date.today()
-    >>> yesterday = today - relativedelta(days=1)
-    >>> tomorrow = today + relativedelta(days=1)
+
+    >>> today = dt.date.today()
+    >>> yesterday = today - dt.timedelta(days=1)
+    >>> tomorrow = today + dt.timedelta(days=1)
 
 Activate modules::
 
     >>> config = activate_modules('stock')
 
 Create company::
```

### Comparing `trytond_stock-6.6.3/tests/scenario_stock_recompute_average_cost_price.rst` & `trytond_stock-6.8.0/tests/scenario_stock_recompute_average_cost_price.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ==================================
 Stock Recompute Average Cost Price
 ==================================
 
 Imports::
 
     >>> import datetime as dt
-    >>> from dateutil.relativedelta import relativedelta
     >>> from decimal import Decimal
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
+
     >>> today = dt.date.today()
 
 Activate modules::
 
     >>> config = activate_modules('stock')
 
 Create company::
```

### Comparing `trytond_stock-6.6.3/tests/scenario_stock_recompute_average_cost_price_production.rst` & `trytond_stock-6.8.0/tests/scenario_stock_recompute_average_cost_price_production.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.6.3/tests/scenario_stock_reporting.rst` & `trytond_stock-6.8.0/tests/scenario_stock_reporting.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 =================================
 Stock Shipment Reporting Scenario
 =================================
 
 Imports::
 
-    >>> import datetime
-    >>> from dateutil.relativedelta import relativedelta
+    >>> import datetime as dt
     >>> from decimal import Decimal
     >>> from proteus import Model, Wizard, Report
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
-    >>> today = datetime.date.today()
-    >>> yesterday = today - relativedelta(days=1)
+
+    >>> today = dt.date.today()
+    >>> yesterday = today - dt.timedelta(days=1)
 
 Activate modules::
 
     >>> config = activate_modules('stock')
 
 Create company::
 
@@ -108,15 +108,14 @@
     >>> move.to_location = customer_loc
     >>> move.company = company
     >>> move.unit_price = Decimal('1')
     >>> move.currency = company.currency
     >>> shipment_out.save()
     >>> shipment_out.click('wait')
     >>> shipment_out.click('assign_try')
-    True
     >>> shipment_out.click('pick')
     >>> shipment_out.click('pack')
     >>> shipment_out.click('done')
 
 Testing the reports::
 
     >>> delivery_note = Report('stock.shipment.out.delivery_note')
@@ -149,15 +148,14 @@
     >>> move.to_location = lost_loc
     >>> move.company = company
     >>> move.unit_price = Decimal('1')
     >>> move.currency = company.currency
     >>> shipment_internal.save()
     >>> shipment_internal.click('wait')
     >>> shipment_internal.click('assign_try')
-    True
     >>> shipment_internal.click('done')
 
 Testing the report::
 
     >>> internal_report = Report('stock.shipment.internal.report')
     >>> ext, _, _, name = internal_report.execute([shipment_internal], {})
     >>> ext
```

### Comparing `trytond_stock-6.6.3/tests/scenario_stock_reporting_margin.rst` & `trytond_stock-6.8.0/tests/scenario_stock_reporting_margin.rst`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
     >>> import datetime as dt
     >>> from decimal import Decimal
     >>> from proteus import Model
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import (
     ...     create_company, get_company)
+
     >>> today = dt.date.today()
     >>> yesterday = today - dt.timedelta(days=1)
 
 Activate modules::
 
     >>> config = activate_modules('stock')
 
@@ -199,14 +200,17 @@
     ...     ("Root", Decimal('140.00'), Decimal('270.00'),
     ...         Decimal('130.00'), Decimal('0.4815')),
     ...     ("Child1", Decimal('100.00'), Decimal('170.00'),
     ...         Decimal('70.00'), Decimal('0.4118')),
     ...     ('Child2', Decimal('40.00'), Decimal('100.00'),
     ...         Decimal('60.00'), Decimal('0.6000'))])
     True
+    >>> child1, = MarginCategoryTree.find([('rec_name', '=', 'Child1')])
+    >>> child1.rec_name
+    'Child1'
 
 Check reporting margin including lost::
 
     >>> context['include_lost'] = True
 
     >>> with config.set_context(context=context):
     ...     reports = MarginProduct.find([])
```

### Comparing `trytond_stock-6.6.3/tests/scenario_stock_shipment_in_return.rst` & `trytond_stock-6.8.0/tests/scenario_stock_shipment_in_return.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 =================================
 Stock Shipment In Return Scenario
 =================================
 
 Imports::
 
-    >>> import datetime
-    >>> from dateutil.relativedelta import relativedelta
+    >>> import datetime as dt
     >>> from decimal import Decimal
     >>> from proteus import Model
     >>> from trytond.tests.tools import activate_modules
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
-    >>> today = datetime.date.today()
-    >>> yesterday = today - relativedelta(days=1)
+
+    >>> today = dt.date.today()
+    >>> yesterday = today - dt.timedelta(days=1)
 
 Activate modules::
 
     >>> config = activate_modules('stock')
 
 Create company::
```

### Comparing `trytond_stock-6.6.3/tests/scenario_stock_shipment_in_same_storage_input.rst` & `trytond_stock-6.8.0/tests/scenario_stock_shipment_in_same_storage_input.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.6.3/tests/scenario_stock_shipment_internal.rst` & `trytond_stock-6.8.0/tests/scenario_stock_shipment_internal.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 ================================
 Stock Shipment Internal Scenario
 ================================
 
 Imports::
 
-    >>> import datetime
-    >>> from dateutil.relativedelta import relativedelta
+    >>> import datetime as dt
     >>> from decimal import Decimal
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules, set_user
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
-    >>> today = datetime.date.today()
-    >>> yesterday = today - relativedelta(days=1)
-    >>> tomorrow = today + relativedelta(days=1)
+
+    >>> today = dt.date.today()
+    >>> yesterday = today - dt.timedelta(days=1)
+    >>> tomorrow = today + dt.timedelta(days=1)
 
 Activate modules::
 
     >>> config = activate_modules('stock')
 
 Create company::
 
@@ -85,15 +85,16 @@
     >>> shipment.assigned_by
     >>> shipment.done_by
 
     >>> shipment.click('wait')
     >>> shipment.state
     'waiting'
     >>> shipment.click('assign_try')
-    False
+    >>> shipment.state
+    'waiting'
     >>> shipment.assigned_by
     >>> shipment.done_by
 
 Create Internal Shipment from lost_found location::
 
     >>> lost_found_shipment = Shipment()
     >>> lost_found_shipment.planned_date = today
@@ -106,25 +107,23 @@
     >>> move.uom = unit
     >>> move.quantity = 2
     >>> move.from_location = lost_found_loc
     >>> move.to_location = internal_loc
     >>> move.currency = company.currency
     >>> lost_found_shipment.click('wait')
     >>> lost_found_shipment.click('assign_try')
-    True
     >>> lost_found_shipment.state
     'assigned'
     >>> lost_found_shipment.click('done')
     >>> lost_found_shipment.state
     'done'
 
 Check that now we can finish the older shipment::
 
     >>> shipment.click('assign_try')
-    True
     >>> shipment.assigned_by == employee
     True
     >>> shipment.done_by
 
     >>> shipment.click('done')
     >>> shipment.state
     'done'
```

### Comparing `trytond_stock-6.6.3/tests/scenario_stock_shipment_internal_transit.rst` & `trytond_stock-6.8.0/tests/scenario_stock_shipment_internal_transit.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.6.3/tests/scenario_stock_shipment_out.rst` & `trytond_stock-6.8.0/tests/scenario_stock_shipment_out.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 ===========================
 Stock Shipment Out Scenario
 ===========================
 
 Imports::
 
-    >>> import datetime
-    >>> from dateutil.relativedelta import relativedelta
+    >>> import datetime as dt
     >>> from decimal import Decimal
     >>> from proteus import Model, Wizard
     >>> from trytond.tests.tools import activate_modules, set_user
     >>> from trytond.modules.company.tests.tools import create_company, \
     ...     get_company
-    >>> today = datetime.date.today()
-    >>> yesterday = today - relativedelta(days=1)
+
+    >>> today = dt.date.today()
+    >>> yesterday = today - dt.timedelta(days=1)
 
 Activate modules::
 
     >>> config = activate_modules('stock')
 
 Create company::
 
@@ -127,15 +127,15 @@
     >>> incoming_move.company = company
     >>> incoming_move.unit_price = Decimal('1')
     >>> incoming_move.currency = company.currency
     >>> incoming_move.click('do')
 
 Assign the shipment now::
 
-    >>> shipment_assign = Wizard('stock.shipment.assign', [shipment_out])
+    >>> shipment_assign = shipment_out.click('assign_wizard')
     >>> len(shipment_assign.form.moves)
     1
     >>> shipment_assign.execute('end')
     >>> shipment_out.reload()
     >>> len(shipment_out.outgoing_moves)
     2
     >>> len(shipment_out.inventory_moves)
@@ -151,15 +151,15 @@
     >>> planned_dates = [m.planned_date for m in
     ...     shipment_out.outgoing_moves]
     >>> len(set(planned_dates))
     1
 
 Ignore non assigned moves and pack shipment::
 
-    >>> shipment_assign = Wizard('stock.shipment.assign', [shipment_out])
+    >>> shipment_assign = shipment_out.click('assign_wizard')
     >>> shipment_assign.execute('ignore')
     >>> sorted([m.quantity for m in shipment_out.inventory_moves])
     [0.0, 1.0]
     >>> shipment_out.picked_by
     >>> shipment_out.packed_by
     >>> shipment_out.done_by
 
@@ -244,15 +244,14 @@
     >>> incoming_move.unit_price = Decimal('1')
     >>> incoming_move.currency = company.currency
     >>> incoming_move.click('do')
 
 Finish the shipment::
 
     >>> shipment_out.click('assign_try')
-    True
     >>> shipment_out.click('pick')
     >>> shipment_out.click('pack')
     >>> shipment_out.click('done')
     >>> shipment_out.state
     'done'
     >>> outgoing_move, = shipment_out.outgoing_moves
     >>> outgoing_move.effective_date == yesterday
```

### Comparing `trytond_stock-6.6.3/tests/scenario_stock_shipment_out_return_same_storage_input.rst` & `trytond_stock-6.8.0/tests/scenario_stock_shipment_out_return_same_storage_input.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.6.3/tests/scenario_stock_shipment_out_same_storage_output.rst` & `trytond_stock-6.8.0/tests/scenario_stock_shipment_out_same_storage_output.rst`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.6.3/tests/test_module.py` & `trytond_stock-6.8.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.6.3/trytond_stock.egg-info/PKG-INFO` & `trytond_stock-6.8.0/trytond_stock.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: trytond-stock
-Version: 6.6.3
+Version: 6.8.0
 Summary: Tryton module for stock and inventory
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/6.6/
+Download-URL: http://downloads.tryton.org/6.8/
 Author: Tryton
-Author-email: bugs@tryton.org
+Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/projects/modules-stock/
 Project-URL: Forum, https://www.tryton.org/forum
-Project-URL: Source Code, https://hg.tryton.org/modules/stock
+Project-URL: Source Code, https://code.tryton.org/tryton
 Keywords: tryton stock
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
@@ -39,21 +39,21 @@
 Classifier: Natural Language :: Russian
 Classifier: Natural Language :: Slovenian
 Classifier: Natural Language :: Spanish
 Classifier: Natural Language :: Turkish
 Classifier: Natural Language :: Ukrainian
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: sparklines
 Provides-Extra: test
 License-File: LICENSE
 
 ############
 Stock Module
 ############
```

### Comparing `trytond_stock-6.6.3/trytond_stock.egg-info/SOURCES.txt` & `trytond_stock-6.8.0/trytond_stock.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.6.3/view/configuration_form.xml` & `trytond_stock-6.8.0/view/configuration_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.6.3/view/inventory_form.xml` & `trytond_stock-6.8.0/view/inventory_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.6.3/view/inventory_line_form.xml` & `trytond_stock-6.8.0/view/inventory_line_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.6.3/view/location_form.xml` & `trytond_stock-6.8.0/view/location_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.6.3/view/location_quantity_form.xml` & `trytond_stock-6.8.0/view/location_quantity_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.6.3/view/move_form.xml` & `trytond_stock-6.8.0/view/move_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.6.3/view/move_tree.xml` & `trytond_stock-6.8.0/view/move_tree.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.6.3/view/party_form.xml` & `trytond_stock-6.8.0/view/party_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.6.3/view/reporting_margin_category_list.xml` & `trytond_stock-6.8.0/view/reporting_margin_category_list.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.6.3/view/reporting_margin_context_form.xml` & `trytond_stock-6.8.0/view/reporting_margin_context_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.6.3/view/shipment_in_form.xml` & `trytond_stock-6.8.0/view/shipment_in_return_form.xml`

 * *Files 8% similar despite different names*

#### Comparing `trytond_stock-6.6.3/view/shipment_in_form.xml` & `trytond_stock-6.8.0/view/shipment_in_return_form.xml`

```diff
@@ -4,40 +4,38 @@
 <form col="4" cursor="supplier">
   <label name="reference"/>
   <field name="reference"/>
   <label name="number"/>
   <field name="number"/>
   <label name="supplier"/>
   <field name="supplier"/>
-  <label name="contact_address"/>
-  <field name="contact_address"/>
+  <label name="delivery_address"/>
+  <field name="delivery_address"/>
+  <label name="from_location"/>
+  <field name="from_location"/>
+  <label name="to_location"/>
+  <field name="to_location"/>
   <label name="planned_date"/>
   <field name="planned_date"/>
   <label name="effective_date"/>
   <field name="effective_date"/>
-  <label name="company"/>
-  <field name="company"/>
-  <label name="warehouse"/>
-  <field name="warehouse"/>
-  <notebook colspan="6">
-    <page name="incoming_moves">
-      <field name="incoming_moves" colspan="4" view_ids="stock.move_view_list_shipment_in"/>
-    </page>
-    <page name="inventory_moves">
-      <field name="inventory_moves" colspan="4" view_ids="stock.move_view_list_shipment"/>
+  <notebook colspan="4">
+    <page name="moves">
+      <field name="moves" colspan="4" view_ids="stock.move_view_list_shipment"/>
     </page>
     <page string="Other Info" id="other">
-      <label name="received_by"/>
-      <field name="received_by"/>
+      <label name="assigned_by"/>
+      <field name="assigned_by"/>
       <label name="done_by"/>
       <field name="done_by"/>
     </page>
   </notebook>
   <label name="state"/>
   <field name="state"/>
   <group col="-1" colspan="2" id="buttons">
     <button name="cancel" icon="tryton-cancel"/>
-    <button name="receive" icon="tryton-forward"/>
+    <button name="draft" icon="tryton-forward"/>
+    <button name="wait"/>
+    <button name="assign_wizard" icon="tryton-forward"/>
     <button name="done" icon="tryton-ok"/>
-    <button name="draft" icon="tryton-undo"/>
   </group>
 </form>
```

### Comparing `trytond_stock-6.6.3/view/shipment_in_return_form.xml` & `trytond_stock-6.8.0/view/shipment_out_return_form.xml`

 * *Files 11% similar despite different names*

#### Comparing `trytond_stock-6.6.3/view/shipment_in_return_form.xml` & `trytond_stock-6.8.0/view/shipment_out_return_form.xml`

```diff
@@ -1,41 +1,47 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!-- This file is part of Tryton.  The COPYRIGHT file at the top level of
 this repository contains the full copyright notices and license terms. -->
-<form col="4" cursor="supplier">
+<form col="4" cursor="customer">
   <label name="reference"/>
   <field name="reference"/>
   <label name="number"/>
   <field name="number"/>
-  <label name="supplier"/>
-  <field name="supplier"/>
-  <label name="delivery_address"/>
-  <field name="delivery_address"/>
-  <label name="from_location"/>
-  <field name="from_location"/>
-  <label name="to_location"/>
-  <field name="to_location"/>
+  <label name="customer"/>
+  <field name="customer"/>
+  <label name="contact_address"/>
+  <field name="contact_address"/>
   <label name="planned_date"/>
   <field name="planned_date"/>
   <label name="effective_date"/>
   <field name="effective_date"/>
-  <notebook colspan="4">
-    <page name="moves">
-      <field name="moves" colspan="4" view_ids="stock.move_view_list_shipment"/>
+  <label name="company"/>
+  <field name="company"/>
+  <label name="warehouse"/>
+  <field name="warehouse"/>
+  <notebook colspan="6">
+    <page name="incoming_moves">
+      <field name="incoming_moves" colspan="4" view_ids="stock.move_view_list_shipment"/>
+    </page>
+    <page name="inventory_moves">
+      <field name="inventory_moves" colspan="4" view_ids="stock.move_view_list_shipment"/>
     </page>
     <page string="Other Info" id="other">
-      <label name="assigned_by"/>
-      <field name="assigned_by"/>
+      <label name="warehouse_input"/>
+      <field name="warehouse_input"/>
+      <label name="warehouse_storage"/>
+      <field name="warehouse_storage"/>
+      <label name="received_by"/>
+      <field name="received_by"/>
       <label name="done_by"/>
       <field name="done_by"/>
     </page>
   </notebook>
   <label name="state"/>
   <field name="state"/>
   <group col="-1" colspan="2" id="buttons">
     <button name="cancel" icon="tryton-cancel"/>
-    <button name="draft" icon="tryton-forward"/>
-    <button name="wait"/>
-    <button name="assign_wizard" icon="tryton-forward"/>
+    <button name="draft" icon="tryton-clear"/>
+    <button name="receive" icon="tryton-forward"/>
     <button name="done" icon="tryton-ok"/>
   </group>
 </form>
```

### Comparing `trytond_stock-6.6.3/view/shipment_in_return_tree.xml` & `trytond_stock-6.8.0/view/shipment_in_return_tree.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.6.3/view/shipment_in_tree.xml` & `trytond_stock-6.8.0/view/shipment_in_tree.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.6.3/view/shipment_internal_form.xml` & `trytond_stock-6.8.0/view/shipment_internal_form.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.6.3/view/shipment_internal_tree.xml` & `trytond_stock-6.8.0/view/shipment_internal_tree.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.6.3/view/shipment_out_form.xml` & `trytond_stock-6.8.0/view/shipment_in_form.xml`

 * *Files 12% similar despite different names*

#### Comparing `trytond_stock-6.6.3/view/shipment_out_form.xml` & `trytond_stock-6.8.0/view/shipment_in_form.xml`

```diff
@@ -1,48 +1,47 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!-- This file is part of Tryton.  The COPYRIGHT file at the top level of
 this repository contains the full copyright notices and license terms. -->
-<form cursor="customer">
+<form col="4" cursor="supplier">
   <label name="reference"/>
   <field name="reference"/>
   <label name="number"/>
   <field name="number"/>
-  <label name="customer"/>
-  <field name="customer"/>
-  <label name="delivery_address"/>
-  <field name="delivery_address"/>
+  <label name="supplier"/>
+  <field name="supplier"/>
+  <label name="contact_address"/>
+  <field name="contact_address"/>
   <label name="planned_date"/>
   <field name="planned_date"/>
   <label name="effective_date"/>
   <field name="effective_date"/>
   <label name="company"/>
   <field name="company"/>
   <label name="warehouse"/>
   <field name="warehouse"/>
-  <notebook colspan="4">
+  <notebook colspan="6">
+    <page name="incoming_moves">
+      <field name="incoming_moves" colspan="4" view_ids="stock.move_view_list_shipment_in"/>
+    </page>
     <page name="inventory_moves">
       <field name="inventory_moves" colspan="4" view_ids="stock.move_view_list_shipment"/>
     </page>
-    <page string="Outgoing Moves" id="outgoing_moves">
-      <field name="outgoing_moves" colspan="4" view_ids="stock.move_view_list_shipment"/>
-    </page>
     <page string="Other Info" id="other">
-      <label name="picked_by"/>
-      <field name="picked_by"/>
-      <label name="packed_by"/>
-      <field name="packed_by"/>
+      <label name="warehouse_input"/>
+      <field name="warehouse_input"/>
+      <label name="warehouse_storage"/>
+      <field name="warehouse_storage"/>
+      <label name="received_by"/>
+      <field name="received_by"/>
       <label name="done_by"/>
       <field name="done_by"/>
     </page>
   </notebook>
   <label name="state"/>
   <field name="state"/>
   <group col="-1" colspan="2" id="buttons">
     <button name="cancel" icon="tryton-cancel"/>
-    <button name="draft"/>
-    <button name="wait"/>
-    <button name="assign_wizard" icon="tryton-forward"/>
-    <button name="pick"/>
-    <button name="pack" icon="tryton-forward"/>
+    <button name="receive" icon="tryton-forward"/>
     <button name="done" icon="tryton-ok"/>
+    <button name="draft" icon="tryton-undo"/>
   </group>
 </form>
```

### Comparing `trytond_stock-6.6.3/view/shipment_out_return_form.xml` & `trytond_stock-6.8.0/view/shipment_out_form.xml`

 * *Files 25% similar despite different names*

#### Comparing `trytond_stock-6.6.3/view/shipment_out_return_form.xml` & `trytond_stock-6.8.0/view/shipment_out_form.xml`

```diff
@@ -1,43 +1,52 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!-- This file is part of Tryton.  The COPYRIGHT file at the top level of
 this repository contains the full copyright notices and license terms. -->
-<form col="4" cursor="customer">
+<form cursor="customer">
   <label name="reference"/>
   <field name="reference"/>
   <label name="number"/>
   <field name="number"/>
   <label name="customer"/>
   <field name="customer"/>
-  <label name="contact_address"/>
-  <field name="contact_address"/>
+  <label name="delivery_address"/>
+  <field name="delivery_address"/>
   <label name="planned_date"/>
   <field name="planned_date"/>
   <label name="effective_date"/>
   <field name="effective_date"/>
   <label name="company"/>
   <field name="company"/>
   <label name="warehouse"/>
   <field name="warehouse"/>
-  <notebook colspan="6">
-    <page name="incoming_moves">
-      <field name="incoming_moves" colspan="4" view_ids="stock.move_view_list_shipment"/>
-    </page>
+  <notebook colspan="4">
     <page name="inventory_moves">
       <field name="inventory_moves" colspan="4" view_ids="stock.move_view_list_shipment"/>
     </page>
+    <page string="Outgoing Moves" id="outgoing_moves">
+      <field name="outgoing_moves" colspan="4" view_ids="stock.move_view_list_shipment"/>
+    </page>
     <page string="Other Info" id="other">
-      <label name="received_by"/>
-      <field name="received_by"/>
+      <label name="warehouse_storage"/>
+      <field name="warehouse_storage"/>
+      <label name="warehouse_output"/>
+      <field name="warehouse_output"/>
+      <label name="picked_by"/>
+      <field name="picked_by"/>
+      <label name="packed_by"/>
+      <field name="packed_by"/>
       <label name="done_by"/>
       <field name="done_by"/>
     </page>
   </notebook>
   <label name="state"/>
   <field name="state"/>
   <group col="-1" colspan="2" id="buttons">
     <button name="cancel" icon="tryton-cancel"/>
-    <button name="draft" icon="tryton-clear"/>
-    <button name="receive" icon="tryton-forward"/>
+    <button name="draft"/>
+    <button name="wait"/>
+    <button name="assign_wizard" icon="tryton-forward"/>
+    <button name="pick"/>
+    <button name="pack" icon="tryton-forward"/>
     <button name="done" icon="tryton-ok"/>
   </group>
 </form>
```

### Comparing `trytond_stock-6.6.3/view/shipment_out_return_tree.xml` & `trytond_stock-6.8.0/view/shipment_out_return_tree.xml`

 * *Files identical despite different names*

### Comparing `trytond_stock-6.6.3/view/shipment_out_tree.xml` & `trytond_stock-6.8.0/view/shipment_out_tree.xml`

 * *Files identical despite different names*

