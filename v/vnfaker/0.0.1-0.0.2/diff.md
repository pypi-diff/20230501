# Comparing `tmp/vnfaker-0.0.1.tar.gz` & `tmp/vnfaker-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vnfaker-0.0.1.tar", last modified: Sat Apr 22 09:11:37 2023, max compression
+gzip compressed data, was "vnfaker-0.0.2.tar", last modified: Mon May  1 03:23:22 2023, max compression
```

## Comparing `vnfaker-0.0.1.tar` & `vnfaker-0.0.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-04-22 09:11:37.682939 vnfaker-0.0.1/
--rw-r--r--   0 ducquang   (501) admin       (80)     1056 2023-04-15 03:22:43.000000 vnfaker-0.0.1/LICENSE.txt
--rw-r--r--   0 ducquang   (501) admin       (80)     1812 2023-04-22 09:11:37.682429 vnfaker-0.0.1/PKG-INFO
--rw-r--r--   0 ducquang   (501) admin       (80)     1177 2023-04-22 08:57:04.000000 vnfaker-0.0.1/README.md
--rw-r--r--   0 ducquang   (501) admin       (80)       38 2023-04-22 09:11:37.683126 vnfaker-0.0.1/setup.cfg
--rw-r--r--   0 ducquang   (501) admin       (80)     1006 2023-04-22 09:11:21.000000 vnfaker-0.0.1/setup.py
-drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-04-22 09:11:37.655089 vnfaker-0.0.1/src/
-drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-04-22 09:11:37.658169 vnfaker-0.0.1/src/vnfaker/
--rw-r--r--   0 ducquang   (501) admin       (80)       70 2023-04-22 07:54:20.000000 vnfaker-0.0.1/src/vnfaker/__init__.py
--rw-r--r--   0 ducquang   (501) admin       (80)     3000 2023-04-22 07:28:33.000000 vnfaker-0.0.1/src/vnfaker/commonUtils.py
-drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-04-22 09:11:37.660769 vnfaker-0.0.1/src/vnfaker/data/
--rw-r--r--   0 ducquang   (501) admin       (80)        0 2023-04-10 18:01:14.000000 vnfaker-0.0.1/src/vnfaker/data/__init__.py
-drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-04-22 09:11:37.661687 vnfaker-0.0.1/src/vnfaker/data/company/
--rw-r--r--   0 ducquang   (501) admin       (80)        0 2023-04-10 18:01:35.000000 vnfaker-0.0.1/src/vnfaker/data/company/__init__.py
--rw-r--r--   0 ducquang   (501) admin       (80)     4748 2023-04-11 01:32:31.000000 vnfaker-0.0.1/src/vnfaker/data/company/company.name
-drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-04-22 09:11:37.662683 vnfaker-0.0.1/src/vnfaker/data/occupation/
--rw-r--r--   0 ducquang   (501) admin       (80)        0 2023-04-10 18:01:35.000000 vnfaker-0.0.1/src/vnfaker/data/occupation/__init__.py
--rw-r--r--   0 ducquang   (501) admin       (80)    34962 2023-04-11 06:57:16.000000 vnfaker-0.0.1/src/vnfaker/data/occupation/occupation.name
-drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-04-22 09:11:37.665963 vnfaker-0.0.1/src/vnfaker/data/person/
--rw-r--r--   0 ducquang   (501) admin       (80)        0 2023-04-10 18:01:35.000000 vnfaker-0.0.1/src/vnfaker/data/person/__init__.py
--rw-r--r--   0 ducquang   (501) admin       (80)     1136 2023-04-11 08:39:50.000000 vnfaker-0.0.1/src/vnfaker/data/person/female.name
--rw-r--r--   0 ducquang   (501) admin       (80)     1089 2023-04-11 08:42:28.000000 vnfaker-0.0.1/src/vnfaker/data/person/female_middle.name
--rw-r--r--   0 ducquang   (501) admin       (80)      111 2023-04-10 17:26:37.000000 vnfaker-0.0.1/src/vnfaker/data/person/first.name
--rw-r--r--   0 ducquang   (501) admin       (80)      148 2023-04-11 08:43:12.000000 vnfaker-0.0.1/src/vnfaker/data/person/last.name
--rw-r--r--   0 ducquang   (501) admin       (80)     1782 2023-04-11 08:36:23.000000 vnfaker-0.0.1/src/vnfaker/data/person/male.name
--rw-r--r--   0 ducquang   (501) admin       (80)     1178 2023-04-11 08:38:25.000000 vnfaker-0.0.1/src/vnfaker/data/person/male_middle.name
-drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-04-22 09:11:37.674480 vnfaker-0.0.1/src/vnfaker/data/provinces/
--rw-r--r--   0 ducquang   (501) admin       (80)        0 2023-04-10 18:01:35.000000 vnfaker-0.0.1/src/vnfaker/data/provinces/__init__.py
--rw-r--r--   0 ducquang   (501) admin       (80)  3512185 2023-04-10 17:48:23.000000 vnfaker-0.0.1/src/vnfaker/data/provinces/flat-divisions.json
--rw-r--r--   0 ducquang   (501) admin       (80)  2404923 2023-04-10 17:48:23.000000 vnfaker-0.0.1/src/vnfaker/data/provinces/nested-divisions.json
-drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-04-22 09:11:37.681164 vnfaker-0.0.1/src/vnfaker/data/sentence/
--rw-r--r--   0 ducquang   (501) admin       (80)        0 2023-04-10 18:01:14.000000 vnfaker-0.0.1/src/vnfaker/data/sentence/__init__.py
--rw-r--r--   0 ducquang   (501) admin       (80)   244103 2023-04-12 08:52:12.000000 vnfaker-0.0.1/src/vnfaker/data/sentence/sentence.txt
--rw-r--r--   0 ducquang   (501) admin       (80)     9017 2023-04-22 08:15:59.000000 vnfaker-0.0.1/src/vnfaker/generator.py
-drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-04-22 09:11:37.660211 vnfaker-0.0.1/src/vnfaker.egg-info/
--rw-r--r--   0 ducquang   (501) admin       (80)     1812 2023-04-22 09:11:37.000000 vnfaker-0.0.1/src/vnfaker.egg-info/PKG-INFO
--rw-r--r--   0 ducquang   (501) admin       (80)      939 2023-04-22 09:11:37.000000 vnfaker-0.0.1/src/vnfaker.egg-info/SOURCES.txt
--rw-r--r--   0 ducquang   (501) admin       (80)        1 2023-04-22 09:11:37.000000 vnfaker-0.0.1/src/vnfaker.egg-info/dependency_links.txt
--rw-r--r--   0 ducquang   (501) admin       (80)       15 2023-04-22 09:11:37.000000 vnfaker-0.0.1/src/vnfaker.egg-info/requires.txt
--rw-r--r--   0 ducquang   (501) admin       (80)        8 2023-04-22 09:11:37.000000 vnfaker-0.0.1/src/vnfaker.egg-info/top_level.txt
+drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-05-01 03:23:22.345397 vnfaker-0.0.2/
+-rw-r--r--   0 ducquang   (501) admin       (80)     1056 2023-04-15 03:22:43.000000 vnfaker-0.0.2/LICENSE.txt
+-rw-r--r--   0 ducquang   (501) admin       (80)     1812 2023-05-01 03:23:22.345156 vnfaker-0.0.2/PKG-INFO
+-rw-r--r--   0 ducquang   (501) admin       (80)     1177 2023-04-22 08:57:04.000000 vnfaker-0.0.2/README.md
+-rw-r--r--   0 ducquang   (501) admin       (80)       38 2023-05-01 03:23:22.345492 vnfaker-0.0.2/setup.cfg
+-rw-r--r--   0 ducquang   (501) admin       (80)     1006 2023-05-01 03:22:48.000000 vnfaker-0.0.2/setup.py
+drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-05-01 03:23:22.313522 vnfaker-0.0.2/src/
+drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-05-01 03:23:22.318135 vnfaker-0.0.2/src/vnfaker/
+-rw-r--r--   0 ducquang   (501) admin       (80)       70 2023-04-22 07:54:20.000000 vnfaker-0.0.2/src/vnfaker/__init__.py
+-rw-r--r--   0 ducquang   (501) admin       (80)     3000 2023-04-22 07:28:33.000000 vnfaker-0.0.2/src/vnfaker/commonUtils.py
+drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-05-01 03:23:22.320354 vnfaker-0.0.2/src/vnfaker/data/
+-rw-r--r--   0 ducquang   (501) admin       (80)        0 2023-04-10 18:01:14.000000 vnfaker-0.0.2/src/vnfaker/data/__init__.py
+drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-05-01 03:23:22.321060 vnfaker-0.0.2/src/vnfaker/data/company/
+-rw-r--r--   0 ducquang   (501) admin       (80)        0 2023-04-10 18:01:35.000000 vnfaker-0.0.2/src/vnfaker/data/company/__init__.py
+-rw-r--r--   0 ducquang   (501) admin       (80)     4748 2023-04-11 01:32:31.000000 vnfaker-0.0.2/src/vnfaker/data/company/company.name
+drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-05-01 03:23:22.322197 vnfaker-0.0.2/src/vnfaker/data/occupation/
+-rw-r--r--   0 ducquang   (501) admin       (80)        0 2023-04-10 18:01:35.000000 vnfaker-0.0.2/src/vnfaker/data/occupation/__init__.py
+-rw-r--r--   0 ducquang   (501) admin       (80)    34962 2023-04-11 06:57:16.000000 vnfaker-0.0.2/src/vnfaker/data/occupation/occupation.name
+drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-05-01 03:23:22.328016 vnfaker-0.0.2/src/vnfaker/data/person/
+-rw-r--r--   0 ducquang   (501) admin       (80)        0 2023-04-10 18:01:35.000000 vnfaker-0.0.2/src/vnfaker/data/person/__init__.py
+-rw-r--r--   0 ducquang   (501) admin       (80)     1136 2023-04-11 08:39:50.000000 vnfaker-0.0.2/src/vnfaker/data/person/female.name
+-rw-r--r--   0 ducquang   (501) admin       (80)     1089 2023-04-11 08:42:28.000000 vnfaker-0.0.2/src/vnfaker/data/person/female_middle.name
+-rw-r--r--   0 ducquang   (501) admin       (80)      111 2023-04-10 17:26:37.000000 vnfaker-0.0.2/src/vnfaker/data/person/first.name
+-rw-r--r--   0 ducquang   (501) admin       (80)      148 2023-04-11 08:43:12.000000 vnfaker-0.0.2/src/vnfaker/data/person/last.name
+-rw-r--r--   0 ducquang   (501) admin       (80)     1782 2023-04-25 12:45:47.000000 vnfaker-0.0.2/src/vnfaker/data/person/male.name
+-rw-r--r--   0 ducquang   (501) admin       (80)     1178 2023-04-11 08:38:25.000000 vnfaker-0.0.2/src/vnfaker/data/person/male_middle.name
+drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-05-01 03:23:22.335864 vnfaker-0.0.2/src/vnfaker/data/provinces/
+-rw-r--r--   0 ducquang   (501) admin       (80)        0 2023-04-10 18:01:35.000000 vnfaker-0.0.2/src/vnfaker/data/provinces/__init__.py
+-rw-r--r--   0 ducquang   (501) admin       (80)  3512185 2023-04-10 17:48:23.000000 vnfaker-0.0.2/src/vnfaker/data/provinces/flat-divisions.json
+-rw-r--r--   0 ducquang   (501) admin       (80)  2404923 2023-04-10 17:48:23.000000 vnfaker-0.0.2/src/vnfaker/data/provinces/nested-divisions.json
+drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-05-01 03:23:22.341188 vnfaker-0.0.2/src/vnfaker/data/sentence/
+-rw-r--r--   0 ducquang   (501) admin       (80)        0 2023-04-10 18:01:14.000000 vnfaker-0.0.2/src/vnfaker/data/sentence/__init__.py
+-rw-r--r--   0 ducquang   (501) admin       (80)   244103 2023-04-12 08:52:12.000000 vnfaker-0.0.2/src/vnfaker/data/sentence/sentence.txt
+-rw-r--r--   0 ducquang   (501) admin       (80)     9052 2023-05-01 03:22:48.000000 vnfaker-0.0.2/src/vnfaker/generator.py
+drwxr-xr-x   0 ducquang   (501) admin       (80)        0 2023-05-01 03:23:22.320002 vnfaker-0.0.2/src/vnfaker.egg-info/
+-rw-r--r--   0 ducquang   (501) admin       (80)     1812 2023-05-01 03:23:22.000000 vnfaker-0.0.2/src/vnfaker.egg-info/PKG-INFO
+-rw-r--r--   0 ducquang   (501) admin       (80)      939 2023-05-01 03:23:22.000000 vnfaker-0.0.2/src/vnfaker.egg-info/SOURCES.txt
+-rw-r--r--   0 ducquang   (501) admin       (80)        1 2023-05-01 03:23:22.000000 vnfaker-0.0.2/src/vnfaker.egg-info/dependency_links.txt
+-rw-r--r--   0 ducquang   (501) admin       (80)       15 2023-05-01 03:23:22.000000 vnfaker-0.0.2/src/vnfaker.egg-info/requires.txt
+-rw-r--r--   0 ducquang   (501) admin       (80)        8 2023-05-01 03:23:22.000000 vnfaker-0.0.2/src/vnfaker.egg-info/top_level.txt
```

### Comparing `vnfaker-0.0.1/LICENSE.txt` & `vnfaker-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vnfaker-0.0.1/PKG-INFO` & `vnfaker-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnfaker
-Version: 0.0.1
+Version: 0.0.2
 Summary: vnfaker is a Python package that generates fake data about fullname, address, phone, date_of_birth,... in Viet Nam.
 Home-page: https://github.com/phanducquang/vnfaker
 Author: Phan Duc Quang
 Author-email: phanducquang07@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/phanducquang/vnfaker/issues
 Platform: UNKNOWN
```

### Comparing `vnfaker-0.0.1/README.md` & `vnfaker-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `vnfaker-0.0.1/setup.py` & `vnfaker-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     README = fh.read()
 
 setuptools.setup(
     name="vnfaker",
-    version="0.0.1",
+    version="0.0.2",
     author="Phan Duc Quang",
     author_email="phanducquang07@gmail.com",
     description="vnfaker is a Python package that generates fake data about fullname, address, phone, date_of_birth,... in Viet Nam.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/phanducquang/vnfaker",
     project_urls={
```

### Comparing `vnfaker-0.0.1/src/vnfaker/commonUtils.py` & `vnfaker-0.0.2/src/vnfaker/commonUtils.py`

 * *Files identical despite different names*

### Comparing `vnfaker-0.0.1/src/vnfaker/data/company/company.name` & `vnfaker-0.0.2/src/vnfaker/data/company/company.name`

 * *Files identical despite different names*

### Comparing `vnfaker-0.0.1/src/vnfaker/data/occupation/occupation.name` & `vnfaker-0.0.2/src/vnfaker/data/occupation/occupation.name`

 * *Files identical despite different names*

### Comparing `vnfaker-0.0.1/src/vnfaker/data/person/female.name` & `vnfaker-0.0.2/src/vnfaker/data/person/female.name`

 * *Files identical despite different names*

### Comparing `vnfaker-0.0.1/src/vnfaker/data/person/female_middle.name` & `vnfaker-0.0.2/src/vnfaker/data/person/female_middle.name`

 * *Files identical despite different names*

### Comparing `vnfaker-0.0.1/src/vnfaker/data/person/male.name` & `vnfaker-0.0.2/src/vnfaker/data/person/male.name`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,284 +1,284 @@
-Cơ
-Khang
-Lai
-Nam
-Nguyên
-Ninh
-Tâm
-Thiện
-Tường
-Ðức
-Dũng
-Duy
-Hoàng
-Khải
-Khoa
-Khôi
-Minh
-Quân
-Quốc
-Sơn
-Tài
-Thái
-Tú
-Tuấn
-Tùng
-Việt
-Vũ
-Cường
-Kỳ
-Lộc
-Long
-Phước
-Thành
-Thịnh
-Thúc
-Trúc
-Du
-Nhân
 An
+Án
+Ân
+Ẩn
+Anh
+Bắc
+Bạch
+Bằng
+Bào
 Bảo
+Bảo Long
+Bình
+Bổng
+Bửu
+Ca
+Cần
+Cẩn
+Canh
+Cảnh
+Cao
 Chấn
+Châu
+Chiến
+Chiểu
+Chinh
+Chính
+Chương
+Chưởng
+Chuyên
+Cơ
+Công
+Cung
+Cương
+Cường
+Ðại
+Dân
+Ðan
+Ðăng
+Danh
+Ðạo
+Ðạt
+Ðệ
+Di
+Ðiền
+Diệp
+Ðiệp
+Diệu
+Dinh
+Ðình
 Ðịnh
+Ðộ
+Ðoàn
+Doanh
+Ðôn
+Ðông
+Ðồng
+Du
+Đức
+Ðức
+Duệ
+Dũng
+Dụng
+Dương
+Duy
+Duyệt
+Gia
+Giác
 Giang
+Giáp
+Hà
+Hải
+Hải An
+Hàm
+Hãn
+Hành
+Hạnh
+Hào
+Hảo
+Hậu
+Hiên
+Hiền
 Hiển
+Hiệp
+Hiếu
 Hoa
+Hòa
+Hoài
+Hoán
+Hoàn
+Hoàng
+Hoạt
+Học
+Hội
+Hồng
+Hợp
+Huấn
+Hùng
+Hưng
+Hữu
 Huy
 Huynh
 Huỳnh
+Hỷ
+Kha
+Khải
+Khang
+Khanh
 Khánh
-Lâm
-Pháp
-Thạch
-Tín
-Toàn
-Nhã
-Dân
-Ðạt
-Dương
-Hòa
-Thuận
-Yên
-Chưởng
-Diệp
-Toại
-Nghiệp
-Phong
-Sĩ
-Sỹ
-Thọ
-Tiến
-Uy
-Hùng
-Hưng
-Phương
-Anh
-Công
-Hiếu
 Khiêm
+Khiếu
+Khoa
+Khoan
+Khoát
+Khôi
+Khương
+Kiếm
 Kiên
-Thanh
-Thắng
-Trực
-Thủy
-Án
-Ân
-Bằng
-Hải
-Hào
-Hậu
-Hoán
+Kiện
+Kiệt
+Kim
+Kính
+Kỳ
+Kỷ
+Lạc
+Lai
+Lam
+Lâm
+Lân
 Lập
+Lễ
+Liêm
+Liên
+Liệt
+Linh
+Lĩnh
+Lộ
+Lộc
+Lợi
+Long
+Luân
 Luận
 Luật
+Lực
+Lương
 Lý
-Phụng
-Sinh
-Tráng
+Mẫn
+Mạnh
+Miên
+Minh
+Mỹ
+Nam
+Năng
+Ngân
+Ngạn
 Nghị
-Quyết
-Di
-Lộ
-Lực
-Trọng
-Hành
+Nghĩa
+Nghiêm
+Nghiệp
 Ngọc
-Thống
-Hiệp
-Quế
-Khương
-Quang
-Văn
-Chiểu
-Chương
-Diệu
-Ðôn
-Hảo
-Hợp
-Kim
-Ngân
+Ngôn
+Nguyên
+Nhã
+Nhân
+Nhạn
+Nhất
+Nhật
+Nhiệm
+Nhiên
+Nhu
+Nhuận
+Nhượng
+Ninh
+Pháp
+Phát
+Phi
+Phong
+Phu
 Phú
 Phúc
+Phụng
+Phước
+Phương
+Quân
+Quang
 Quảng
+Quế
+Quốc
+Quý
+Quyền
+Quyết
+Quỳnh
+Sa
+Sâm
+San
 Sang
+Sáng
+Sĩ
 Siêu
-Trung
-Tụ
-Bình
-Chính
-Hạnh
-Mạnh
-Phi
-Quyền
-Toản
-Trí
-Tuệ
-Cẩn
-Hiền
-Kính
-Ngôn
-Nhượng
+Sinh
+Sơn
+Sử
+Sỹ
+Tài
+Tâm
 Tân
-Thông
-Tiếp
-Tuyền
-Bạch
-Cần
-Cảnh
-Ðạo
-Huấn
-Kiệt
-Vinh
-Lam
+Tấn
+Thạc
+Thạch
+Thái
+Thắng
+Thanh
+Thành
+Thế
+Thể
 Thiên
-Ðăng
-Hà
+Thiện
+Thịnh
+Thọ
+Thời
+Thông
+Thống
+Thuận
+Thuật
+Thúc
+Thực
+Thương
+Thủy
 Thụy
-Nhiên
-Dinh
-Dụng
-Học
-Liêm
-Nghĩa
-Bắc
-Lạc
-Vỹ
-Kiếm
-Duệ
-Linh
-Mỹ
-Phát
-Xuân
-Đức
-Lân
-Lĩnh
-Nhật
-Nhuận
-Quý
-Võ
+Thuyết
+Tiến
 Tiền
-Bào
-Canh
-Châu
-Chiến
-Cương
-Khanh
-Khoát
-Lương
-Thực
+Tiển
+Tiếp
+Tín
+Tính
+Tịnh
+Tổ
+Toại
+Toàn
+Toản
 Trác
-Từ
-Vĩnh
-Vượng
-Kha
+Trạch
 Trân
-Kỷ
+Trang
+Tráng
+Trí
+Triết
+Triều
 Triệu
-Ca
-Kiện
-Ðan
-Hoàn
-Hội
+Trình
+Trọng
+Trụ
+Trúc
+Trực
+Trung
+Trương
+Trường
 Trưởng
+Tú
+Từ
+Tụ
+Tuấn
+Tuệ
+Tùng
+Tường
+Tuyền
+Tuyển
+Uy
+Văn
 Vĩ
-Ðồng
-Trường
 Viên
+Việt
+Vinh
+Vĩnh
 Vịnh
-Ðình
-Nghiêm
-Quỳnh
-Tấn
-Trình
-Danh
-Hiên
-Hỷ
-Khiếu
-Mẫn
-Nhu
-Thạc
-Triết
+Võ
 Vu
+Vũ
 Vương
-Giác
-Ẩn
-Ðoàn
-Ngạn
-Tiển
-Trụ
-Bổng
-Giáp
-Hải An
-Sử
-Sâm
-Bảo Long
-Hồng
-Ðiệp
-Nhạn
-Ðộ
-Thời
-Ðiền
-Lễ
-Thể
-Trạch
-Triều
-Bửu
-Ðại
-Hữu
-Sáng
-Hoài
-Trang
-Lợi
-Trương
-San
-Tổ
-Ðệ
-Doanh
-Thế
-Tịnh
+Vượng
+Vỹ
+Xuân
 Ý
-Duyệt
-Năng
-Luân
-Tính
-Nhiệm
-Nhất
-Liệt
-Thuật
-Miên
-Hoạt
-Liên
-Chuyên
-Chinh
-Phu
-Sa
-Ðông
-Khoan
-Tuyển
-Thương
-Gia
-Cao
-Cung
-Hàm
-Hãn
-Thuyết
+Yên
```

### Comparing `vnfaker-0.0.1/src/vnfaker/data/person/male_middle.name` & `vnfaker-0.0.2/src/vnfaker/data/person/male_middle.name`

 * *Files identical despite different names*

### Comparing `vnfaker-0.0.1/src/vnfaker/data/provinces/flat-divisions.json` & `vnfaker-0.0.2/src/vnfaker/data/provinces/flat-divisions.json`

 * *Files identical despite different names*

### Comparing `vnfaker-0.0.1/src/vnfaker/data/provinces/nested-divisions.json` & `vnfaker-0.0.2/src/vnfaker/data/provinces/nested-divisions.json`

 * *Files identical despite different names*

### Comparing `vnfaker-0.0.1/src/vnfaker/data/sentence/sentence.txt` & `vnfaker-0.0.2/src/vnfaker/data/sentence/sentence.txt`

 * *Files identical despite different names*

### Comparing `vnfaker-0.0.1/src/vnfaker/generator.py` & `vnfaker-0.0.2/src/vnfaker/generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 from .commonUtils import CommonUtils, str_clean, change_year, date_time_ad
 
 
 class Generator:
 
     def __init__(self):
+        self.username_value = None
         self.email_value = None
         self.district_name = None
         self.ward_name = None
         self.province_name = None
         self.known_location_value = None
         self.name_value = None
         self.last_name_value = None
```

### Comparing `vnfaker-0.0.1/src/vnfaker.egg-info/PKG-INFO` & `vnfaker-0.0.2/src/vnfaker.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnfaker
-Version: 0.0.1
+Version: 0.0.2
 Summary: vnfaker is a Python package that generates fake data about fullname, address, phone, date_of_birth,... in Viet Nam.
 Home-page: https://github.com/phanducquang/vnfaker
 Author: Phan Duc Quang
 Author-email: phanducquang07@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/phanducquang/vnfaker/issues
 Platform: UNKNOWN
```

### Comparing `vnfaker-0.0.1/src/vnfaker.egg-info/SOURCES.txt` & `vnfaker-0.0.2/src/vnfaker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

