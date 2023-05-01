# Comparing `tmp/sw_mc_lib-0.1.tar.gz` & `tmp/sw_mc_lib-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sw_mc_lib-0.1.tar", last modified: Mon May  1 10:54:25 2023, max compression
+gzip compressed data, was "sw_mc_lib-0.2.0.tar", last modified: Mon May  1 21:29:54 2023, max compression
```

## Comparing `sw_mc_lib-0.1.tar` & `sw_mc_lib-0.2.0.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2023-05-01 10:54:25.724378 sw_mc_lib-0.1/
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1073 2023-04-21 16:19:23.000000 sw_mc_lib-0.1/LICENSE
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      963 2023-05-01 10:54:25.724378 sw_mc_lib-0.1/PKG-INFO
--rw-rw-r--   0 fabian    (1000) fabian    (1000)       47 2023-04-21 16:19:23.000000 sw_mc_lib-0.1/README.md
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1213 2023-05-01 10:53:39.000000 sw_mc_lib-0.1/pyproject.toml
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      163 2023-05-01 10:54:25.724378 sw_mc_lib-0.1/setup.cfg
-drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2023-05-01 10:54:25.707377 sw_mc_lib-0.1/sw_mc_lib/
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     9379 2023-05-01 10:01:40.000000 sw_mc_lib-0.1/sw_mc_lib/Component.py
-drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2023-05-01 10:54:25.721378 sw_mc_lib-0.1/sw_mc_lib/Components/
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1244 2023-04-30 15:17:44.000000 sw_mc_lib-0.1/sw_mc_lib/Components/AND.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1143 2023-04-30 15:17:44.000000 sw_mc_lib-0.1/sw_mc_lib/Components/Abs.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1244 2023-04-30 15:17:44.000000 sw_mc_lib-0.1/sw_mc_lib/Components/Add.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1650 2023-04-30 21:35:03.000000 sw_mc_lib-0.1/sw_mc_lib/Components/ArithmeticFunction1In.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1936 2023-04-30 15:17:44.000000 sw_mc_lib-0.1/sw_mc_lib/Components/ArithmeticFunction3In.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     2682 2023-04-30 15:17:44.000000 sw_mc_lib-0.1/sw_mc_lib/Components/ArithmeticFunction8In.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1664 2023-04-30 21:22:03.000000 sw_mc_lib-0.1/sw_mc_lib/Components/AudioSwitchbox.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1997 2023-04-30 15:17:44.000000 sw_mc_lib-0.1/sw_mc_lib/Components/Blinker.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     2022 2023-04-30 21:35:03.000000 sw_mc_lib-0.1/sw_mc_lib/Components/BooleanFunction4In.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     2636 2023-04-30 21:35:03.000000 sw_mc_lib-0.1/sw_mc_lib/Components/BooleanFunction8In.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1897 2023-04-30 15:17:44.000000 sw_mc_lib-0.1/sw_mc_lib/Components/Capacitor.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1658 2023-04-30 15:17:44.000000 sw_mc_lib-0.1/sw_mc_lib/Components/Clamp.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1391 2023-04-30 21:35:03.000000 sw_mc_lib-0.1/sw_mc_lib/Components/CompositeBinaryToNumber.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1830 2023-04-30 20:21:32.000000 sw_mc_lib-0.1/sw_mc_lib/Components/CompositeReadBoolean.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1822 2023-04-30 20:21:37.000000 sw_mc_lib-0.1/sw_mc_lib/Components/CompositeReadNumber.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1696 2023-04-30 21:21:00.000000 sw_mc_lib-0.1/sw_mc_lib/Components/CompositeSwitchbox.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     3125 2023-04-30 21:35:03.000000 sw_mc_lib-0.1/sw_mc_lib/Components/CompositeWriteBoolean.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     3117 2023-04-30 21:35:03.000000 sw_mc_lib-0.1/sw_mc_lib/Components/CompositeWriteNumber.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1444 2023-04-30 15:17:44.000000 sw_mc_lib-0.1/sw_mc_lib/Components/ConstantNumber.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      962 2023-04-30 15:17:44.000000 sw_mc_lib-0.1/sw_mc_lib/Components/ConstantOn.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1130 2023-04-30 15:17:44.000000 sw_mc_lib-0.1/sw_mc_lib/Components/Delta.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1268 2023-04-30 15:17:44.000000 sw_mc_lib-0.1/sw_mc_lib/Components/Divide.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1260 2023-04-30 20:49:40.000000 sw_mc_lib-0.1/sw_mc_lib/Components/Equal.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1308 2023-04-30 15:17:44.000000 sw_mc_lib-0.1/sw_mc_lib/Components/GreaterThan.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1324 2023-04-30 15:17:44.000000 sw_mc_lib-0.1/sw_mc_lib/Components/JKFlipFlop.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1284 2023-04-30 15:17:44.000000 sw_mc_lib-0.1/sw_mc_lib/Components/LessThan.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     2239 2023-04-30 21:35:03.000000 sw_mc_lib-0.1/sw_mc_lib/Components/LuaScript.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     2048 2023-04-30 15:17:44.000000 sw_mc_lib-0.1/sw_mc_lib/Components/MemoryRegister.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1268 2023-04-30 15:17:44.000000 sw_mc_lib-0.1/sw_mc_lib/Components/Modulo.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1284 2023-04-30 15:17:44.000000 sw_mc_lib-0.1/sw_mc_lib/Components/Multiply.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1252 2023-04-30 15:17:44.000000 sw_mc_lib-0.1/sw_mc_lib/Components/NAND.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1244 2023-04-30 15:17:44.000000 sw_mc_lib-0.1/sw_mc_lib/Components/NOR.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1098 2023-04-30 15:17:44.000000 sw_mc_lib-0.1/sw_mc_lib/Components/NOT.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1391 2023-04-30 21:35:03.000000 sw_mc_lib-0.1/sw_mc_lib/Components/NumberToCompositeBinary.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1589 2023-04-30 15:17:44.000000 sw_mc_lib-0.1/sw_mc_lib/Components/NumericalJunction.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1696 2023-04-30 15:17:44.000000 sw_mc_lib-0.1/sw_mc_lib/Components/NumericalSwitchbox.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1236 2023-04-30 15:17:44.000000 sw_mc_lib-0.1/sw_mc_lib/Components/OR.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     2842 2023-04-30 15:17:44.000000 sw_mc_lib-0.1/sw_mc_lib/Components/PIDController.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     2357 2023-04-30 15:17:44.000000 sw_mc_lib-0.1/sw_mc_lib/Components/PIDControllerAdvanced.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     2874 2023-05-01 08:35:55.000000 sw_mc_lib-0.1/sw_mc_lib/Components/PropertyDropdown.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1564 2023-04-30 15:17:44.000000 sw_mc_lib-0.1/sw_mc_lib/Components/PropertyNumber.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     2318 2023-04-30 15:17:44.000000 sw_mc_lib-0.1/sw_mc_lib/Components/PropertySlider.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1461 2023-04-30 21:35:03.000000 sw_mc_lib-0.1/sw_mc_lib/Components/PropertyText.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1876 2023-04-30 15:17:44.000000 sw_mc_lib-0.1/sw_mc_lib/Components/PropertyToggle.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1457 2023-04-30 21:35:03.000000 sw_mc_lib-0.1/sw_mc_lib/Components/Pulse.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1170 2023-04-30 15:17:44.000000 sw_mc_lib-0.1/sw_mc_lib/Components/PushToToggle.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1300 2023-04-30 15:17:44.000000 sw_mc_lib-0.1/sw_mc_lib/Components/SRLatch.py
-drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2023-05-01 10:54:25.722378 sw_mc_lib-0.1/sw_mc_lib/Components/SubTypes/
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1273 2023-04-30 15:17:44.000000 sw_mc_lib-0.1/sw_mc_lib/Components/SubTypes/MinMaxComponent.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1039 2023-04-30 15:17:44.000000 sw_mc_lib-0.1/sw_mc_lib/Components/SubTypes/ResetComponent.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1046 2023-04-30 15:17:44.000000 sw_mc_lib-0.1/sw_mc_lib/Components/SubTypes/ValueComponent.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)        0 2023-04-21 11:51:32.000000 sw_mc_lib-0.1/sw_mc_lib/Components/SubTypes/__init__.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1284 2023-04-30 15:17:44.000000 sw_mc_lib-0.1/sw_mc_lib/Components/Subtract.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1755 2023-04-30 15:17:44.000000 sw_mc_lib-0.1/sw_mc_lib/Components/Threshold.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1771 2023-04-30 21:35:03.000000 sw_mc_lib-0.1/sw_mc_lib/Components/TimerRTF.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1771 2023-04-30 21:35:03.000000 sw_mc_lib-0.1/sw_mc_lib/Components/TimerRTO.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1592 2023-04-30 21:35:03.000000 sw_mc_lib-0.1/sw_mc_lib/Components/TimerTOF.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1592 2023-04-30 21:35:03.000000 sw_mc_lib-0.1/sw_mc_lib/Components/TimerTON.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     2400 2023-04-30 21:35:03.000000 sw_mc_lib-0.1/sw_mc_lib/Components/TooltipBoolean.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     2082 2023-04-30 21:35:03.000000 sw_mc_lib-0.1/sw_mc_lib/Components/TooltipNumber.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     2819 2023-04-30 15:17:44.000000 sw_mc_lib-0.1/sw_mc_lib/Components/UpDownCounter.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1664 2023-04-30 21:21:41.000000 sw_mc_lib-0.1/sw_mc_lib/Components/VideoSwitchbox.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1244 2023-04-30 15:17:44.000000 sw_mc_lib-0.1/sw_mc_lib/Components/XOR.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     2218 2023-04-30 21:48:55.000000 sw_mc_lib-0.1/sw_mc_lib/Components/__init__.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1062 2023-04-30 15:17:44.000000 sw_mc_lib-0.1/sw_mc_lib/Input.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     3718 2023-05-01 08:46:26.000000 sw_mc_lib-0.1/sw_mc_lib/Microcontroller.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     2909 2023-04-30 15:17:44.000000 sw_mc_lib-0.1/sw_mc_lib/Node.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      960 2023-04-30 15:17:44.000000 sw_mc_lib-0.1/sw_mc_lib/NumberProperty.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      878 2023-04-30 15:17:44.000000 sw_mc_lib-0.1/sw_mc_lib/Position.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     2103 2023-04-30 21:20:09.000000 sw_mc_lib-0.1/sw_mc_lib/Types.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      829 2023-04-30 15:17:44.000000 sw_mc_lib-0.1/sw_mc_lib/XMLElement.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     2256 2023-04-30 08:43:19.000000 sw_mc_lib-0.1/sw_mc_lib/XMLFormatter.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     4269 2023-04-30 15:17:44.000000 sw_mc_lib-0.1/sw_mc_lib/XMLParser.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)        0 2023-04-20 20:44:52.000000 sw_mc_lib-0.1/sw_mc_lib/__init__.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1243 2023-05-01 10:01:07.000000 sw_mc_lib-0.1/sw_mc_lib/util.py
-drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2023-05-01 10:54:25.708377 sw_mc_lib-0.1/sw_mc_lib.egg-info/
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      963 2023-05-01 10:54:25.000000 sw_mc_lib-0.1/sw_mc_lib.egg-info/PKG-INFO
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     2965 2023-05-01 10:54:25.000000 sw_mc_lib-0.1/sw_mc_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 fabian    (1000) fabian    (1000)        1 2023-05-01 10:54:25.000000 sw_mc_lib-0.1/sw_mc_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 fabian    (1000) fabian    (1000)       69 2023-05-01 10:54:25.000000 sw_mc_lib-0.1/sw_mc_lib.egg-info/requires.txt
--rw-rw-r--   0 fabian    (1000) fabian    (1000)       10 2023-05-01 10:54:25.000000 sw_mc_lib-0.1/sw_mc_lib.egg-info/top_level.txt
-drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2023-05-01 10:54:25.724378 sw_mc_lib-0.1/test/
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     4934 2023-04-30 20:36:29.000000 sw_mc_lib-0.1/test/test_component.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1148 2023-04-30 06:28:11.000000 sw_mc_lib-0.1/test/test_input.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     2028 2023-04-30 15:23:37.000000 sw_mc_lib-0.1/test/test_number_property.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1081 2023-04-30 08:03:11.000000 sw_mc_lib-0.1/test/test_position.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     2968 2023-04-30 15:17:44.000000 sw_mc_lib-0.1/test/test_xml_formatter.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1964 2023-04-29 15:44:02.000000 sw_mc_lib-0.1/test/test_xml_parser.py
+drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2023-05-01 21:29:54.929953 sw_mc_lib-0.2.0/
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1073 2023-04-21 16:19:23.000000 sw_mc_lib-0.2.0/LICENSE
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      967 2023-05-01 21:29:54.929953 sw_mc_lib-0.2.0/PKG-INFO
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)       49 2023-05-01 20:30:36.000000 sw_mc_lib-0.2.0/README.md
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1200 2023-05-01 21:28:51.000000 sw_mc_lib-0.2.0/pyproject.toml
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      163 2023-05-01 21:29:54.929953 sw_mc_lib-0.2.0/setup.cfg
+drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2023-05-01 21:29:54.921953 sw_mc_lib-0.2.0/sw_mc_lib/
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     9879 2023-05-01 19:50:53.000000 sw_mc_lib-0.2.0/sw_mc_lib/Component.py
+drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2023-05-01 21:29:54.928954 sw_mc_lib-0.2.0/sw_mc_lib/Components/
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1315 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.0/sw_mc_lib/Components/AND.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1246 2023-05-01 15:24:25.000000 sw_mc_lib-0.2.0/sw_mc_lib/Components/Abs.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1324 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.0/sw_mc_lib/Components/Add.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1753 2023-05-01 15:25:02.000000 sw_mc_lib-0.2.0/sw_mc_lib/Components/ArithmeticFunction1In.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     2046 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.0/sw_mc_lib/Components/ArithmeticFunction3In.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     2792 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.0/sw_mc_lib/Components/ArithmeticFunction8In.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1789 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.0/sw_mc_lib/Components/AudioSwitchbox.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     2080 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.0/sw_mc_lib/Components/Blinker.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     2127 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.0/sw_mc_lib/Components/BooleanFunction4In.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     2741 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.0/sw_mc_lib/Components/BooleanFunction8In.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1997 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.0/sw_mc_lib/Components/Capacitor.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1752 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.0/sw_mc_lib/Components/Clamp.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1507 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.0/sw_mc_lib/Components/CompositeBinaryToNumber.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1920 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.0/sw_mc_lib/Components/CompositeReadBoolean.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1912 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.0/sw_mc_lib/Components/CompositeReadNumber.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1825 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.0/sw_mc_lib/Components/CompositeSwitchbox.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     3339 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.0/sw_mc_lib/Components/CompositeWriteBoolean.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     3324 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.0/sw_mc_lib/Components/CompositeWriteNumber.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1528 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.0/sw_mc_lib/Components/ConstantNumber.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1013 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.0/sw_mc_lib/Components/ConstantOn.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1230 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.0/sw_mc_lib/Components/Delta.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1351 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.0/sw_mc_lib/Components/Divide.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1350 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.0/sw_mc_lib/Components/Equal.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1397 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.0/sw_mc_lib/Components/GreaterThan.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1412 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.0/sw_mc_lib/Components/JKFlipFlop.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1370 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.0/sw_mc_lib/Components/LessThan.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     2329 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.0/sw_mc_lib/Components/LuaScript.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     2268 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.0/sw_mc_lib/Components/MemoryRegister.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1331 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.0/sw_mc_lib/Components/Modulo.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1361 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.0/sw_mc_lib/Components/Multiply.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1324 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.0/sw_mc_lib/Components/NAND.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1315 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.0/sw_mc_lib/Components/NOR.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1164 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.0/sw_mc_lib/Components/NOT.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1500 2023-05-01 15:24:44.000000 sw_mc_lib-0.2.0/sw_mc_lib/Components/NumberToCompositeBinary.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1777 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.0/sw_mc_lib/Components/NumericalJunction.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1821 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.0/sw_mc_lib/Components/NumericalSwitchbox.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1306 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.0/sw_mc_lib/Components/OR.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     2969 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.0/sw_mc_lib/Components/PIDController.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     2454 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.0/sw_mc_lib/Components/PIDControllerAdvanced.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     3112 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.0/sw_mc_lib/Components/PropertyDropdown.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1696 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.0/sw_mc_lib/Components/PropertyNumber.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     2444 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.0/sw_mc_lib/Components/PropertySlider.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1648 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.0/sw_mc_lib/Components/PropertyText.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     2009 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.0/sw_mc_lib/Components/PropertyToggle.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1657 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.0/sw_mc_lib/Components/Pulse.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1273 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.0/sw_mc_lib/Components/PushToToggle.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1384 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.0/sw_mc_lib/Components/SRLatch.py
+drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2023-05-01 21:29:54.928954 sw_mc_lib-0.2.0/sw_mc_lib/Components/SubTypes/
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1339 2023-05-01 12:54:18.000000 sw_mc_lib-0.2.0/sw_mc_lib/Components/SubTypes/MinMaxComponent.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1105 2023-05-01 12:54:18.000000 sw_mc_lib-0.2.0/sw_mc_lib/Components/SubTypes/ResetComponent.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1106 2023-05-01 12:54:18.000000 sw_mc_lib-0.2.0/sw_mc_lib/Components/SubTypes/ValueComponent.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)        0 2023-04-21 11:51:32.000000 sw_mc_lib-0.2.0/sw_mc_lib/Components/SubTypes/__init__.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1371 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.0/sw_mc_lib/Components/Subtract.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1870 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.0/sw_mc_lib/Components/Threshold.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1929 2023-05-01 15:23:45.000000 sw_mc_lib-0.2.0/sw_mc_lib/Components/TimerRTF.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1924 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.0/sw_mc_lib/Components/TimerRTO.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1733 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.0/sw_mc_lib/Components/TimerTOF.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1724 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.0/sw_mc_lib/Components/TimerTON.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     2542 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.0/sw_mc_lib/Components/TooltipBoolean.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     2212 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.0/sw_mc_lib/Components/TooltipNumber.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     2928 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.0/sw_mc_lib/Components/UpDownCounter.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1789 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.0/sw_mc_lib/Components/VideoSwitchbox.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1315 2023-05-01 15:29:11.000000 sw_mc_lib-0.2.0/sw_mc_lib/Components/XOR.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     2218 2023-04-30 21:48:55.000000 sw_mc_lib-0.2.0/sw_mc_lib/Components/__init__.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1173 2023-05-01 15:20:10.000000 sw_mc_lib-0.2.0/sw_mc_lib/Input.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     4058 2023-05-01 19:13:34.000000 sw_mc_lib-0.2.0/sw_mc_lib/Microcontroller.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     3231 2023-05-01 15:37:20.000000 sw_mc_lib-0.2.0/sw_mc_lib/Node.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1478 2023-05-01 19:13:58.000000 sw_mc_lib-0.2.0/sw_mc_lib/NumberProperty.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      874 2023-05-01 15:39:10.000000 sw_mc_lib-0.2.0/sw_mc_lib/Position.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     2586 2023-05-01 12:32:04.000000 sw_mc_lib-0.2.0/sw_mc_lib/Types.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1159 2023-05-01 19:14:23.000000 sw_mc_lib-0.2.0/sw_mc_lib/XMLElement.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     2795 2023-05-01 19:48:50.000000 sw_mc_lib-0.2.0/sw_mc_lib/XMLFormatter.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     5953 2023-05-01 19:43:01.000000 sw_mc_lib-0.2.0/sw_mc_lib/XMLParser.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)        0 2023-04-20 20:44:52.000000 sw_mc_lib-0.2.0/sw_mc_lib/__init__.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1576 2023-05-01 19:14:13.000000 sw_mc_lib-0.2.0/sw_mc_lib/util.py
+drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2023-05-01 21:29:54.921953 sw_mc_lib-0.2.0/sw_mc_lib.egg-info/
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      967 2023-05-01 21:29:54.000000 sw_mc_lib-0.2.0/sw_mc_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     2965 2023-05-01 21:29:54.000000 sw_mc_lib-0.2.0/sw_mc_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)        1 2023-05-01 21:29:54.000000 sw_mc_lib-0.2.0/sw_mc_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)       69 2023-05-01 21:29:54.000000 sw_mc_lib-0.2.0/sw_mc_lib.egg-info/requires.txt
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)       10 2023-05-01 21:29:54.000000 sw_mc_lib-0.2.0/sw_mc_lib.egg-info/top_level.txt
+drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2023-05-01 21:29:54.929953 sw_mc_lib-0.2.0/test/
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     4924 2023-05-01 15:40:04.000000 sw_mc_lib-0.2.0/test/test_component.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1148 2023-04-30 06:28:11.000000 sw_mc_lib-0.2.0/test/test_input.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     2028 2023-04-30 15:23:37.000000 sw_mc_lib-0.2.0/test/test_number_property.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1071 2023-05-01 15:40:04.000000 sw_mc_lib-0.2.0/test/test_position.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     2968 2023-04-30 15:17:44.000000 sw_mc_lib-0.2.0/test/test_xml_formatter.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1851 2023-05-01 15:31:58.000000 sw_mc_lib-0.2.0/test/test_xml_parser.py
```

### Comparing `sw_mc_lib-0.1/LICENSE` & `sw_mc_lib-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.1/PKG-INFO` & `sw_mc_lib-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sw_mc_lib
-Version: 0.1
+Version: 0.2.0
 Summary: Library for interaction with Stormworks Microcontrollers
 Author: Fabian Wunsch
 License: MIT License
 Project-URL: homepage, https://github.com/stormworks-utils/sw_mc_lib
 Project-URL: repository, https://github.com/stormworks-utils/sw_mc_lib
 Keywords: stormworks,lib,microcontroller
 Classifier: Programming Language :: Python :: 3
@@ -20,7 +20,9 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # sw_mc_lib
 Stormworks Microcontroller library
+
+
```

### Comparing `sw_mc_lib-0.1/pyproject.toml` & `sw_mc_lib-0.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
-requires = ["numpy>=1.13", "setuptools"]
+requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "sw_mc_lib"
-version = "0.1"
+version = "0.2.0"
 description = "Library for interaction with Stormworks Microcontrollers"
 readme = "README.md"
 requires-python = ">=3.10"
 keywords = ["stormworks", "lib", "microcontroller"]
 license = {text = "MIT License"}
 authors = [
     {name = "Fabian Wunsch"}
```

### Comparing `sw_mc_lib-0.1/sw_mc_lib/Component.py` & `sw_mc_lib-0.2.0/sw_mc_lib/Component.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,18 @@
 from .XMLElement import XMLElement
 from .XMLParser import XMLParserElement
 
 INNER_TO_XML_RESULT = tuple[dict[str, str], list[XMLParserElement]]
 
 
 class Component(XMLElement, ABC):
+    """
+    A generic Component
+    """
+
     width: float = 1
 
     def __init__(
         self,
         component_type: ComponentType,
         component_id: int,
         position: Position,
@@ -30,42 +34,46 @@
         self.height: float = height
 
     @staticmethod
     def _basic_in_parsing(
         element: XMLParserElement,
     ) -> tuple[int, Position, dict[str, Input], dict[str, NumberProperty]]:
         component_id: int = int(element.attributes.get("id", "0"))
-        position: Optional[Position] = None
+        position: Position = Position()
         inputs: dict[str, Input] = {}
         properties: dict[str, NumberProperty] = {}
         for child in element.children:
             if child.tag == "pos":
                 position = Position.from_xml(child)
             elif child.tag.startswith("in"):
                 input: Input = Input.from_xml(child)
                 if input.component_id > 0:
                     inputs[input.index] = input
             else:
                 properties[child.tag] = NumberProperty.from_xml(child)
-        if not position:
-            position = Position.empty_pos()
         return component_id, position, inputs, properties
 
     @abstractmethod
     def _inner_to_xml(self) -> tuple[dict[str, str], list[XMLParserElement]]:
         ...
 
     def to_xml(self) -> XMLParserElement:
         object_element = XMLParserElement("object", {"id": str(self.component_id)}, [])
         inner_attributes, inner_children = self._inner_to_xml()
         object_element.attributes.update(inner_attributes)
         object_element.children = inner_children
         return XMLParserElement("c", {"type": str(self.type.value)}, [object_element])
 
     def to_state_xml(self, index: int) -> XMLParserElement:
+        """
+        Convert this Component to a XML state entity
+
+        :param index: The zero based index of the entity
+        :return: XML state representation
+        """
         c_element: XMLParserElement = XMLParserElement(
             f"c{index}", {"id": str(self.component_id)}
         )
         inner_attributes, inner_children = self._inner_to_xml()
         c_element.attributes.update(inner_attributes)
         c_element.children = inner_children
         return c_element
@@ -75,14 +83,19 @@
         *inputs: Optional[Input],
         named_inputs: Optional[dict[str, Optional[Input]]] = None,
         properties: Optional[dict[str, NumberProperty]] = None,
     ) -> list[XMLParserElement]:
         """
         Turn the position and inputs into an element. Will strip all None inputs. Will also rename all numbered inputs
         to their according supplied index, and all named inputs to the supplied name.
+
+        :param inputs: Array of inputs, the order is important, as it defines overrides
+        :param named_inputs: Inputs by name, used for overrides
+        :param properties: Properties by name
+        :return: XML elements for all relevant children
         """
         named_inputs = named_inputs or {}
         properties = properties or {}
         children: list[XMLParserElement] = [self.position.to_xml()]
         for i, input in chain(enumerate(inputs), named_inputs.items()):
             if input is not None:
                 if isinstance(i, int):
@@ -94,14 +107,15 @@
         for name, property in properties.items():
             property.name = name
             children.append(property.to_xml())
         return children
 
     @staticmethod
     def from_xml(element: XMLParserElement) -> Component:
+        # pylint: disable=too-many-statements
         component_type: ComponentType = ComponentType(
             int(element.attributes.get("type", "0"))
         )
         element_class: Optional[Type[Component]] = None
         match component_type:
             case ComponentType.Abs:
                 element_class = Abs
@@ -222,8 +236,8 @@
         if not element_class:
             raise NotImplementedError(
                 f"No Component found for component type {component_type}"
             )
         return element_class.from_xml(element)
 
 
-from .Components import *  # noqa: ignore=F403
+from .Components import *  # noqa: ignore=F403 pylint: disable=wildcard-import,wrong-import-position
```

### Comparing `sw_mc_lib-0.1/sw_mc_lib/Components/AND.py` & `sw_mc_lib-0.2.0/sw_mc_lib/Components/Add.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,31 +5,35 @@
 from sw_mc_lib.Component import INNER_TO_XML_RESULT, Component
 from sw_mc_lib.Input import Input
 from sw_mc_lib.Position import Position
 from sw_mc_lib.Types import ComponentType
 from sw_mc_lib.XMLParser import XMLParserElement
 
 
-class AND(Component):
+class Add(Component):
+    """
+    Adds the two input values together and outputs the result.
+    """
+
     def __init__(
         self,
         component_id: int,
         position: Position,
         a_input: Optional[Input] = None,
         b_input: Optional[Input] = None,
     ):
-        super().__init__(ComponentType.AND, component_id, position, 0.75)
+        super().__init__(ComponentType.Add, component_id, position, 0.75)
         self.a_input: Optional[Input] = a_input
         self.b_input: Optional[Input] = b_input
 
     @staticmethod
-    def from_xml(element: XMLParserElement) -> AND:
-        assert element.tag == "c", f"invalid AND {element}"
+    def from_xml(element: XMLParserElement) -> Add:
+        assert element.tag == "c", f"invalid Add {element}"
         assert element.attributes.get("type", "0") == str(
-            ComponentType.AND.value
-        ), f"Not an AND {element}"
+            ComponentType.Add.value
+        ), f"Not an Add {element}"
         obj: XMLParserElement = element.children[0]
-        component_id, position, inputs, _ = AND._basic_in_parsing(obj)
-        return AND(component_id, position, inputs.get("1"), inputs.get("2"))
+        component_id, position, inputs, _ = Add._basic_in_parsing(obj)
+        return Add(component_id, position, inputs.get("1"), inputs.get("2"))
 
     def _inner_to_xml(self) -> INNER_TO_XML_RESULT:
         return {}, self._pos_in_to_xml(self.a_input, self.b_input)
```

### Comparing `sw_mc_lib-0.1/sw_mc_lib/Components/Abs.py` & `sw_mc_lib-0.2.0/sw_mc_lib/Components/XOR.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,29 +5,35 @@
 from sw_mc_lib.Component import INNER_TO_XML_RESULT, Component
 from sw_mc_lib.Input import Input
 from sw_mc_lib.Position import Position
 from sw_mc_lib.Types import ComponentType
 from sw_mc_lib.XMLParser import XMLParserElement
 
 
-class Abs(Component):
+class XOR(Component):
+    """
+    Outputs the logical XOR of its two input signals.
+    """
+
     def __init__(
         self,
         component_id: int,
         position: Position,
-        number_input: Optional[Input] = None,
+        a_input: Optional[Input] = None,
+        b_input: Optional[Input] = None,
     ):
-        super().__init__(ComponentType.Abs, component_id, position, 0.5)
-        self.number_input: Optional[Input] = number_input
+        super().__init__(ComponentType.XOR, component_id, position, 0.75)
+        self.a_input: Optional[Input] = a_input
+        self.b_input: Optional[Input] = b_input
 
     @staticmethod
-    def from_xml(element: XMLParserElement) -> Abs:
-        assert element.tag == "c", f"invalid Abs {element}"
+    def from_xml(element: XMLParserElement) -> XOR:
+        assert element.tag == "c", f"invalid XOR {element}"
         assert element.attributes.get("type", "0") == str(
-            ComponentType.Abs.value
-        ), f"Not an Abs {element}"
+            ComponentType.XOR.value
+        ), f"Not an XOR {element}"
         obj: XMLParserElement = element.children[0]
-        component_id, position, inputs, _ = Abs._basic_in_parsing(obj)
-        return Abs(component_id, position, inputs.get("1"))
+        component_id, position, inputs, _ = XOR._basic_in_parsing(obj)
+        return XOR(component_id, position, inputs.get("1"), inputs.get("2"))
 
     def _inner_to_xml(self) -> INNER_TO_XML_RESULT:
-        return {}, self._pos_in_to_xml(self.number_input)
+        return {}, self._pos_in_to_xml(self.a_input, self.b_input)
```

### Comparing `sw_mc_lib-0.1/sw_mc_lib/Components/Add.py` & `sw_mc_lib-0.2.0/sw_mc_lib/Components/SRLatch.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,31 +5,35 @@
 from sw_mc_lib.Component import INNER_TO_XML_RESULT, Component
 from sw_mc_lib.Input import Input
 from sw_mc_lib.Position import Position
 from sw_mc_lib.Types import ComponentType
 from sw_mc_lib.XMLParser import XMLParserElement
 
 
-class Add(Component):
+class SRLatch(Component):
+    """
+    An SR latch that can be set and reset using two on/off inputs.
+    """
+
     def __init__(
         self,
         component_id: int,
         position: Position,
-        a_input: Optional[Input] = None,
-        b_input: Optional[Input] = None,
+        set_input: Optional[Input] = None,
+        reset_input: Optional[Input] = None,
     ):
-        super().__init__(ComponentType.Add, component_id, position, 0.75)
-        self.a_input: Optional[Input] = a_input
-        self.b_input: Optional[Input] = b_input
+        super().__init__(ComponentType.SRLatch, component_id, position, 0.75)
+        self.set_input: Optional[Input] = set_input
+        self.reset_input: Optional[Input] = reset_input
 
     @staticmethod
-    def from_xml(element: XMLParserElement) -> Add:
-        assert element.tag == "c", f"invalid Add {element}"
+    def from_xml(element: XMLParserElement) -> SRLatch:
+        assert element.tag == "c", f"invalid SRLatch {element}"
         assert element.attributes.get("type", "0") == str(
-            ComponentType.Add.value
-        ), f"Not an Add {element}"
+            ComponentType.SRLatch.value
+        ), f"Not an SRLatch {element}"
         obj: XMLParserElement = element.children[0]
-        component_id, position, inputs, _ = Add._basic_in_parsing(obj)
-        return Add(component_id, position, inputs.get("1"), inputs.get("2"))
+        component_id, position, inputs, _ = SRLatch._basic_in_parsing(obj)
+        return SRLatch(component_id, position, inputs.get("1"), inputs.get("2"))
 
     def _inner_to_xml(self) -> INNER_TO_XML_RESULT:
-        return {}, self._pos_in_to_xml(self.a_input, self.b_input)
+        return {}, self._pos_in_to_xml(self.set_input, self.reset_input)
```

### Comparing `sw_mc_lib-0.1/sw_mc_lib/Components/ArithmeticFunction1In.py` & `sw_mc_lib-0.2.0/sw_mc_lib/Components/ArithmeticFunction1In.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,18 @@
 from sw_mc_lib.Input import Input
 from sw_mc_lib.Position import Position
 from sw_mc_lib.Types import ComponentType
 from sw_mc_lib.XMLParser import XMLParserElement
 
 
 class ArithmeticFunction1In(Component):
+    """
+    Evaluates a mathematical expression with 1 input variable and outputs the result.
+    """
+
     def __init__(
         self,
         component_id: int,
         position: Position,
         function: str,
         x_input: Optional[Input] = None,
     ):
```

### Comparing `sw_mc_lib-0.1/sw_mc_lib/Components/ArithmeticFunction3In.py` & `sw_mc_lib-0.2.0/sw_mc_lib/Components/TimerRTF.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,58 +1,52 @@
 from __future__ import annotations
 
 from typing import Optional
 
 from sw_mc_lib.Component import INNER_TO_XML_RESULT, Component
 from sw_mc_lib.Input import Input
 from sw_mc_lib.Position import Position
-from sw_mc_lib.Types import ComponentType
+from sw_mc_lib.Types import ComponentType, TimerUnit
 from sw_mc_lib.XMLParser import XMLParserElement
 
 
-class ArithmeticFunction3In(Component):
+class TimerRTF(Component):
+    """
+    Variable input timer. Outputs an on signal when the timer is less than its duration.
+    The timer will not reset until it is signalled.
+    """
+
     def __init__(
         self,
         component_id: int,
         position: Position,
-        function: str,
-        x_input: Optional[Input] = None,
-        y_input: Optional[Input] = None,
-        z_input: Optional[Input] = None,
+        unit_property: TimerUnit = TimerUnit.Seconds,
+        timer_enable_input: Optional[Input] = None,
+        duration_input: Optional[Input] = None,
+        reset_input: Optional[Input] = None,
     ):
-        super().__init__(
-            ComponentType.ArithmeticFunction3In, component_id, position, 1.0
-        )
-        self.function: str = function
-        self.x_input: Optional[Input] = x_input
-        self.y_input: Optional[Input] = y_input
-        self.z_input: Optional[Input] = z_input
+        super().__init__(ComponentType.TimerRTF, component_id, position, 0.75)
+        self.timer_enable_input: Optional[Input] = timer_enable_input
+        self.duration_input: Optional[Input] = duration_input
+        self.reset_input: Optional[Input] = reset_input
+        self.unit_property: TimerUnit = unit_property
 
     @staticmethod
-    def from_xml(element: XMLParserElement) -> ArithmeticFunction3In:
-        assert element.tag == "c", f"invalid ArithmeticFunction3In {element}"
+    def from_xml(element: XMLParserElement) -> TimerRTF:
+        assert element.tag == "c", f"invalid TimerRTF {element}"
         assert element.attributes.get("type", "0") == str(
-            ComponentType.ArithmeticFunction3In.value
-        ), f"Not an ArithmeticFunction3In {element}"
+            ComponentType.TimerRTF.value
+        ), f"Not an TimerRTF {element}"
         obj: XMLParserElement = element.children[0]
-        (
+        component_id, position, inputs, _ = TimerRTF._basic_in_parsing(obj)
+        unit_property: TimerUnit = TimerUnit(int(obj.attributes.get("u", "0")))
+        return TimerRTF(
             component_id,
             position,
-            inputs,
-            _,
-        ) = ArithmeticFunction3In._basic_in_parsing(obj)
-        function: str = obj.attributes.get("e", "")
-        return ArithmeticFunction3In(
-            component_id,
-            position,
-            function,
+            unit_property,
             inputs.get("1"),
             inputs.get("2"),
             inputs.get("3"),
         )
 
     def _inner_to_xml(self) -> INNER_TO_XML_RESULT:
-        attributes: dict[str, str] = {"e": self.function}
-        children: list[XMLParserElement] = self._pos_in_to_xml(
-            self.x_input, self.y_input, self.z_input
-        )
-        return attributes, children
+        return {}, self._pos_in_to_xml(self.timer_enable_input, self.duration_input)
```

### Comparing `sw_mc_lib-0.1/sw_mc_lib/Components/ArithmeticFunction8In.py` & `sw_mc_lib-0.2.0/sw_mc_lib/Components/ArithmeticFunction3In.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,76 +5,58 @@
 from sw_mc_lib.Component import INNER_TO_XML_RESULT, Component
 from sw_mc_lib.Input import Input
 from sw_mc_lib.Position import Position
 from sw_mc_lib.Types import ComponentType
 from sw_mc_lib.XMLParser import XMLParserElement
 
 
-class ArithmeticFunction8In(Component):
+class ArithmeticFunction3In(Component):
+    """
+    Evaluates a mathematical expression with up to 3 input variables and outputs the result.
+    """
+
     def __init__(
         self,
         component_id: int,
         position: Position,
         function: str,
         x_input: Optional[Input] = None,
         y_input: Optional[Input] = None,
         z_input: Optional[Input] = None,
-        w_input: Optional[Input] = None,
-        a_input: Optional[Input] = None,
-        b_input: Optional[Input] = None,
-        c_input: Optional[Input] = None,
-        d_input: Optional[Input] = None,
     ):
         super().__init__(
-            ComponentType.ArithmeticFunction8In, component_id, position, 2.25
+            ComponentType.ArithmeticFunction3In, component_id, position, 1.0
         )
         self.function: str = function
         self.x_input: Optional[Input] = x_input
         self.y_input: Optional[Input] = y_input
         self.z_input: Optional[Input] = z_input
-        self.w_input: Optional[Input] = w_input
-        self.a_input: Optional[Input] = a_input
-        self.b_input: Optional[Input] = b_input
-        self.c_input: Optional[Input] = c_input
-        self.d_input: Optional[Input] = d_input
 
     @staticmethod
-    def from_xml(element: XMLParserElement) -> ArithmeticFunction8In:
-        assert element.tag == "c", f"invalid ArithmeticFunction8In {element}"
+    def from_xml(element: XMLParserElement) -> ArithmeticFunction3In:
+        assert element.tag == "c", f"invalid ArithmeticFunction3In {element}"
         assert element.attributes.get("type", "0") == str(
-            ComponentType.ArithmeticFunction8In.value
-        ), f"Not an ArithmeticFunction8In {element}"
+            ComponentType.ArithmeticFunction3In.value
+        ), f"Not an ArithmeticFunction3In {element}"
         obj: XMLParserElement = element.children[0]
         (
             component_id,
             position,
             inputs,
             _,
-        ) = ArithmeticFunction8In._basic_in_parsing(obj)
+        ) = ArithmeticFunction3In._basic_in_parsing(obj)
         function: str = obj.attributes.get("e", "")
-        return ArithmeticFunction8In(
+        return ArithmeticFunction3In(
             component_id,
             position,
             function,
             inputs.get("1"),
             inputs.get("2"),
             inputs.get("3"),
-            inputs.get("4"),
-            inputs.get("5"),
-            inputs.get("6"),
-            inputs.get("7"),
-            inputs.get("8"),
         )
 
     def _inner_to_xml(self) -> INNER_TO_XML_RESULT:
         attributes: dict[str, str] = {"e": self.function}
         children: list[XMLParserElement] = self._pos_in_to_xml(
-            self.x_input,
-            self.y_input,
-            self.z_input,
-            self.w_input,
-            self.a_input,
-            self.b_input,
-            self.c_input,
-            self.d_input,
+            self.x_input, self.y_input, self.z_input
         )
         return attributes, children
```

### Comparing `sw_mc_lib-0.1/sw_mc_lib/Components/AudioSwitchbox.py` & `sw_mc_lib-0.2.0/sw_mc_lib/Components/NumericalSwitchbox.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,42 +5,46 @@
 from sw_mc_lib.Component import INNER_TO_XML_RESULT, Component
 from sw_mc_lib.Input import Input
 from sw_mc_lib.Position import Position
 from sw_mc_lib.Types import ComponentType
 from sw_mc_lib.XMLParser import XMLParserElement
 
 
-class AudioSwitchbox(Component):
+class NumericalSwitchbox(Component):
+    """
+    Outputs the first input value when receiving an on signal, and the second when receiving an off signal.
+    """
+
     def __init__(
         self,
         component_id: int,
         position: Position,
         on_value_input: Optional[Input] = None,
         off_value_input: Optional[Input] = None,
         switch_signal_input: Optional[Input] = None,
     ):
-        super().__init__(ComponentType.AudioSwitchbox, component_id, position, 1.0)
+        super().__init__(ComponentType.NumericalSwitchbox, component_id, position, 1.0)
         self.on_value_input: Optional[Input] = on_value_input
         self.off_value_input: Optional[Input] = off_value_input
         self.switch_signal_input: Optional[Input] = switch_signal_input
 
     @staticmethod
-    def from_xml(element: XMLParserElement) -> AudioSwitchbox:
-        assert element.tag == "c", f"invalid AudioSwitchbox {element}"
+    def from_xml(element: XMLParserElement) -> NumericalSwitchbox:
+        assert element.tag == "c", f"invalid NumericalSwitchbox {element}"
         assert element.attributes.get("type", "0") == str(
-            ComponentType.AudioSwitchbox.value
-        ), f"Not an AudioSwitchbox {element}"
+            ComponentType.NumericalSwitchbox.value
+        ), f"Not an NumericalSwitchbox {element}"
         obj: XMLParserElement = element.children[0]
         (
             component_id,
             position,
             inputs,
             _,
-        ) = AudioSwitchbox._basic_in_parsing(obj)
-        return AudioSwitchbox(
+        ) = NumericalSwitchbox._basic_in_parsing(obj)
+        return NumericalSwitchbox(
             component_id, position, inputs.get("1"), inputs.get("2"), inputs.get("3")
         )
 
     def _inner_to_xml(self) -> INNER_TO_XML_RESULT:
         return {}, self._pos_in_to_xml(
             self.on_value_input, self.off_value_input, self.switch_signal_input
         )
```

### Comparing `sw_mc_lib-0.1/sw_mc_lib/Components/Blinker.py` & `sw_mc_lib-0.2.0/sw_mc_lib/Components/Blinker.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,14 +6,18 @@
 from sw_mc_lib.Input import Input
 from sw_mc_lib.Position import Position
 from sw_mc_lib.Types import ComponentType
 from sw_mc_lib.XMLParser import XMLParserElement
 
 
 class Blinker(Component):
+    """
+    Outputs a value that blinks between on and off at a set rate.
+    """
+
     def __init__(
         self,
         component_id: int,
         position: Position,
         control_signal_input: Optional[Input] = None,
         blink_on_duration_property: float = 1.0,
         blink_off_duration_property: float = 1.0,
```

### Comparing `sw_mc_lib-0.1/sw_mc_lib/Components/BooleanFunction4In.py` & `sw_mc_lib-0.2.0/sw_mc_lib/Components/BooleanFunction4In.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,14 +6,18 @@
 from sw_mc_lib.Input import Input
 from sw_mc_lib.Position import Position
 from sw_mc_lib.Types import ComponentType
 from sw_mc_lib.XMLParser import XMLParserElement
 
 
 class BooleanFunction4In(Component):
+    """
+    Evaluates a logical expression with up to 4 input variables and outputs the result.
+    """
+
     def __init__(
         self,
         component_id: int,
         position: Position,
         function: str,
         x_input: Optional[Input] = None,
         y_input: Optional[Input] = None,
```

### Comparing `sw_mc_lib-0.1/sw_mc_lib/Components/BooleanFunction8In.py` & `sw_mc_lib-0.2.0/sw_mc_lib/Components/BooleanFunction8In.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,18 @@
 from sw_mc_lib.Input import Input
 from sw_mc_lib.Position import Position
 from sw_mc_lib.Types import ComponentType
 from sw_mc_lib.XMLParser import XMLParserElement
 
 
 class BooleanFunction8In(Component):
+    """
+    Evaluates a logical expression with up to 8 input variables and outputs the result.
+    """
+
     def __init__(
         self,
         component_id: int,
         position: Position,
         function: str,
         x_input: Optional[Input] = None,
         y_input: Optional[Input] = None,
```

### Comparing `sw_mc_lib-0.1/sw_mc_lib/Components/Capacitor.py` & `sw_mc_lib-0.2.0/sw_mc_lib/Components/Capacitor.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,18 @@
 from sw_mc_lib.Input import Input
 from sw_mc_lib.Position import Position
 from sw_mc_lib.Types import ComponentType
 from sw_mc_lib.XMLParser import XMLParserElement
 
 
 class Capacitor(Component):
+    """
+    Charges up when receiving an on signal, then discharges over a period of time.
+    """
+
     def __init__(
         self,
         component_id: int,
         position: Position,
         charge_input: Optional[Input] = None,
         charge_time_property: float = 1.0,
         discharge_time_property: float = 1.0,
```

### Comparing `sw_mc_lib-0.1/sw_mc_lib/Components/Clamp.py` & `sw_mc_lib-0.2.0/sw_mc_lib/Components/Clamp.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,14 +9,18 @@
 from sw_mc_lib.Types import ComponentType
 from sw_mc_lib.XMLParser import XMLParserElement
 
 from .SubTypes.MinMaxComponent import MinMaxComponent
 
 
 class Clamp(MinMaxComponent):
+    """
+    Clamps the input value between a set min and max and outputs the result.
+    """
+
     def __init__(
         self,
         component_id: int,
         position: Position,
         min_property: Optional[NumberProperty] = None,
         max_property: Optional[NumberProperty] = None,
         number_input: Optional[Input] = None,
```

### Comparing `sw_mc_lib-0.1/sw_mc_lib/Components/CompositeBinaryToNumber.py` & `sw_mc_lib-0.2.0/sw_mc_lib/Components/CompositeBinaryToNumber.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,18 @@
 from sw_mc_lib.Input import Input
 from sw_mc_lib.Position import Position
 from sw_mc_lib.Types import ComponentType
 from sw_mc_lib.XMLParser import XMLParserElement
 
 
 class CompositeBinaryToNumber(Component):
+    """
+    Reads the on/off signals of a composite link and encodes them in the bits of an output number.
+    """
+
     def __init__(
         self,
         component_id: int,
         position: Position,
         signal_to_convert_input: Optional[Input] = None,
     ):
         super().__init__(
```

### Comparing `sw_mc_lib-0.1/sw_mc_lib/Components/CompositeReadBoolean.py` & `sw_mc_lib-0.2.0/sw_mc_lib/Components/CompositeReadBoolean.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,14 +6,18 @@
 from sw_mc_lib.Input import Input
 from sw_mc_lib.Position import Position
 from sw_mc_lib.Types import ComponentType
 from sw_mc_lib.XMLParser import XMLParserElement
 
 
 class CompositeReadBoolean(Component):
+    """
+    Reads the on/off value from a selected channel of a composite input.
+    """
+
     def __init__(
         self,
         component_id: int,
         position: Position,
         channel_property: int = 1,
         composite_signal_input: Optional[Input] = None,
     ):
```

### Comparing `sw_mc_lib-0.1/sw_mc_lib/Components/CompositeReadNumber.py` & `sw_mc_lib-0.2.0/sw_mc_lib/Components/CompositeReadNumber.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,14 +6,18 @@
 from sw_mc_lib.Input import Input
 from sw_mc_lib.Position import Position
 from sw_mc_lib.Types import ComponentType
 from sw_mc_lib.XMLParser import XMLParserElement
 
 
 class CompositeReadNumber(Component):
+    """
+    Reads the number value from a selected channel of a composite input.
+    """
+
     def __init__(
         self,
         component_id: int,
         position: Position,
         channel_property: int = 1,
         composite_signal_input: Optional[Input] = None,
     ):
```

### Comparing `sw_mc_lib-0.1/sw_mc_lib/Components/CompositeSwitchbox.py` & `sw_mc_lib-0.2.0/sw_mc_lib/Components/TimerRTO.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,46 +1,52 @@
 from __future__ import annotations
 
 from typing import Optional
 
 from sw_mc_lib.Component import INNER_TO_XML_RESULT, Component
 from sw_mc_lib.Input import Input
 from sw_mc_lib.Position import Position
-from sw_mc_lib.Types import ComponentType
+from sw_mc_lib.Types import ComponentType, TimerUnit
 from sw_mc_lib.XMLParser import XMLParserElement
 
 
-class CompositeSwitchbox(Component):
+class TimerRTO(Component):
+    """
+    Variable input timer. Outputs an on signal when the timer reaches its duration.
+    The timer will not reset until it is signalled.
+    """
+
     def __init__(
         self,
         component_id: int,
         position: Position,
-        on_value_input: Optional[Input] = None,
-        off_value_input: Optional[Input] = None,
-        switch_signal_input: Optional[Input] = None,
+        unit_property: TimerUnit = TimerUnit.Seconds,
+        timer_enable_input: Optional[Input] = None,
+        duration_input: Optional[Input] = None,
+        reset_input: Optional[Input] = None,
     ):
-        super().__init__(ComponentType.CompositeSwitchbox, component_id, position, 1.0)
-        self.on_value_input: Optional[Input] = on_value_input
-        self.off_value_input: Optional[Input] = off_value_input
-        self.switch_signal_input: Optional[Input] = switch_signal_input
+        super().__init__(ComponentType.TimerRTO, component_id, position, 0.75)
+        self.timer_enable_input: Optional[Input] = timer_enable_input
+        self.duration_input: Optional[Input] = duration_input
+        self.reset_input: Optional[Input] = reset_input
+        self.unit_property: TimerUnit = unit_property
 
     @staticmethod
-    def from_xml(element: XMLParserElement) -> CompositeSwitchbox:
-        assert element.tag == "c", f"invalid CompositeSwitchbox {element}"
+    def from_xml(element: XMLParserElement) -> TimerRTO:
+        assert element.tag == "c", f"invalid TimerRTO {element}"
         assert element.attributes.get("type", "0") == str(
-            ComponentType.CompositeSwitchbox.value
-        ), f"Not an CompositeSwitchbox {element}"
+            ComponentType.TimerRTO.value
+        ), f"Not an TimerRTO {element}"
         obj: XMLParserElement = element.children[0]
-        (
+        component_id, position, inputs, _ = TimerRTO._basic_in_parsing(obj)
+        unit_property: TimerUnit = TimerUnit(int(obj.attributes.get("u", "0")))
+        return TimerRTO(
             component_id,
             position,
-            inputs,
-            _,
-        ) = CompositeSwitchbox._basic_in_parsing(obj)
-        return CompositeSwitchbox(
-            component_id, position, inputs.get("1"), inputs.get("2"), inputs.get("3")
+            unit_property,
+            inputs.get("1"),
+            inputs.get("2"),
+            inputs.get("3"),
         )
 
     def _inner_to_xml(self) -> INNER_TO_XML_RESULT:
-        return {}, self._pos_in_to_xml(
-            self.on_value_input, self.off_value_input, self.switch_signal_input
-        )
+        return {}, self._pos_in_to_xml(self.timer_enable_input, self.duration_input)
```

### Comparing `sw_mc_lib-0.1/sw_mc_lib/Components/CompositeWriteBoolean.py` & `sw_mc_lib-0.2.0/sw_mc_lib/Components/CompositeWriteBoolean.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,19 @@
 from sw_mc_lib.Input import Input
 from sw_mc_lib.Position import Position
 from sw_mc_lib.Types import ComponentType
 from sw_mc_lib.XMLParser import XMLParserElement
 
 
 class CompositeWriteBoolean(Component):
+    """
+    Writes up to 32 on/off signals to a composite link in a single logic tick.
+    Only connected channels will be modified. The number of inputs and channel to begin writing at can be configured.
+    """
+
     def __init__(
         self,
         component_id: int,
         position: Position,
         start_channel_property: int = 1,
         channel_count_property: int = 1,
         composite_signal_input: Optional[Input] = None,
```

### Comparing `sw_mc_lib-0.1/sw_mc_lib/Components/CompositeWriteNumber.py` & `sw_mc_lib-0.2.0/sw_mc_lib/Components/CompositeWriteNumber.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,14 +6,19 @@
 from sw_mc_lib.Input import Input
 from sw_mc_lib.Position import Position
 from sw_mc_lib.Types import ComponentType
 from sw_mc_lib.XMLParser import XMLParserElement
 
 
 class CompositeWriteNumber(Component):
+    """
+    Writes up to 32 numbers to a composite link in a single logic tick. Only connected channels will be modified.
+    The number of inputs and channel to begin writing at can be configured.
+    """
+
     def __init__(
         self,
         component_id: int,
         position: Position,
         start_channel_property: int = 1,
         channel_count_property: int = 1,
         composite_signal_input: Optional[Input] = None,
```

### Comparing `sw_mc_lib-0.1/sw_mc_lib/Components/ConstantNumber.py` & `sw_mc_lib-0.2.0/sw_mc_lib/Components/ConstantNumber.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,18 @@
 from sw_mc_lib.Types import ComponentType
 from sw_mc_lib.XMLParser import XMLParserElement
 
 from .SubTypes.ValueComponent import ValueComponent
 
 
 class ConstantNumber(ValueComponent):
+    """
+    Outputs a constant number that is set on the properties panel.
+    """
+
     def __init__(
         self,
         component_id: int,
         position: Position,
         value_property: Optional[NumberProperty] = None,
     ):
         super().__init__(
```

### Comparing `sw_mc_lib-0.1/sw_mc_lib/Components/ConstantOn.py` & `sw_mc_lib-0.2.0/sw_mc_lib/Components/ConstantOn.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 from sw_mc_lib.Component import INNER_TO_XML_RESULT, Component
 from sw_mc_lib.Position import Position
 from sw_mc_lib.Types import ComponentType
 from sw_mc_lib.XMLParser import XMLParserElement
 
 
 class ConstantOn(Component):
+    """
+    Outputs a constant on signal.
+    """
+
     def __init__(self, component_id: int, position: Position):
         super().__init__(ComponentType.ConstantOn, component_id, position, 0.5)
 
     @staticmethod
     def from_xml(element: XMLParserElement) -> ConstantOn:
         assert element.tag == "c", f"invalid ConstantOn {element}"
         assert element.attributes.get("type", "0") == str(
```

### Comparing `sw_mc_lib-0.1/sw_mc_lib/Components/Delta.py` & `sw_mc_lib-0.2.0/sw_mc_lib/Components/JKFlipFlop.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,26 +5,35 @@
 from sw_mc_lib.Component import INNER_TO_XML_RESULT, Component
 from sw_mc_lib.Input import Input
 from sw_mc_lib.Position import Position
 from sw_mc_lib.Types import ComponentType
 from sw_mc_lib.XMLParser import XMLParserElement
 
 
-class Delta(Component):
+class JKFlipFlop(Component):
+    """
+    An JK flip flop that can be set and reset using two on/off inputs.
+    """
+
     def __init__(
-        self, component_id: int, position: Position, value_input: Optional[Input] = None
+        self,
+        component_id: int,
+        position: Position,
+        set_input: Optional[Input] = None,
+        reset_input: Optional[Input] = None,
     ):
-        super().__init__(ComponentType.Delta, component_id, position, 0.5)
-        self.value_input: Optional[Input] = value_input
+        super().__init__(ComponentType.JKFlipFlop, component_id, position, 0.75)
+        self.set_input: Optional[Input] = set_input
+        self.reset_input: Optional[Input] = reset_input
 
     @staticmethod
-    def from_xml(element: XMLParserElement) -> Delta:
-        assert element.tag == "c", f"invalid Delta {element}"
+    def from_xml(element: XMLParserElement) -> JKFlipFlop:
+        assert element.tag == "c", f"invalid JKFlipFlop {element}"
         assert element.attributes.get("type", "0") == str(
-            ComponentType.Delta.value
-        ), f"Not an Delta {element}"
+            ComponentType.JKFlipFlop.value
+        ), f"Not an JKFlipFlop {element}"
         obj: XMLParserElement = element.children[0]
-        component_id, position, inputs, _ = Delta._basic_in_parsing(obj)
-        return Delta(component_id, position, inputs.get("1"))
+        component_id, position, inputs, _ = JKFlipFlop._basic_in_parsing(obj)
+        return JKFlipFlop(component_id, position, inputs.get("1"), inputs.get("2"))
 
     def _inner_to_xml(self) -> INNER_TO_XML_RESULT:
-        return {}, self._pos_in_to_xml(self.value_input)
+        return {}, self._pos_in_to_xml(self.set_input, self.reset_input)
```

### Comparing `sw_mc_lib-0.1/sw_mc_lib/Components/Divide.py` & `sw_mc_lib-0.2.0/sw_mc_lib/Components/Equal.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,31 +5,35 @@
 from sw_mc_lib.Component import INNER_TO_XML_RESULT, Component
 from sw_mc_lib.Input import Input
 from sw_mc_lib.Position import Position
 from sw_mc_lib.Types import ComponentType
 from sw_mc_lib.XMLParser import XMLParserElement
 
 
-class Divide(Component):
+class Equal(Component):
+    """
+    Compares whether or not two numbers are equal within a set accuracy.
+    """
+
     def __init__(
         self,
         component_id: int,
         position: Position,
         a_input: Optional[Input] = None,
         b_input: Optional[Input] = None,
     ):
-        super().__init__(ComponentType.Divide, component_id, position, 0.75)
+        super().__init__(ComponentType.Equal, component_id, position, 0.75)
         self.a_input: Optional[Input] = a_input
         self.b_input: Optional[Input] = b_input
 
     @staticmethod
-    def from_xml(element: XMLParserElement) -> Divide:
-        assert element.tag == "c", f"invalid Divide {element}"
+    def from_xml(element: XMLParserElement) -> Equal:
+        assert element.tag == "c", f"invalid Equal {element}"
         assert element.attributes.get("type", "0") == str(
-            ComponentType.Divide.value
-        ), f"Not an Divide {element}"
+            ComponentType.Equal.value
+        ), f"Not an Equal {element}"
         obj: XMLParserElement = element.children[0]
-        component_id, position, inputs, _ = Divide._basic_in_parsing(obj)
-        return Divide(component_id, position, inputs.get("1"), inputs.get("2"))
+        component_id, position, inputs, _ = Equal._basic_in_parsing(obj)
+        return Equal(component_id, position, inputs.get("1"), inputs.get("2"))
 
     def _inner_to_xml(self) -> INNER_TO_XML_RESULT:
         return {}, self._pos_in_to_xml(self.a_input, self.b_input)
```

### Comparing `sw_mc_lib-0.1/sw_mc_lib/Components/Equal.py` & `sw_mc_lib-0.2.0/sw_mc_lib/Components/Multiply.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,31 +5,35 @@
 from sw_mc_lib.Component import INNER_TO_XML_RESULT, Component
 from sw_mc_lib.Input import Input
 from sw_mc_lib.Position import Position
 from sw_mc_lib.Types import ComponentType
 from sw_mc_lib.XMLParser import XMLParserElement
 
 
-class Equal(Component):
+class Multiply(Component):
+    """
+    Multiplies the two input values and outputs the result.
+    """
+
     def __init__(
         self,
         component_id: int,
         position: Position,
         a_input: Optional[Input] = None,
         b_input: Optional[Input] = None,
     ):
-        super().__init__(ComponentType.Equal, component_id, position, 0.75)
+        super().__init__(ComponentType.Multiply, component_id, position, 0.75)
         self.a_input: Optional[Input] = a_input
         self.b_input: Optional[Input] = b_input
 
     @staticmethod
-    def from_xml(element: XMLParserElement) -> Equal:
-        assert element.tag == "c", f"invalid Equal {element}"
+    def from_xml(element: XMLParserElement) -> Multiply:
+        assert element.tag == "c", f"invalid Multiply {element}"
         assert element.attributes.get("type", "0") == str(
-            ComponentType.Equal.value
-        ), f"Not an Equal {element}"
+            ComponentType.Multiply.value
+        ), f"Not an Multiply {element}"
         obj: XMLParserElement = element.children[0]
-        component_id, position, inputs, _ = Equal._basic_in_parsing(obj)
-        return Equal(component_id, position, inputs.get("1"), inputs.get("2"))
+        component_id, position, inputs, _ = Multiply._basic_in_parsing(obj)
+        return Multiply(component_id, position, inputs.get("1"), inputs.get("2"))
 
     def _inner_to_xml(self) -> INNER_TO_XML_RESULT:
         return {}, self._pos_in_to_xml(self.a_input, self.b_input)
```

### Comparing `sw_mc_lib-0.1/sw_mc_lib/Components/GreaterThan.py` & `sw_mc_lib-0.2.0/sw_mc_lib/Components/GreaterThan.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,18 @@
 from sw_mc_lib.Input import Input
 from sw_mc_lib.Position import Position
 from sw_mc_lib.Types import ComponentType
 from sw_mc_lib.XMLParser import XMLParserElement
 
 
 class GreaterThan(Component):
+    """
+    Outputs an on signal if the first input is greater than the second.
+    """
+
     def __init__(
         self,
         component_id: int,
         position: Position,
         a_input: Optional[Input] = None,
         b_input: Optional[Input] = None,
     ):
```

### Comparing `sw_mc_lib-0.1/sw_mc_lib/Components/JKFlipFlop.py` & `sw_mc_lib-0.2.0/sw_mc_lib/Components/Abs.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,31 +5,33 @@
 from sw_mc_lib.Component import INNER_TO_XML_RESULT, Component
 from sw_mc_lib.Input import Input
 from sw_mc_lib.Position import Position
 from sw_mc_lib.Types import ComponentType
 from sw_mc_lib.XMLParser import XMLParserElement
 
 
-class JKFlipFlop(Component):
+class Abs(Component):
+    """
+    Outputs the absolute value of the input value (negative numbers become positive).
+    """
+
     def __init__(
         self,
         component_id: int,
         position: Position,
-        set_input: Optional[Input] = None,
-        reset_input: Optional[Input] = None,
+        number_input: Optional[Input] = None,
     ):
-        super().__init__(ComponentType.JKFlipFlop, component_id, position, 0.75)
-        self.set_input: Optional[Input] = set_input
-        self.reset_input: Optional[Input] = reset_input
+        super().__init__(ComponentType.Abs, component_id, position, 0.5)
+        self.number_input: Optional[Input] = number_input
 
     @staticmethod
-    def from_xml(element: XMLParserElement) -> JKFlipFlop:
-        assert element.tag == "c", f"invalid JKFlipFlop {element}"
+    def from_xml(element: XMLParserElement) -> Abs:
+        assert element.tag == "c", f"invalid Abs {element}"
         assert element.attributes.get("type", "0") == str(
-            ComponentType.JKFlipFlop.value
-        ), f"Not an JKFlipFlop {element}"
+            ComponentType.Abs.value
+        ), f"Not an Abs {element}"
         obj: XMLParserElement = element.children[0]
-        component_id, position, inputs, _ = JKFlipFlop._basic_in_parsing(obj)
-        return JKFlipFlop(component_id, position, inputs.get("1"), inputs.get("2"))
+        component_id, position, inputs, _ = Abs._basic_in_parsing(obj)
+        return Abs(component_id, position, inputs.get("1"))
 
     def _inner_to_xml(self) -> INNER_TO_XML_RESULT:
-        return {}, self._pos_in_to_xml(self.set_input, self.reset_input)
+        return {}, self._pos_in_to_xml(self.number_input)
```

### Comparing `sw_mc_lib-0.1/sw_mc_lib/Components/LessThan.py` & `sw_mc_lib-0.2.0/sw_mc_lib/Components/LessThan.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,18 @@
 from sw_mc_lib.Input import Input
 from sw_mc_lib.Position import Position
 from sw_mc_lib.Types import ComponentType
 from sw_mc_lib.XMLParser import XMLParserElement
 
 
 class LessThan(Component):
+    """
+    Outputs an on signal if the first value is less than the second.
+    """
+
     def __init__(
         self,
         component_id: int,
         position: Position,
         a_input: Optional[Input] = None,
         b_input: Optional[Input] = None,
     ):
```

### Comparing `sw_mc_lib-0.1/sw_mc_lib/Components/LuaScript.py` & `sw_mc_lib-0.2.0/sw_mc_lib/Components/LuaScript.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,18 @@
 \th = screen.getHeight()\t\t\t\t\t
 \tscreen.setColor(0, 255, 0)\t\t\t -- Set draw color to green
 \tscreen.drawCircleF(w / 2, h / 2, 30)   -- Draw a 30px radius circle in the center of the screen
 end"""
 
 
 class LuaScript(Component):
+    """
+    Runs a custom lua script for advanced logic and drawing to monitors.
+    """
+
     def __init__(
         self,
         component_id: int,
         position: Position,
         script_property: str = DEFAULT_SCRIPT,
         data_input: Optional[Input] = None,
         video_input: Optional[Input] = None,
```

### Comparing `sw_mc_lib-0.1/sw_mc_lib/Components/MemoryRegister.py` & `sw_mc_lib-0.2.0/sw_mc_lib/Components/MemoryRegister.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,19 @@
 from sw_mc_lib.Types import ComponentType
 from sw_mc_lib.XMLParser import XMLParserElement
 
 from .SubTypes.ResetComponent import ResetComponent
 
 
 class MemoryRegister(ResetComponent):
+    """
+    "Remembers the input value when receiving a signal to the Set node. When the Reset node receives a signal,
+    the stored number is cleared to a value that can be customised in the properties panel.
+    """
+
     def __init__(
         self,
         component_id: int,
         position: Position,
         reset_property: Optional[NumberProperty] = None,
         set_input: Optional[Input] = None,
         reset_input: Optional[Input] = None,
```

### Comparing `sw_mc_lib-0.1/sw_mc_lib/Components/Modulo.py` & `sw_mc_lib-0.2.0/sw_mc_lib/Components/NOR.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,31 +5,35 @@
 from sw_mc_lib.Component import INNER_TO_XML_RESULT, Component
 from sw_mc_lib.Input import Input
 from sw_mc_lib.Position import Position
 from sw_mc_lib.Types import ComponentType
 from sw_mc_lib.XMLParser import XMLParserElement
 
 
-class Modulo(Component):
+class NOR(Component):
+    """
+    Outputs the logical NOR of its two input signals.
+    """
+
     def __init__(
         self,
         component_id: int,
         position: Position,
         a_input: Optional[Input] = None,
         b_input: Optional[Input] = None,
     ):
-        super().__init__(ComponentType.Modulo, component_id, position, 0.75)
+        super().__init__(ComponentType.NOR, component_id, position, 0.75)
         self.a_input: Optional[Input] = a_input
         self.b_input: Optional[Input] = b_input
 
     @staticmethod
-    def from_xml(element: XMLParserElement) -> Modulo:
-        assert element.tag == "c", f"invalid Modulo {element}"
+    def from_xml(element: XMLParserElement) -> NOR:
+        assert element.tag == "c", f"invalid NOR {element}"
         assert element.attributes.get("type", "0") == str(
-            ComponentType.Modulo.value
-        ), f"Not an Modulo {element}"
+            ComponentType.NOR.value
+        ), f"Not an NOR {element}"
         obj: XMLParserElement = element.children[0]
-        component_id, position, inputs, _ = Modulo._basic_in_parsing(obj)
-        return Modulo(component_id, position, inputs.get("1"), inputs.get("2"))
+        component_id, position, inputs, _ = NOR._basic_in_parsing(obj)
+        return NOR(component_id, position, inputs.get("1"), inputs.get("2"))
 
     def _inner_to_xml(self) -> INNER_TO_XML_RESULT:
         return {}, self._pos_in_to_xml(self.a_input, self.b_input)
```

### Comparing `sw_mc_lib-0.1/sw_mc_lib/Components/Multiply.py` & `sw_mc_lib-0.2.0/sw_mc_lib/Components/OR.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,31 +5,35 @@
 from sw_mc_lib.Component import INNER_TO_XML_RESULT, Component
 from sw_mc_lib.Input import Input
 from sw_mc_lib.Position import Position
 from sw_mc_lib.Types import ComponentType
 from sw_mc_lib.XMLParser import XMLParserElement
 
 
-class Multiply(Component):
+class OR(Component):
+    """
+    Outputs the logical OR of its two input signals.
+    """
+
     def __init__(
         self,
         component_id: int,
         position: Position,
         a_input: Optional[Input] = None,
         b_input: Optional[Input] = None,
     ):
-        super().__init__(ComponentType.Multiply, component_id, position, 0.75)
+        super().__init__(ComponentType.OR, component_id, position, 0.75)
         self.a_input: Optional[Input] = a_input
         self.b_input: Optional[Input] = b_input
 
     @staticmethod
-    def from_xml(element: XMLParserElement) -> Multiply:
-        assert element.tag == "c", f"invalid Multiply {element}"
+    def from_xml(element: XMLParserElement) -> OR:
+        assert element.tag == "c", f"invalid OR {element}"
         assert element.attributes.get("type", "0") == str(
-            ComponentType.Multiply.value
-        ), f"Not an Multiply {element}"
+            ComponentType.OR.value
+        ), f"Not an OR {element}"
         obj: XMLParserElement = element.children[0]
-        component_id, position, inputs, _ = Multiply._basic_in_parsing(obj)
-        return Multiply(component_id, position, inputs.get("1"), inputs.get("2"))
+        component_id, position, inputs, _ = OR._basic_in_parsing(obj)
+        return OR(component_id, position, inputs.get("1"), inputs.get("2"))
 
     def _inner_to_xml(self) -> INNER_TO_XML_RESULT:
         return {}, self._pos_in_to_xml(self.a_input, self.b_input)
```

### Comparing `sw_mc_lib-0.1/sw_mc_lib/Components/NAND.py` & `sw_mc_lib-0.2.0/sw_mc_lib/Components/Divide.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,31 +5,35 @@
 from sw_mc_lib.Component import INNER_TO_XML_RESULT, Component
 from sw_mc_lib.Input import Input
 from sw_mc_lib.Position import Position
 from sw_mc_lib.Types import ComponentType
 from sw_mc_lib.XMLParser import XMLParserElement
 
 
-class NAND(Component):
+class Divide(Component):
+    """
+    Divides the first input by the second and outputs the result.
+    """
+
     def __init__(
         self,
         component_id: int,
         position: Position,
         a_input: Optional[Input] = None,
         b_input: Optional[Input] = None,
     ):
-        super().__init__(ComponentType.NAND, component_id, position, 0.75)
+        super().__init__(ComponentType.Divide, component_id, position, 0.75)
         self.a_input: Optional[Input] = a_input
         self.b_input: Optional[Input] = b_input
 
     @staticmethod
-    def from_xml(element: XMLParserElement) -> NAND:
-        assert element.tag == "c", f"invalid NAND {element}"
+    def from_xml(element: XMLParserElement) -> Divide:
+        assert element.tag == "c", f"invalid Divide {element}"
         assert element.attributes.get("type", "0") == str(
-            ComponentType.NAND.value
-        ), f"Not an NAND {element}"
+            ComponentType.Divide.value
+        ), f"Not an Divide {element}"
         obj: XMLParserElement = element.children[0]
-        component_id, position, inputs, _ = NAND._basic_in_parsing(obj)
-        return NAND(component_id, position, inputs.get("1"), inputs.get("2"))
+        component_id, position, inputs, _ = Divide._basic_in_parsing(obj)
+        return Divide(component_id, position, inputs.get("1"), inputs.get("2"))
 
     def _inner_to_xml(self) -> INNER_TO_XML_RESULT:
         return {}, self._pos_in_to_xml(self.a_input, self.b_input)
```

### Comparing `sw_mc_lib-0.1/sw_mc_lib/Components/NOR.py` & `sw_mc_lib-0.2.0/sw_mc_lib/Components/AND.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,31 +5,35 @@
 from sw_mc_lib.Component import INNER_TO_XML_RESULT, Component
 from sw_mc_lib.Input import Input
 from sw_mc_lib.Position import Position
 from sw_mc_lib.Types import ComponentType
 from sw_mc_lib.XMLParser import XMLParserElement
 
 
-class NOR(Component):
+class AND(Component):
+    """
+    Outputs the logical AND of its two input signals.
+    """
+
     def __init__(
         self,
         component_id: int,
         position: Position,
         a_input: Optional[Input] = None,
         b_input: Optional[Input] = None,
     ):
-        super().__init__(ComponentType.NOR, component_id, position, 0.75)
+        super().__init__(ComponentType.AND, component_id, position, 0.75)
         self.a_input: Optional[Input] = a_input
         self.b_input: Optional[Input] = b_input
 
     @staticmethod
-    def from_xml(element: XMLParserElement) -> NOR:
-        assert element.tag == "c", f"invalid NOR {element}"
+    def from_xml(element: XMLParserElement) -> AND:
+        assert element.tag == "c", f"invalid AND {element}"
         assert element.attributes.get("type", "0") == str(
-            ComponentType.NOR.value
-        ), f"Not an NOR {element}"
+            ComponentType.AND.value
+        ), f"Not an AND {element}"
         obj: XMLParserElement = element.children[0]
-        component_id, position, inputs, _ = NOR._basic_in_parsing(obj)
-        return NOR(component_id, position, inputs.get("1"), inputs.get("2"))
+        component_id, position, inputs, _ = AND._basic_in_parsing(obj)
+        return AND(component_id, position, inputs.get("1"), inputs.get("2"))
 
     def _inner_to_xml(self) -> INNER_TO_XML_RESULT:
         return {}, self._pos_in_to_xml(self.a_input, self.b_input)
```

### Comparing `sw_mc_lib-0.1/sw_mc_lib/Components/NOT.py` & `sw_mc_lib-0.2.0/sw_mc_lib/Components/Delta.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,26 +5,30 @@
 from sw_mc_lib.Component import INNER_TO_XML_RESULT, Component
 from sw_mc_lib.Input import Input
 from sw_mc_lib.Position import Position
 from sw_mc_lib.Types import ComponentType
 from sw_mc_lib.XMLParser import XMLParserElement
 
 
-class NOT(Component):
+class Delta(Component):
+    """
+    Outputs the difference between the input and the input from the previous tick.
+    """
+
     def __init__(
-        self, component_id: int, position: Position, a_input: Optional[Input] = None
+        self, component_id: int, position: Position, value_input: Optional[Input] = None
     ):
-        super().__init__(ComponentType.NOT, component_id, position, 0.5)
-        self.a_input: Optional[Input] = a_input
+        super().__init__(ComponentType.Delta, component_id, position, 0.5)
+        self.value_input: Optional[Input] = value_input
 
     @staticmethod
-    def from_xml(element: XMLParserElement) -> NOT:
-        assert element.tag == "c", f"invalid NOT {element}"
+    def from_xml(element: XMLParserElement) -> Delta:
+        assert element.tag == "c", f"invalid Delta {element}"
         assert element.attributes.get("type", "0") == str(
-            ComponentType.NOT.value
-        ), f"Not an NOT {element}"
+            ComponentType.Delta.value
+        ), f"Not an Delta {element}"
         obj: XMLParserElement = element.children[0]
-        component_id, position, inputs, _ = NOT._basic_in_parsing(obj)
-        return NOT(component_id, position, inputs.get("1"))
+        component_id, position, inputs, _ = Delta._basic_in_parsing(obj)
+        return Delta(component_id, position, inputs.get("1"))
 
     def _inner_to_xml(self) -> INNER_TO_XML_RESULT:
-        return {}, self._pos_in_to_xml(self.a_input)
+        return {}, self._pos_in_to_xml(self.value_input)
```

### Comparing `sw_mc_lib-0.1/sw_mc_lib/Components/NumberToCompositeBinary.py` & `sw_mc_lib-0.2.0/sw_mc_lib/Components/NumberToCompositeBinary.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,14 +6,18 @@
 from sw_mc_lib.Input import Input
 from sw_mc_lib.Position import Position
 from sw_mc_lib.Types import ComponentType
 from sw_mc_lib.XMLParser import XMLParserElement
 
 
 class NumberToCompositeBinary(Component):
+    """
+    Converts a number (rounded) to binary and outputs the bits as composite on/off signals.
+    """
+
     def __init__(
         self,
         component_id: int,
         position: Position,
         number_to_convert_input: Optional[Input] = None,
     ):
         super().__init__(
```

### Comparing `sw_mc_lib-0.1/sw_mc_lib/Components/NumericalJunction.py` & `sw_mc_lib-0.2.0/sw_mc_lib/Components/NumericalJunction.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,14 +6,19 @@
 from sw_mc_lib.Input import Input
 from sw_mc_lib.Position import Position
 from sw_mc_lib.Types import ComponentType
 from sw_mc_lib.XMLParser import XMLParserElement
 
 
 class NumericalJunction(Component):
+    """
+    Outputs the input number to one of the outputs depending on whether or not the Switch Signal is on.
+    The path that the input doesn't take will output a value of 0.
+    """
+
     def __init__(
         self,
         component_id: int,
         position: Position,
         value_to_pass_through_input: Optional[Input] = None,
         switch_signal_input: Optional[Input] = None,
     ):
```

### Comparing `sw_mc_lib-0.1/sw_mc_lib/Components/NumericalSwitchbox.py` & `sw_mc_lib-0.2.0/sw_mc_lib/Components/CompositeSwitchbox.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,42 +5,46 @@
 from sw_mc_lib.Component import INNER_TO_XML_RESULT, Component
 from sw_mc_lib.Input import Input
 from sw_mc_lib.Position import Position
 from sw_mc_lib.Types import ComponentType
 from sw_mc_lib.XMLParser import XMLParserElement
 
 
-class NumericalSwitchbox(Component):
+class CompositeSwitchbox(Component):
+    """
+    Outputs the first input composite when receiving an on signal, and the second when receiving an off signal.
+    """
+
     def __init__(
         self,
         component_id: int,
         position: Position,
         on_value_input: Optional[Input] = None,
         off_value_input: Optional[Input] = None,
         switch_signal_input: Optional[Input] = None,
     ):
-        super().__init__(ComponentType.NumericalSwitchbox, component_id, position, 1.0)
+        super().__init__(ComponentType.CompositeSwitchbox, component_id, position, 1.0)
         self.on_value_input: Optional[Input] = on_value_input
         self.off_value_input: Optional[Input] = off_value_input
         self.switch_signal_input: Optional[Input] = switch_signal_input
 
     @staticmethod
-    def from_xml(element: XMLParserElement) -> NumericalSwitchbox:
-        assert element.tag == "c", f"invalid NumericalSwitchbox {element}"
+    def from_xml(element: XMLParserElement) -> CompositeSwitchbox:
+        assert element.tag == "c", f"invalid CompositeSwitchbox {element}"
         assert element.attributes.get("type", "0") == str(
-            ComponentType.NumericalSwitchbox.value
-        ), f"Not an NumericalSwitchbox {element}"
+            ComponentType.CompositeSwitchbox.value
+        ), f"Not an CompositeSwitchbox {element}"
         obj: XMLParserElement = element.children[0]
         (
             component_id,
             position,
             inputs,
             _,
-        ) = NumericalSwitchbox._basic_in_parsing(obj)
-        return NumericalSwitchbox(
+        ) = CompositeSwitchbox._basic_in_parsing(obj)
+        return CompositeSwitchbox(
             component_id, position, inputs.get("1"), inputs.get("2"), inputs.get("3")
         )
 
     def _inner_to_xml(self) -> INNER_TO_XML_RESULT:
         return {}, self._pos_in_to_xml(
             self.on_value_input, self.off_value_input, self.switch_signal_input
         )
```

### Comparing `sw_mc_lib-0.1/sw_mc_lib/Components/OR.py` & `sw_mc_lib-0.2.0/sw_mc_lib/Components/TimerTOF.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,45 @@
 from __future__ import annotations
 
 from typing import Optional
 
 from sw_mc_lib.Component import INNER_TO_XML_RESULT, Component
 from sw_mc_lib.Input import Input
 from sw_mc_lib.Position import Position
-from sw_mc_lib.Types import ComponentType
+from sw_mc_lib.Types import ComponentType, TimerUnit
 from sw_mc_lib.XMLParser import XMLParserElement
 
 
-class OR(Component):
+class TimerTOF(Component):
+    """
+    Variable input timer. Outputs an on signal when the timer is less than its duration.
+    The timer will reset when off.
+    """
+
     def __init__(
         self,
         component_id: int,
         position: Position,
-        a_input: Optional[Input] = None,
-        b_input: Optional[Input] = None,
+        unit_property: TimerUnit = TimerUnit.Seconds,
+        timer_enable_input: Optional[Input] = None,
+        duration_input: Optional[Input] = None,
     ):
-        super().__init__(ComponentType.OR, component_id, position, 0.75)
-        self.a_input: Optional[Input] = a_input
-        self.b_input: Optional[Input] = b_input
+        super().__init__(ComponentType.TimerTOF, component_id, position, 0.75)
+        self.timer_enable_input: Optional[Input] = timer_enable_input
+        self.duration_input: Optional[Input] = duration_input
+        self.unit_property: TimerUnit = unit_property
 
     @staticmethod
-    def from_xml(element: XMLParserElement) -> OR:
-        assert element.tag == "c", f"invalid OR {element}"
+    def from_xml(element: XMLParserElement) -> TimerTOF:
+        assert element.tag == "c", f"invalid TimerTOF {element}"
         assert element.attributes.get("type", "0") == str(
-            ComponentType.OR.value
-        ), f"Not an OR {element}"
+            ComponentType.TimerTOF.value
+        ), f"Not an TimerTOF {element}"
         obj: XMLParserElement = element.children[0]
-        component_id, position, inputs, _ = OR._basic_in_parsing(obj)
-        return OR(component_id, position, inputs.get("1"), inputs.get("2"))
+        component_id, position, inputs, _ = TimerTOF._basic_in_parsing(obj)
+        unit_property: TimerUnit = TimerUnit(int(obj.attributes.get("u", "0")))
+        return TimerTOF(
+            component_id, position, unit_property, inputs.get("1"), inputs.get("2")
+        )
 
     def _inner_to_xml(self) -> INNER_TO_XML_RESULT:
-        return {}, self._pos_in_to_xml(self.a_input, self.b_input)
+        return {}, self._pos_in_to_xml(self.timer_enable_input, self.duration_input)
```

### Comparing `sw_mc_lib-0.1/sw_mc_lib/Components/PIDController.py` & `sw_mc_lib-0.2.0/sw_mc_lib/Components/PIDController.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,18 @@
 from sw_mc_lib.NumberProperty import NumberProperty
 from sw_mc_lib.Position import Position
 from sw_mc_lib.Types import ComponentType
 from sw_mc_lib.XMLParser import XMLParserElement
 
 
 class PIDController(Component):
+    """
+    A basic PID controller. The proportional, integral and derivative gains can be set in the property panel.
+    """
+
     def __init__(
         self,
         component_id: int,
         position: Position,
         setpoint_input: Optional[Input] = None,
         process_variable_input: Optional[Input] = None,
         active_input: Optional[Input] = None,
```

### Comparing `sw_mc_lib-0.1/sw_mc_lib/Components/PIDControllerAdvanced.py` & `sw_mc_lib-0.2.0/sw_mc_lib/Components/PIDControllerAdvanced.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,18 @@
 from sw_mc_lib.Input import Input
 from sw_mc_lib.Position import Position
 from sw_mc_lib.Types import ComponentType
 from sw_mc_lib.XMLParser import XMLParserElement
 
 
 class PIDControllerAdvanced(Component):
+    """
+    A PID controller with variable proportional, integral and derivative gains.
+    """
+
     def __init__(
         self,
         component_id: int,
         position: Position,
         setpoint_input: Optional[Input] = None,
         process_variable_input: Optional[Input] = None,
         proportional_input: Optional[Input] = None,
```

### Comparing `sw_mc_lib-0.1/sw_mc_lib/Components/PropertyDropdown.py` & `sw_mc_lib-0.2.0/sw_mc_lib/Components/PropertyDropdown.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,14 +7,18 @@
 from sw_mc_lib.Position import Position
 from sw_mc_lib.Types import ComponentType
 from sw_mc_lib.XMLElement import XMLElement
 from sw_mc_lib.XMLParser import XMLParserElement
 
 
 class DropDownOption(XMLElement):
+    """
+    A single Option for :class:`sw_mc_lib.Components.PropertyDropDown.PropertyDropDown`
+    """
+
     def __init__(self, label: str, value_property: Optional[NumberProperty]):
         self.label: str = label
         self.value_property: NumberProperty = value_property or NumberProperty("0", "v")
 
     @staticmethod
     def from_xml(element: XMLParserElement) -> DropDownOption:
         assert element.tag == "i", f"invalid DropDownOption {element}"
@@ -26,14 +30,18 @@
         return DropDownOption(label, value_property)
 
     def to_xml(self) -> XMLParserElement:
         return XMLParserElement("i", {"l": self.label}, [self.value_property.to_xml()])
 
 
 class PropertyDropdown(Component):
+    """
+    Adds a custom dropdown list that will be seen on the microcontroller's property panel when placed on a vehicle.
+    """
+
     def __init__(
         self,
         component_id: int,
         position: Position,
         selected_property: int = 0,
         options: Optional[list[DropDownOption]] = None,
     ):
```

### Comparing `sw_mc_lib-0.1/sw_mc_lib/Components/PropertyNumber.py` & `sw_mc_lib-0.2.0/sw_mc_lib/Components/PropertyText.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 from __future__ import annotations
 
-from typing import Optional
-
-from sw_mc_lib.Component import INNER_TO_XML_RESULT
-from sw_mc_lib.NumberProperty import NumberProperty
+from sw_mc_lib.Component import INNER_TO_XML_RESULT, Component
 from sw_mc_lib.Position import Position
 from sw_mc_lib.Types import ComponentType
 from sw_mc_lib.XMLParser import XMLParserElement
 
-from .SubTypes.ValueComponent import ValueComponent
 
+class PropertyText(Component):
+    """
+    Adds a custom text input that will be seen on the microcontroller's property panel when placed on a vehicle,
+    for showing player-defined text within a lua script.
+    """
 
-class PropertyNumber(ValueComponent):
     def __init__(
         self,
         component_id: int,
         position: Position,
-        name: str = "number",
-        value_property: Optional[NumberProperty] = None,
+        name: str = "Label",
+        value_property: str = "",
     ):
-        super().__init__(
-            ComponentType.PropertyNumber, component_id, position, 0.5, value_property
-        )
+        super().__init__(ComponentType.PropertyText, component_id, position, 0.5)
         self.name: str = name
+        self.value_property: str = value_property
 
     @staticmethod
-    def from_xml(element: XMLParserElement) -> PropertyNumber:
-        assert element.tag == "c", f"invalid PropertyNumber {element}"
+    def from_xml(element: XMLParserElement) -> PropertyText:
+        assert element.tag == "c", f"invalid PropertyText {element}"
         assert element.attributes.get("type", "0") == str(
-            ComponentType.PropertyNumber.value
-        ), f"Not an PropertyNumber {element}"
+            ComponentType.PropertyText.value
+        ), f"Not an PropertyText {element}"
         obj: XMLParserElement = element.children[0]
-        component_id, position, _, properties = PropertyNumber._basic_in_parsing(obj)
-        name: str = obj.attributes.get("n", "number")
-        value_property = PropertyNumber._basic_value_parsing(properties)
-        return PropertyNumber(component_id, position, name, value_property)
+        component_id, position, _, _ = PropertyText._basic_in_parsing(obj)
+        name: str = obj.attributes.get("n", "toggle")
+        value_property: str = obj.attributes.get("v", "")
+        return PropertyText(component_id, position, name, value_property)
 
     def _inner_to_xml(self) -> INNER_TO_XML_RESULT:
+        attributes: dict[str, str] = {
+            "n": self.name,
+            "v": self.value_property,
+        }
         children: list[XMLParserElement] = self._pos_in_to_xml()
-        children.extend(self._value_to_xml())
-        return {}, children
+        return attributes, children
```

### Comparing `sw_mc_lib-0.1/sw_mc_lib/Components/PropertySlider.py` & `sw_mc_lib-0.2.0/sw_mc_lib/Components/PropertySlider.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,14 +9,18 @@
 from sw_mc_lib.XMLParser import XMLParserElement
 
 from .SubTypes.MinMaxComponent import MinMaxComponent
 from .SubTypes.ValueComponent import ValueComponent
 
 
 class PropertySlider(MinMaxComponent, ValueComponent):
+    """
+    Adds a custom slider that will be seen on the microcontroller's property panel when placed on a vehicle.
+    """
+
     def __init__(
         self,
         component_id: int,
         position: Position,
         min_property: Optional[NumberProperty] = None,
         max_property: Optional[NumberProperty] = None,
         value_property: Optional[NumberProperty] = None,
```

### Comparing `sw_mc_lib-0.1/sw_mc_lib/Components/PropertyText.py` & `sw_mc_lib-0.2.0/sw_mc_lib/Components/SubTypes/ValueComponent.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,39 +1,37 @@
 from __future__ import annotations
 
-from sw_mc_lib.Component import INNER_TO_XML_RESULT, Component
+from abc import ABC
+from typing import Optional
+
+from sw_mc_lib.Component import Component
+from sw_mc_lib.NumberProperty import NumberProperty
 from sw_mc_lib.Position import Position
 from sw_mc_lib.Types import ComponentType
 from sw_mc_lib.XMLParser import XMLParserElement
 
 
-class PropertyText(Component):
+class ValueComponent(Component, ABC):
+    """
+    A Component that has a value property.
+    """
+
     def __init__(
         self,
+        component_type: ComponentType,
         component_id: int,
         position: Position,
-        name: str = "Label",
-        value_property: str = "",
+        height: float,
+        value_property: Optional[NumberProperty] = None,
+        **kwargs: Optional[NumberProperty],
     ):
-        super().__init__(ComponentType.PropertyText, component_id, position, 0.5)
-        self.name: str = name
-        self.value_property: str = value_property
+        super().__init__(component_type, component_id, position, height, **kwargs)
+        self.value_property: NumberProperty = value_property or NumberProperty("0", "v")
 
     @staticmethod
-    def from_xml(element: XMLParserElement) -> PropertyText:
-        assert element.tag == "c", f"invalid PropertyText {element}"
-        assert element.attributes.get("type", "0") == str(
-            ComponentType.PropertyText.value
-        ), f"Not an PropertyText {element}"
-        obj: XMLParserElement = element.children[0]
-        component_id, position, _, _ = PropertyText._basic_in_parsing(obj)
-        name: str = obj.attributes.get("n", "toggle")
-        value_property: str = obj.attributes.get("v", "")
-        return PropertyText(component_id, position, name, value_property)
-
-    def _inner_to_xml(self) -> INNER_TO_XML_RESULT:
-        attributes: dict[str, str] = {
-            "n": self.name,
-            "v": self.value_property,
-        }
-        children: list[XMLParserElement] = self._pos_in_to_xml()
-        return attributes, children
+    def _basic_value_parsing(
+        properties: dict[str, NumberProperty]
+    ) -> Optional[NumberProperty]:
+        return properties.get("v")
+
+    def _value_to_xml(self) -> list[XMLParserElement]:
+        return [self.value_property.to_xml()]
```

### Comparing `sw_mc_lib-0.1/sw_mc_lib/Components/PropertyToggle.py` & `sw_mc_lib-0.2.0/sw_mc_lib/Components/PropertyToggle.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 from sw_mc_lib.Component import INNER_TO_XML_RESULT, Component
 from sw_mc_lib.Position import Position
 from sw_mc_lib.Types import ComponentType
 from sw_mc_lib.XMLParser import XMLParserElement
 
 
 class PropertyToggle(Component):
+    """
+    Adds a custom on/off toggle that will be seen on the microcontroller's property panel when placed on a vehicle.
+    """
+
     def __init__(
         self,
         component_id: int,
         position: Position,
         name: str = "toggle",
         on_label: str = "on",
         off_label: str = "off",
```

### Comparing `sw_mc_lib-0.1/sw_mc_lib/Components/Pulse.py` & `sw_mc_lib-0.2.0/sw_mc_lib/Components/VideoSwitchbox.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,38 +1,50 @@
 from __future__ import annotations
 
 from typing import Optional
 
 from sw_mc_lib.Component import INNER_TO_XML_RESULT, Component
 from sw_mc_lib.Input import Input
 from sw_mc_lib.Position import Position
-from sw_mc_lib.Types import ComponentType, PulseMode
+from sw_mc_lib.Types import ComponentType
 from sw_mc_lib.XMLParser import XMLParserElement
 
 
-class Pulse(Component):
+class VideoSwitchbox(Component):
+    """
+    Outputs the first input video when receiving an on signal, and the second when receiving an off signal.
+    """
+
     def __init__(
         self,
         component_id: int,
         position: Position,
-        mode_property: PulseMode = PulseMode.OffToOn,
-        toggle_signal_input: Optional[Input] = None,
+        on_value_input: Optional[Input] = None,
+        off_value_input: Optional[Input] = None,
+        switch_signal_input: Optional[Input] = None,
     ):
-        super().__init__(ComponentType.Pulse, component_id, position, 0.5)
-        self.toggle_signal_input: Optional[Input] = toggle_signal_input
-        self.mode_property: PulseMode = mode_property
+        super().__init__(ComponentType.VideoSwitchbox, component_id, position, 1.0)
+        self.on_value_input: Optional[Input] = on_value_input
+        self.off_value_input: Optional[Input] = off_value_input
+        self.switch_signal_input: Optional[Input] = switch_signal_input
 
     @staticmethod
-    def from_xml(element: XMLParserElement) -> Pulse:
-        assert element.tag == "c", f"invalid Pulse {element}"
+    def from_xml(element: XMLParserElement) -> VideoSwitchbox:
+        assert element.tag == "c", f"invalid VideoSwitchbox {element}"
         assert element.attributes.get("type", "0") == str(
-            ComponentType.Pulse.value
-        ), f"Not an Pulse {element}"
+            ComponentType.VideoSwitchbox.value
+        ), f"Not an VideoSwitchbox {element}"
         obj: XMLParserElement = element.children[0]
-        component_id, position, inputs, _ = Pulse._basic_in_parsing(obj)
-        mode_property: PulseMode = PulseMode(int(obj.attributes.get("m", "1")))
-        return Pulse(component_id, position, mode_property, inputs.get("1"))
+        (
+            component_id,
+            position,
+            inputs,
+            _,
+        ) = VideoSwitchbox._basic_in_parsing(obj)
+        return VideoSwitchbox(
+            component_id, position, inputs.get("1"), inputs.get("2"), inputs.get("3")
+        )
 
     def _inner_to_xml(self) -> INNER_TO_XML_RESULT:
-        return {"m": str(self.mode_property.value)}, self._pos_in_to_xml(
-            self.toggle_signal_input
+        return {}, self._pos_in_to_xml(
+            self.on_value_input, self.off_value_input, self.switch_signal_input
         )
```

### Comparing `sw_mc_lib-0.1/sw_mc_lib/Components/PushToToggle.py` & `sw_mc_lib-0.2.0/sw_mc_lib/Components/PushToToggle.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,14 +6,18 @@
 from sw_mc_lib.Input import Input
 from sw_mc_lib.Position import Position
 from sw_mc_lib.Types import ComponentType
 from sw_mc_lib.XMLParser import XMLParserElement
 
 
 class PushToToggle(Component):
+    """
+    An on/off switch that is toggled every time a new on signal is sent to its input.
+    """
+
     def __init__(
         self, component_id: int, position: Position, a_input: Optional[Input] = None
     ):
         super().__init__(ComponentType.PushToToggle, component_id, position, 0.5)
         self.a_input: Optional[Input] = a_input
 
     @staticmethod
```

### Comparing `sw_mc_lib-0.1/sw_mc_lib/Components/SRLatch.py` & `sw_mc_lib-0.2.0/sw_mc_lib/Components/TimerTON.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,35 +1,44 @@
 from __future__ import annotations
 
 from typing import Optional
 
 from sw_mc_lib.Component import INNER_TO_XML_RESULT, Component
 from sw_mc_lib.Input import Input
 from sw_mc_lib.Position import Position
-from sw_mc_lib.Types import ComponentType
+from sw_mc_lib.Types import ComponentType, TimerUnit
 from sw_mc_lib.XMLParser import XMLParserElement
 
 
-class SRLatch(Component):
+class TimerTON(Component):
+    """
+    Variable input timer. Outputs an on signal when the timer reaches its duration. The timer will reset when off.
+    """
+
     def __init__(
         self,
         component_id: int,
         position: Position,
-        set_input: Optional[Input] = None,
-        reset_input: Optional[Input] = None,
+        unit_property: TimerUnit = TimerUnit.Seconds,
+        timer_enable_input: Optional[Input] = None,
+        duration_input: Optional[Input] = None,
     ):
-        super().__init__(ComponentType.SRLatch, component_id, position, 0.75)
-        self.set_input: Optional[Input] = set_input
-        self.reset_input: Optional[Input] = reset_input
+        super().__init__(ComponentType.TimerTON, component_id, position, 0.75)
+        self.timer_enable_input: Optional[Input] = timer_enable_input
+        self.duration_input: Optional[Input] = duration_input
+        self.unit_property: TimerUnit = unit_property
 
     @staticmethod
-    def from_xml(element: XMLParserElement) -> SRLatch:
-        assert element.tag == "c", f"invalid SRLatch {element}"
+    def from_xml(element: XMLParserElement) -> TimerTON:
+        assert element.tag == "c", f"invalid TimerTON {element}"
         assert element.attributes.get("type", "0") == str(
-            ComponentType.SRLatch.value
-        ), f"Not an SRLatch {element}"
+            ComponentType.TimerTON.value
+        ), f"Not an TimerTON {element}"
         obj: XMLParserElement = element.children[0]
-        component_id, position, inputs, _ = SRLatch._basic_in_parsing(obj)
-        return SRLatch(component_id, position, inputs.get("1"), inputs.get("2"))
+        component_id, position, inputs, _ = TimerTON._basic_in_parsing(obj)
+        unit_property: TimerUnit = TimerUnit(int(obj.attributes.get("u", "0")))
+        return TimerTON(
+            component_id, position, unit_property, inputs.get("1"), inputs.get("2")
+        )
 
     def _inner_to_xml(self) -> INNER_TO_XML_RESULT:
-        return {}, self._pos_in_to_xml(self.set_input, self.reset_input)
+        return {}, self._pos_in_to_xml(self.timer_enable_input, self.duration_input)
```

### Comparing `sw_mc_lib-0.1/sw_mc_lib/Components/SubTypes/MinMaxComponent.py` & `sw_mc_lib-0.2.0/sw_mc_lib/Components/SubTypes/MinMaxComponent.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,18 @@
 from sw_mc_lib.NumberProperty import NumberProperty
 from sw_mc_lib.Position import Position
 from sw_mc_lib.Types import ComponentType
 from sw_mc_lib.XMLParser import XMLParserElement
 
 
 class MinMaxComponent(Component, ABC):
+    """
+    A Component that has a min and max Property.
+    """
+
     def __init__(
         self,
         component_type: ComponentType,
         component_id: int,
         position: Position,
         height: float,
         min_property: Optional[NumberProperty] = None,
```

### Comparing `sw_mc_lib-0.1/sw_mc_lib/Components/SubTypes/ResetComponent.py` & `sw_mc_lib-0.2.0/sw_mc_lib/Components/SubTypes/ResetComponent.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,18 @@
 from sw_mc_lib.NumberProperty import NumberProperty
 from sw_mc_lib.Position import Position
 from sw_mc_lib.Types import ComponentType
 from sw_mc_lib.XMLParser import XMLParserElement
 
 
 class ResetComponent(Component, ABC):
+    """
+    A Component that has a reset value property.
+    """
+
     def __init__(
         self,
         component_type: ComponentType,
         component_id: int,
         position: Position,
         height: float,
         reset_property: Optional[NumberProperty],
```

### Comparing `sw_mc_lib-0.1/sw_mc_lib/Components/Subtract.py` & `sw_mc_lib-0.2.0/sw_mc_lib/Components/Subtract.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,18 @@
 from sw_mc_lib.Input import Input
 from sw_mc_lib.Position import Position
 from sw_mc_lib.Types import ComponentType
 from sw_mc_lib.XMLParser import XMLParserElement
 
 
 class Subtract(Component):
+    """
+    Subtracts the second input from the first and outputs the result.
+    """
+
     def __init__(
         self,
         component_id: int,
         position: Position,
         a_input: Optional[Input] = None,
         b_input: Optional[Input] = None,
     ):
```

### Comparing `sw_mc_lib-0.1/sw_mc_lib/Components/Threshold.py` & `sw_mc_lib-0.2.0/sw_mc_lib/Components/Threshold.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,14 +9,18 @@
 from sw_mc_lib.Types import ComponentType
 from sw_mc_lib.XMLParser import XMLParserElement
 
 from .SubTypes.MinMaxComponent import MinMaxComponent
 
 
 class Threshold(MinMaxComponent):
+    """
+    Outputs an on/off signal indicating whether or not the input value is within a set threshold.
+    """
+
     def __init__(
         self,
         component_id: int,
         position: Position,
         min_property: Optional[NumberProperty] = None,
         max_property: Optional[NumberProperty] = None,
         number_input: Optional[Input] = None,
```

### Comparing `sw_mc_lib-0.1/sw_mc_lib/Components/TooltipBoolean.py` & `sw_mc_lib-0.2.0/sw_mc_lib/Components/TooltipBoolean.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,14 +6,19 @@
 from sw_mc_lib.Input import Input
 from sw_mc_lib.Position import Position
 from sw_mc_lib.Types import ComponentType, TooltipMode
 from sw_mc_lib.XMLParser import XMLParserElement
 
 
 class TooltipBoolean(Component):
+    """
+    Displays an on/off signal on this microcontroller's tooltip when it is looked at by the player
+    on a spawned vehicle.
+    """
+
     def __init__(
         self,
         component_id: int,
         position: Position,
         label_property: str = "value",
         on_label_property: str = "on",
         off_label_property: str = "off",
```

### Comparing `sw_mc_lib-0.1/sw_mc_lib/Components/TooltipNumber.py` & `sw_mc_lib-0.2.0/sw_mc_lib/Components/TooltipNumber.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,14 +6,18 @@
 from sw_mc_lib.Input import Input
 from sw_mc_lib.Position import Position
 from sw_mc_lib.Types import ComponentType, TooltipMode
 from sw_mc_lib.XMLParser import XMLParserElement
 
 
 class TooltipNumber(Component):
+    """
+    Displays a number on this microcontroller's tooltip when it is looked at by the player on a spawned vehicle.
+    """
+
     def __init__(
         self,
         component_id: int,
         position: Position,
         label_property: str = "value",
         mode_property: TooltipMode = TooltipMode.Always,
         display_number_input: Optional[Input] = None,
```

### Comparing `sw_mc_lib-0.1/sw_mc_lib/Components/UpDownCounter.py` & `sw_mc_lib-0.2.0/sw_mc_lib/Components/UpDownCounter.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,18 @@
 from sw_mc_lib.XMLParser import XMLParserElement
 
 from .SubTypes.MinMaxComponent import MinMaxComponent
 from .SubTypes.ResetComponent import ResetComponent
 
 
 class UpDownCounter(MinMaxComponent, ResetComponent):
+    """
+    Has an internal value that will increase and decrease when receiving different signals.
+    """
+
     def __init__(
         self,
         component_id: int,
         position: Position,
         up_input: Optional[Input] = None,
         down_input: Optional[Input] = None,
         reset_input: Optional[Input] = None,
```

### Comparing `sw_mc_lib-0.1/sw_mc_lib/Components/VideoSwitchbox.py` & `sw_mc_lib-0.2.0/sw_mc_lib/Components/AudioSwitchbox.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,42 +5,46 @@
 from sw_mc_lib.Component import INNER_TO_XML_RESULT, Component
 from sw_mc_lib.Input import Input
 from sw_mc_lib.Position import Position
 from sw_mc_lib.Types import ComponentType
 from sw_mc_lib.XMLParser import XMLParserElement
 
 
-class VideoSwitchbox(Component):
+class AudioSwitchbox(Component):
+    """
+    Outputs the first input audio when receiving an on signal, and the second when receiving an off signal.
+    """
+
     def __init__(
         self,
         component_id: int,
         position: Position,
         on_value_input: Optional[Input] = None,
         off_value_input: Optional[Input] = None,
         switch_signal_input: Optional[Input] = None,
     ):
-        super().__init__(ComponentType.VideoSwitchbox, component_id, position, 1.0)
+        super().__init__(ComponentType.AudioSwitchbox, component_id, position, 1.0)
         self.on_value_input: Optional[Input] = on_value_input
         self.off_value_input: Optional[Input] = off_value_input
         self.switch_signal_input: Optional[Input] = switch_signal_input
 
     @staticmethod
-    def from_xml(element: XMLParserElement) -> VideoSwitchbox:
-        assert element.tag == "c", f"invalid VideoSwitchbox {element}"
+    def from_xml(element: XMLParserElement) -> AudioSwitchbox:
+        assert element.tag == "c", f"invalid AudioSwitchbox {element}"
         assert element.attributes.get("type", "0") == str(
-            ComponentType.VideoSwitchbox.value
-        ), f"Not an VideoSwitchbox {element}"
+            ComponentType.AudioSwitchbox.value
+        ), f"Not an AudioSwitchbox {element}"
         obj: XMLParserElement = element.children[0]
         (
             component_id,
             position,
             inputs,
             _,
-        ) = VideoSwitchbox._basic_in_parsing(obj)
-        return VideoSwitchbox(
+        ) = AudioSwitchbox._basic_in_parsing(obj)
+        return AudioSwitchbox(
             component_id, position, inputs.get("1"), inputs.get("2"), inputs.get("3")
         )
 
     def _inner_to_xml(self) -> INNER_TO_XML_RESULT:
         return {}, self._pos_in_to_xml(
             self.on_value_input, self.off_value_input, self.switch_signal_input
         )
```

### Comparing `sw_mc_lib-0.1/sw_mc_lib/Components/XOR.py` & `sw_mc_lib-0.2.0/sw_mc_lib/Components/Modulo.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,31 +5,35 @@
 from sw_mc_lib.Component import INNER_TO_XML_RESULT, Component
 from sw_mc_lib.Input import Input
 from sw_mc_lib.Position import Position
 from sw_mc_lib.Types import ComponentType
 from sw_mc_lib.XMLParser import XMLParserElement
 
 
-class XOR(Component):
+class Modulo(Component):
+    """
+    Outputs the modulo of input A by input B.
+    """
+
     def __init__(
         self,
         component_id: int,
         position: Position,
         a_input: Optional[Input] = None,
         b_input: Optional[Input] = None,
     ):
-        super().__init__(ComponentType.XOR, component_id, position, 0.75)
+        super().__init__(ComponentType.Modulo, component_id, position, 0.75)
         self.a_input: Optional[Input] = a_input
         self.b_input: Optional[Input] = b_input
 
     @staticmethod
-    def from_xml(element: XMLParserElement) -> XOR:
-        assert element.tag == "c", f"invalid XOR {element}"
+    def from_xml(element: XMLParserElement) -> Modulo:
+        assert element.tag == "c", f"invalid Modulo {element}"
         assert element.attributes.get("type", "0") == str(
-            ComponentType.XOR.value
-        ), f"Not an XOR {element}"
+            ComponentType.Modulo.value
+        ), f"Not an Modulo {element}"
         obj: XMLParserElement = element.children[0]
-        component_id, position, inputs, _ = XOR._basic_in_parsing(obj)
-        return XOR(component_id, position, inputs.get("1"), inputs.get("2"))
+        component_id, position, inputs, _ = Modulo._basic_in_parsing(obj)
+        return Modulo(component_id, position, inputs.get("1"), inputs.get("2"))
 
     def _inner_to_xml(self) -> INNER_TO_XML_RESULT:
         return {}, self._pos_in_to_xml(self.a_input, self.b_input)
```

### Comparing `sw_mc_lib-0.1/sw_mc_lib/Components/__init__.py` & `sw_mc_lib-0.2.0/sw_mc_lib/Components/__init__.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.1/sw_mc_lib/Input.py` & `sw_mc_lib-0.2.0/sw_mc_lib/Input.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 
 from typing import Optional
 
 from .XMLElement import XMLElement, XMLParserElement
 
 
 class Input(XMLElement):
+    """
+    An input for a Component. Contains both component_id as well as node_index of the source.
+    """
+
     def __init__(
         self, component_id: int, node_index: int = 0, index: Optional[str] = None
     ):
         self.index: str = index or "temp"
         self.component_id: int = component_id
         self.node_index: int = node_index
```

### Comparing `sw_mc_lib-0.1/sw_mc_lib/Microcontroller.py` & `sw_mc_lib-0.2.0/sw_mc_lib/Microcontroller.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 
 from .Component import Component
 from .Node import Node
 from .XMLElement import XMLElement, XMLParserElement
 
 
 class Microcontroller(XMLElement):
+    """
+    A Stormworks Microcontroller
+    """
+
     def __init__(
         self,
         name: str,
         description: str,
         width: int,
         length: int,
         nodes: list[Node],
@@ -75,15 +79,25 @@
             "id_counter": str(self.id_counter),
             "id_counter_node": str(self.node_counter),
         }
         return XMLParserElement("microprocessor", attributes, [nodes_elem, group_elem])
 
     @property
     def id_counter(self) -> int:
+        """
+        Stormworks internal counter of what the largest component_id is.
+
+        :return: The currently largest component_id
+        """
         components = (comp.component_id for comp in self.components)
         nodes = (node.component_id for node in self.nodes)
         return max(chain(components, nodes, (0,)))
 
     @property
     def node_counter(self) -> int:
+        """
+        Stormworks internal counter of what the largest node_id is.
+
+        :return: The currently largest node_id
+        """
         nodes = (node.node_id for node in self.nodes)
         return max(chain(nodes, (0,)))
```

### Comparing `sw_mc_lib-0.1/sw_mc_lib/Node.py` & `sw_mc_lib-0.2.0/sw_mc_lib/Node.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,14 +4,19 @@
 
 from .Types import NodeMode, SignalType
 from .XMLElement import XMLElement
 from .XMLParser import XMLParserElement
 
 
 class NodePosition(XMLElement):
+    """
+    A Position for a node. This is distinct from :class:`sw_mc_lib.Position.Position` in that it has x, y and z, and
+    that they are integers instead of floats. You probably never need to use y.
+    """
+
     def __init__(self, x: int, y: int, z: int):
         self.x: int = x
         self.y: int = y
         self.z: int = z
 
     @staticmethod
     def from_xml(element: XMLParserElement) -> NodePosition:
@@ -30,14 +35,18 @@
             attributes["y"] = str(self.y)
         if self.z != 0:
             attributes["z"] = str(self.z)
         return XMLParserElement("position", attributes)
 
 
 class Node(XMLElement):
+    """
+    A Microcontroller node. Interface between Microcontroller and the rest of the Vehicle.
+    """
+
     def __init__(
         self,
         node_id: int,
         component_id: int,
         label: str,
         mode: int,
         type: int,
```

### Comparing `sw_mc_lib-0.1/sw_mc_lib/XMLFormatter.py` & `sw_mc_lib-0.2.0/sw_mc_lib/XMLFormatter.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 
 
 def _escape_string(to_escape: str) -> str:
     """
     Escapes a string so that it results in valid xml. To be used like following:
 
     `abc<>"def\n"` -> `'abc&lt;&gt;"def\n"'`
+
+    :param to_escape: The string that needs to be escaped
+    :return: Escaped string
     """
     to_escape = to_escape.replace("&", "&amp;")
     to_escape = to_escape.replace("<", "&lt;")
     to_escape = to_escape.replace(">", "&gt;")
     if to_escape.count('"') > to_escape.count("'"):
         to_escape = to_escape.replace("'", "&apos;")
         to_escape = f"'{to_escape}'"
@@ -20,17 +23,22 @@
         to_escape = f'"{to_escape}"'
     to_escape = to_escape.replace("\r\n", "\n")
     return to_escape
 
 
 def _indent(to_indent: str, indentation_character: str, line_breaks: str) -> str:
     """
-    Indents the string by one tab and adds a newline at the end
+    Indents the string by one tab and adds a newline at the end. Will only indent lines with `\r\n`
 
     `<node/>` -> `\t<node/>\n`
+
+    :param to_indent: XML block to indent
+    :param indentation_character: The character(s) to use for indentation
+    :param line_breaks: Either line breaks or empty string
+    :return: Indented text
     """
     return (
         "\r\n".join(
             indentation_character + line for line in to_indent.rstrip().split("\r\n")
         )
         + line_breaks
     )
@@ -53,14 +61,19 @@
 
 
 def format(
     element: XMLParserElement, indentation: Optional[str] = "\t", header: bool = False
 ) -> str:
     """
     Formats a XMLParserElement into a xml string. If indentation is None, there will be no line breaks or indentation.
-    If header is true, it will add a xml declaration at the top of the document
+    If header is true, it will add a xml declaration at the top of the document.
+
+    :param element: The XML element to format
+    :param indentation: The indentation character to use, `None` will not indent at all
+    :param header: Whether to include the XML Header
+    :return: XML string
     """
     line_breaks: str = "\r\n" if indentation is not None else ""
     indentation_character = indentation or ""
     xml: str = f'<?xml version="1.0" encoding="UTF-8"?>{line_breaks}' if header else ""
     xml += _inner_format(element, indentation_character, line_breaks)
     return xml.replace("\r\n", "\n")
```

### Comparing `sw_mc_lib-0.1/sw_mc_lib.egg-info/PKG-INFO` & `sw_mc_lib-0.2.0/sw_mc_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sw-mc-lib
-Version: 0.1
+Version: 0.2.0
 Summary: Library for interaction with Stormworks Microcontrollers
 Author: Fabian Wunsch
 License: MIT License
 Project-URL: homepage, https://github.com/stormworks-utils/sw_mc_lib
 Project-URL: repository, https://github.com/stormworks-utils/sw_mc_lib
 Keywords: stormworks,lib,microcontroller
 Classifier: Programming Language :: Python :: 3
@@ -20,7 +20,9 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # sw_mc_lib
 Stormworks Microcontroller library
+
+
```

### Comparing `sw_mc_lib-0.1/sw_mc_lib.egg-info/SOURCES.txt` & `sw_mc_lib-0.2.0/sw_mc_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.1/test/test_component.py` & `sw_mc_lib-0.2.0/test/test_component.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
 
 class TestComponent(unittest.TestCase):
     def test_basic_in_parsing(self) -> None:
         elem: XMLParserElement = XMLParserElement("object", {"id": "123"})
         expected: tuple[int, Position, dict[str, Input], dict[str, NumberProperty]] = (
             123,
-            Position.empty_pos(),
+            Position(),
             {},
             {},
         )
         self.assertEqual(Component._basic_in_parsing(elem), expected)
         elem.children.append(XMLParserElement("in1", {"component_id": "1"}))
         expected[2]["1"] = Input(1, 0, "1")
         self.assertEqual(Component._basic_in_parsing(elem), expected)
```

### Comparing `sw_mc_lib-0.1/test/test_input.py` & `sw_mc_lib-0.2.0/test/test_input.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.1/test/test_number_property.py` & `sw_mc_lib-0.2.0/test/test_number_property.py`

 * *Files identical despite different names*

### Comparing `sw_mc_lib-0.1/test/test_position.py` & `sw_mc_lib-0.2.0/test/test_position.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         expected.x = 1.25
         self.assertEqual(Position.from_xml(elem), expected)
         elem.attributes["y"] = "-4.75"
         expected.y = -4.75
         self.assertEqual(Position.from_xml(elem), expected)
 
     def test_empty_pos(self) -> None:
-        self.assertEqual(Position.empty_pos(), Position(0, 0))
+        self.assertEqual(Position(), Position(0, 0))
 
     def test_to_xml(self) -> None:
         elem: Position = Position(0, 0)
         expected: XMLParserElement = XMLParserElement("pos")
         self.assertEqual(elem.to_xml(), expected)
         elem.x = 1.25
         expected.attributes["x"] = "1.25"
```

### Comparing `sw_mc_lib-0.1/test/test_xml_formatter.py` & `sw_mc_lib-0.2.0/test/test_xml_formatter.py`

 * *Files identical despite different names*

