# Comparing `tmp/satdigitalinvoice-4.0.6.tar.gz` & `tmp/satdigitalinvoice-4.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satdigitalinvoice-4.0.6.tar", last modified: Wed Apr 26 06:52:39 2023, max compression
+gzip compressed data, was "satdigitalinvoice-4.0.7.tar", last modified: Mon May  1 16:21:40 2023, max compression
```

## Comparing `satdigitalinvoice-4.0.6.tar` & `satdigitalinvoice-4.0.7.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:52:39.731170 satdigitalinvoice-4.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-26 06:52:39.731170 satdigitalinvoice-4.0.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:52:39.727170 satdigitalinvoice-4.0.6/satdigitalinvoice/
--rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-04-26 06:52:19.000000 satdigitalinvoice-4.0.6/satdigitalinvoice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-26 06:52:19.000000 satdigitalinvoice-4.0.6/satdigitalinvoice/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-04-26 06:52:19.000000 satdigitalinvoice-4.0.6/satdigitalinvoice/client_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-04-26 06:52:19.000000 satdigitalinvoice-4.0.6/satdigitalinvoice/environments.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-26 06:52:19.000000 satdigitalinvoice-4.0.6/satdigitalinvoice/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    38644 2023-04-26 06:52:19.000000 satdigitalinvoice-4.0.6/satdigitalinvoice/facturacion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-04-26 06:52:19.000000 satdigitalinvoice-4.0.6/satdigitalinvoice/file_data_managers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:52:39.727170 satdigitalinvoice-4.0.6/satdigitalinvoice/formatting_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 06:52:19.000000 satdigitalinvoice-4.0.6/satdigitalinvoice/formatting_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-26 06:52:19.000000 satdigitalinvoice-4.0.6/satdigitalinvoice/formatting_functions/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    13105 2023-04-26 06:52:19.000000 satdigitalinvoice-4.0.6/satdigitalinvoice/gui_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:52:39.727170 satdigitalinvoice-4.0.6/satdigitalinvoice/images/
--rw-r--r--   0 runner    (1001) docker     (123)    71867 2023-04-26 06:52:19.000000 satdigitalinvoice-4.0.6/satdigitalinvoice/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    30053 2023-04-26 06:52:19.000000 satdigitalinvoice-4.0.6/satdigitalinvoice/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     6555 2023-04-26 06:52:19.000000 satdigitalinvoice-4.0.6/satdigitalinvoice/localdb.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-26 06:52:19.000000 satdigitalinvoice-4.0.6/satdigitalinvoice/log_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:52:39.727170 satdigitalinvoice-4.0.6/satdigitalinvoice/markdown_styles/
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-26 06:52:19.000000 satdigitalinvoice-4.0.6/satdigitalinvoice/markdown_styles/markdown6.css
--rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-04-26 06:52:19.000000 satdigitalinvoice-4.0.6/satdigitalinvoice/mycfdi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:52:39.727170 satdigitalinvoice-4.0.6/satdigitalinvoice/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-26 06:52:19.000000 satdigitalinvoice-4.0.6/satdigitalinvoice/schemas/cliente.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-26 06:52:19.000000 satdigitalinvoice-4.0.6/satdigitalinvoice/schemas/factura.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-04-26 06:52:19.000000 satdigitalinvoice-4.0.6/satdigitalinvoice/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:52:39.727170 satdigitalinvoice-4.0.6/satdigitalinvoice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-26 06:52:39.000000 satdigitalinvoice-4.0.6/satdigitalinvoice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-26 06:52:39.000000 satdigitalinvoice-4.0.6/satdigitalinvoice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 06:52:39.000000 satdigitalinvoice-4.0.6/satdigitalinvoice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-26 06:52:39.000000 satdigitalinvoice-4.0.6/satdigitalinvoice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-26 06:52:39.000000 satdigitalinvoice-4.0.6/satdigitalinvoice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 06:52:39.731170 satdigitalinvoice-4.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-04-26 06:52:19.000000 satdigitalinvoice-4.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:52:39.731170 satdigitalinvoice-4.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-26 06:52:19.000000 satdigitalinvoice-4.0.6/tests/test_clients.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-26 06:52:19.000000 satdigitalinvoice-4.0.6/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-04-26 06:52:19.000000 satdigitalinvoice-4.0.6/tests/test_crear_facturas.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-26 06:52:19.000000 satdigitalinvoice-4.0.6/tests/test_localdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-04-26 06:52:19.000000 satdigitalinvoice-4.0.6/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:21:40.786599 satdigitalinvoice-4.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-05-01 16:21:40.786599 satdigitalinvoice-4.0.7/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:21:40.786599 satdigitalinvoice-4.0.7/satdigitalinvoice/
+-rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-05-01 16:21:29.000000 satdigitalinvoice-4.0.7/satdigitalinvoice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-01 16:21:29.000000 satdigitalinvoice-4.0.7/satdigitalinvoice/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-05-01 16:21:29.000000 satdigitalinvoice-4.0.7/satdigitalinvoice/client_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-05-01 16:21:29.000000 satdigitalinvoice-4.0.7/satdigitalinvoice/environments.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-01 16:21:29.000000 satdigitalinvoice-4.0.7/satdigitalinvoice/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39432 2023-05-01 16:21:29.000000 satdigitalinvoice-4.0.7/satdigitalinvoice/facturacion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-05-01 16:21:29.000000 satdigitalinvoice-4.0.7/satdigitalinvoice/file_data_managers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:21:40.786599 satdigitalinvoice-4.0.7/satdigitalinvoice/formatting_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 16:21:29.000000 satdigitalinvoice-4.0.7/satdigitalinvoice/formatting_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-01 16:21:29.000000 satdigitalinvoice-4.0.7/satdigitalinvoice/formatting_functions/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13105 2023-05-01 16:21:29.000000 satdigitalinvoice-4.0.7/satdigitalinvoice/gui_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:21:40.786599 satdigitalinvoice-4.0.7/satdigitalinvoice/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    71867 2023-05-01 16:21:29.000000 satdigitalinvoice-4.0.7/satdigitalinvoice/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    30053 2023-05-01 16:21:29.000000 satdigitalinvoice-4.0.7/satdigitalinvoice/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-05-01 16:21:29.000000 satdigitalinvoice-4.0.7/satdigitalinvoice/localdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-01 16:21:29.000000 satdigitalinvoice-4.0.7/satdigitalinvoice/log_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:21:40.786599 satdigitalinvoice-4.0.7/satdigitalinvoice/markdown_styles/
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-05-01 16:21:29.000000 satdigitalinvoice-4.0.7/satdigitalinvoice/markdown_styles/markdown6.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-05-01 16:21:29.000000 satdigitalinvoice-4.0.7/satdigitalinvoice/mycfdi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:21:40.786599 satdigitalinvoice-4.0.7/satdigitalinvoice/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-01 16:21:29.000000 satdigitalinvoice-4.0.7/satdigitalinvoice/schemas/cliente.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-01 16:21:29.000000 satdigitalinvoice-4.0.7/satdigitalinvoice/schemas/factura.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-05-01 16:21:29.000000 satdigitalinvoice-4.0.7/satdigitalinvoice/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:21:40.786599 satdigitalinvoice-4.0.7/satdigitalinvoice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-05-01 16:21:40.000000 satdigitalinvoice-4.0.7/satdigitalinvoice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-01 16:21:40.000000 satdigitalinvoice-4.0.7/satdigitalinvoice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 16:21:40.000000 satdigitalinvoice-4.0.7/satdigitalinvoice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-01 16:21:40.000000 satdigitalinvoice-4.0.7/satdigitalinvoice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-01 16:21:40.000000 satdigitalinvoice-4.0.7/satdigitalinvoice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 16:21:40.786599 satdigitalinvoice-4.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-05-01 16:21:29.000000 satdigitalinvoice-4.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:21:40.786599 satdigitalinvoice-4.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-01 16:21:29.000000 satdigitalinvoice-4.0.7/tests/test_clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-01 16:21:29.000000 satdigitalinvoice-4.0.7/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-05-01 16:21:29.000000 satdigitalinvoice-4.0.7/tests/test_crear_facturas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-01 16:21:29.000000 satdigitalinvoice-4.0.7/tests/test_localdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-05-01 16:21:29.000000 satdigitalinvoice-4.0.7/tests/test_main.py
```

### Comparing `satdigitalinvoice-4.0.6/PKG-INFO` & `satdigitalinvoice-4.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satdigitalinvoice
-Version: 4.0.6
+Version: 4.0.7
 Summary: GUI APP to Generate CFDI
 Home-page: https://github.com/SAT-CFDI/python-satdigitalinvoice
 Author: satcfdi@outlook.com
 Author-email: satcfdi@outlook.com
 License: MIT License
 Project-URL: Documentation, https://satdigitalinvoice.readthedocs.io
 Project-URL: Source, https://github.com/SAT-CFDI/python-satdigitalinvoice
```

### Comparing `satdigitalinvoice-4.0.6/satdigitalinvoice/__init__.py` & `satdigitalinvoice-4.0.7/satdigitalinvoice/__init__.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.6/satdigitalinvoice/__version__.py` & `satdigitalinvoice-4.0.7/satdigitalinvoice/__version__.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.6/satdigitalinvoice/client_validation.py` & `satdigitalinvoice-4.0.7/satdigitalinvoice/client_validation.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.6/satdigitalinvoice/environments.py` & `satdigitalinvoice-4.0.7/satdigitalinvoice/environments.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.6/satdigitalinvoice/facturacion.py` & `satdigitalinvoice-4.0.7/satdigitalinvoice/facturacion.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,16 @@
     layout = [[sg.Text("New Window", key="new")]]
     window = sg.Window("Launch Window", layout, modal=True, size=(300, 300))
     window.read(timeout=1000)
 
     return window
 
 
+
+
 class FacturacionGUI:
     def __init__(self, config):
         os.makedirs(TEMP_DIRECTORY, exist_ok=True)
         self.email_manager = EmailManager(
             **config['email']
         )
         pac = config['pac']
@@ -152,23 +154,25 @@
 
         cfdi40.Comprobante.sign(invoice, self.csd_signer)
 
         attempts = 3
         for i in range(attempts):
             if i:
                 print(f'Intentando de nuevo... Intento {i + 1} de {attempts}')
-                self._read(timeout=2000 * i)
+                if not self._read(timeout=2000 * i):
+                    return
 
             try:
                 res = self.pac_service.stamp(
                     cfdi=invoice,
                     accept=Accept.XML_PDF,
                     ref_id=ref_id
                 )
             except Exception as ex:
+                self.show_console()
                 message = f"Error al generar factura: {invoice.get('Serie')}{invoice.get('Folio')} {invoice['Receptor']['Rfc']}"
                 logger.exception(message)
                 print(message)
                 if isinstance(ex, ResponseError):
                     logger.error(f"Status Code: {ex.response.status_code}")
                     print(f"Status Code: {ex.response.status_code}")
                     logger.error(f"Response: {ex.response.text}")
@@ -237,15 +241,15 @@
                 if paquete:
                     data = base64.b64decode(paquete)
                     with io.BytesIO(data) as b:
                         self.unzip_cfdi(b)
 
     def unzip_cfdi(self, file):
         with ZipFile(file, "r") as zf:
-            for fileinfo in zf.infolist():
+            for fileinfo in self.progress_iterate(zf.infolist(), 'Descomprimiendo'):
                 data = zf.read(fileinfo)
                 match os.path.splitext(fileinfo.filename)[1]:
                     case ".xml":
                         self.all_invoices = None
                         MyCFDI.move_to_folder(data, pdf_data=None)
                     case ".pdf":
                         pass
@@ -260,114 +264,117 @@
                             row = dict(zip(header, row))
                             print_yaml(row)
                             self.local_db.status_merge(
                                 uuid=row['Uuid'],
                                 estatus=row['Estatus'],
                                 fecha_cancelacion=row['FechaCancelacion']
                             )
-                self._read()
 
     def _read(self, timeout=0):
         event, values = self.window.read(timeout=timeout)
         if event in ("Exit", sg.WIN_CLOSED):
-            exit(0)
+            return False
+        return True
 
-    def action_button(self, action_name, action_items):
+    def progress_iterate(self, items, title, fn=None):
+        ln = None
+        if hasattr(items, '__len__'):
+            ln = len(items)
+
+        for i, item in enumerate(items):
+            if not sg.one_line_progress_meter(
+                    'Progress Meter',
+                    i,
+                    ln or (i + 1),
+                    title,
+                    fn(item) if callable(fn) else "",
+                    keep_on_top=True,
+                    no_titlebar=True,
+                    grab_anywhere=True,
+            ):
+                return
+            yield item
+            if not self._read():
+                return
+        sg.one_line_progress_meter_cancel()
+
+    def action_button(self, action_name, action_items, action_text):
         match action_name:
             case 'solicitudes':
-                for solicitud in action_items:
+                self.show_console()
+                for solicitud in self.progress_iterate(action_items, action_text):
                     id_solicitud = solicitud["response"]["IdSolicitud"]
                     response = self.sat_service.recover_comprobante_status(
                         id_solicitud=id_solicitud
                     )
                     print_yaml(response)
                     self.local_db.solicitud_merge(id_solicitud, response=response)
                     self.recupera_comprobantes(response)
-                    self._read()
 
             case 'facturas' | 'pago':
-                for invoice in action_items:
+                for invoice in self.progress_iterate(action_items, action_text):
                     cfdi = self.generate_invoice(invoice=invoice)
                     if cfdi is None:
                         break
-                    print_yaml({
-                        "FacturaGenerada": cfdi_header(cfdi),
-                    })
-                    self._read()
 
             case 'correos':
                 clients = ClientsManager()
                 emisor = clients[self.csd_signer.rfc]
                 with self.email_manager.sender as s:
-                    for receptor, facturas, facturas_facturas_pendientes_meses_anteriores in action_items:
-
+                    for receptor, facturas, facturas_facturas_pendientes_meses_anteriores in self.progress_iterate(action_items, action_text):
                         def attachments():
                             for ni in facturas:
                                 yield ni.filename + ".xml"
                                 yield ni.filename + ".pdf"
 
-                        subject = f"Comprobantes Fiscales {receptor['RazonSocial']} - {receptor['Rfc']}"
-
                         s.send_email(
-                            subject=subject,
+                            subject=f"Comprobantes Fiscales {receptor['RazonSocial']} - {receptor['Rfc']}",
                             to_addrs=receptor["Email"],
                             html=facturacion_environment.get_template('mail_facturas_template.html').render(
                                 facturas=facturas,
                                 facturas_pendientes_meses_anteriores=facturas_facturas_pendientes_meses_anteriores,
                                 emisor=emisor,
                                 receptor=receptor,
                             ),
                             file_attachments=attachments()
                         )
                         for r in facturas:
                             self.local_db.notified_set(r.uuid, True)
-                        print_yaml({
-                            "correo": subject,
-                            "para": receptor["Email"]
-                        })
-                        self._read()
 
             case 'ajustes':
                 clients = ClientsManager()
                 emisor = clients[self.csd_signer.rfc]
                 with self.email_manager.sender as s:
-                    for data in action_items:
-                        receptor = data['receptor']
-                        file_name = data['file_name']
-                        subject = f"Ajuste Renta {receptor['RazonSocial']} - {receptor['Rfc']}"
-
+                    for data in self.progress_iterate(action_items, action_text):
                         if not data['ajuste_porcentaje']:
-                            print(f"NO HAY {subject}")
                             continue
 
+                        receptor = data['receptor']
+                        file_name = data['file_name']
+
                         s.send_email(
-                            subject=subject,
+                            subject=f"Ajuste Renta {receptor['RazonSocial']} - {receptor['Rfc']}",
                             to_addrs=receptor["Email"],
                             html=facturacion_environment.get_template('mail_ajustes_template.html').render(
                                 emisor=emisor,
                                 receptor=receptor,
                             ),
                             file_attachments=[file_name]
                         )
-                        print_yaml({
-                            "correo": subject,
-                            "para": receptor["Email"]
-                        })
-                        self._read()
 
             case 'clientes':
-                for client in action_items:
-                    print(f"Validando: {client['Rfc']}")
+                for client in self.progress_iterate(
+                        action_items, action_text, lambda x: f"Validando: {x['Rfc']}"
+                ):
                     validar_client(client)
-                    self._read()
 
             case _:
                 raise ValueError(f"Invalid action: {action_name}")
 
-        print("FIN")
+        sg.one_line_progress_meter_cancel()
 
     def set_selected_satcfdis(self, cfdis: list):
         i = cfdis[0] if len(cfdis) == 1 else None
 
         if i:
             estatus = EstadoComprobante(i.estatus)
             self.window["status_sat"].update(
@@ -438,19 +445,23 @@
         self.window["ppd_action_items"].update(visible=is_ppd_active)
         self.window["importe_pago"].update(i.saldo_pendiente if is_ppd_active else '')
         if is_ppd_active:
             self.action_button_manager.set_items("pago", [i])
         else:
             self.action_button_manager.clear()
 
-    def header(self, name):
-        self.window['console_tab'].select()
+    def header(self, name, select_console=True):
+        if select_console:
+            self.show_console()
         self.console.update(header_line(name))
         self._read()
 
+    def show_console(self):
+        self.window['errores_tab'].select()
+
     def download_invoice(self, uuid: UUID):
         res = self.pac_service.recover(uuid, accept=Accept.XML_PDF)
         self.all_invoices = None
         return MyCFDI.move_to_folder(res.xml, pdf_data=res.pdf)
 
     def facturas_search(self):
         search_text = self.window["emitidas_search"].get()
@@ -524,14 +535,25 @@
             background_color="red4",
             location=center_location(self.window),
             button_type=POPUP_BUTTONS_NO_BUTTONS,
             auto_close=True,
             non_blocking=True,
         )
 
+    def done_message(self, ex):
+        sg.Popup(
+            ex,
+            no_titlebar=True,
+            background_color="green4",
+            location=center_location(self.window),
+            button_type=POPUP_BUTTONS_NO_BUTTONS,
+            auto_close=True,
+            non_blocking=True,
+        )
+
     def nuevas_facturas(self, values, force=False):
         facturas_table = self.window['facturas_table']
         has_value = bool(facturas_table.metadata)
         facturas_table.update(values=[])
         self.window['preparar_facturas_text'].update("")
 
         if has_value or force:
@@ -792,20 +814,22 @@
                                 f"Estas seguro que quieres '{action_text}'?",
                                 title="Confirmar",
                                 button_type=POPUP_BUTTONS_OK_CANCEL,
                                 location=center_location(self.window),
                                 keep_on_top=True,
                             )
                             if res == "OK":
-                                self.header(action_text.upper())
+                                self.header(action_text.upper(), select_console=False)
                                 self.action_button_manager.clear()
                                 self.action_button(
                                     action_name=action_name,
-                                    action_items=action_items
+                                    action_items=action_items,
+                                    action_text=action_text
                                 )
+                                self.main_tab_group(values)
 
                     case "editar_clientes":
                         open_file(
                             os.path.abspath("clientes.yaml")
                         )
 
                     case "exportar_clientes":
@@ -862,43 +886,42 @@
                         if zip_file:
                             self.header("Cargar ZIP")
                             self.unzip_cfdi(zip_file)
 
                     case 'importar_emitidas':
                         csv_file = sg.popup_get_file('', multiple_files=False, no_window=True, file_types=(("CSV Files", "*.csv"),))
                         if csv_file:
-                            self.header("Importar emitidas")
                             all_invoices = self.get_all_invoices()
                             with open(csv_file, newline='', encoding='utf-8') as f:
                                 reader = csv.reader(f)
                                 header = next(reader)
                                 for row in reader:
                                     row = dict(zip(header, row))
                                     uuid = UUID(row["Folio Fiscal (UUID)"])
                                     if uuid not in all_invoices:
                                         cfdi = self.download_invoice(uuid)
 
                                         if row.get("Estatus", "Entregado SAT") != "Entregado SAT":
-                                            estado = self.local_db.status_sat(cfdi, update=True)
-                                            print_yaml(estado)
-                                    self._read()
-                                print("FIN")
+                                            self.local_db.status_sat(cfdi, update=True)
+                            self.done_message("FIN")
 
                     case "exportar_metadata":
                         with open(METADATA_FILE, 'w', newline='', encoding='utf-8') as f:
                             writer = csv.writer(f)
                             for i in self.get_all_invoices():
                                 if status := self.local_db.status_export(i):
                                     writer.writerow(status)
+                        self.done_message("FIN")
 
                     case "importar_metadata":
                         with open(METADATA_FILE, newline='', encoding='utf-8') as f:
                             reader = csv.reader(f)
                             for row in reader:
                                 self.local_db.status_merge(*row)
+                        self.done_message("FIN")
 
                     case _:
                         logger.error(f"Unknown event '{event}'")
 
             except (ValueError, XlsxFileError) as ex:
                 self.error_message(ex)
             except ConsoleErrors as ex:
```

### Comparing `satdigitalinvoice-4.0.6/satdigitalinvoice/file_data_managers.py` & `satdigitalinvoice-4.0.7/satdigitalinvoice/file_data_managers.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.6/satdigitalinvoice/formatting_functions/common.py` & `satdigitalinvoice-4.0.7/satdigitalinvoice/formatting_functions/common.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.6/satdigitalinvoice/gui_functions.py` & `satdigitalinvoice-4.0.7/satdigitalinvoice/gui_functions.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.6/satdigitalinvoice/images/logo.png` & `satdigitalinvoice-4.0.7/satdigitalinvoice/images/logo.png`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.6/satdigitalinvoice/layout.py` & `satdigitalinvoice-4.0.7/satdigitalinvoice/layout.py`

 * *Files 0% similar despite different names*

```diff
@@ -430,30 +430,30 @@
                                 sg.Button(image_data=EXCEL_ICON, key="ver_excel", border_width=0, button_color=BUTTON_COLOR),
                                 sg.Button(image_data=FOLDER_ICON, key="ver_carpeta", border_width=0, button_color=BUTTON_COLOR),
                             ]])
                         ]],
                         key='contabilidad_tab',
                     ),
                     sg.Tab(
-                        'Consola'.center(13),
+                        'Errores'.center(13),
                         [
                             [
                                 sg.Push(),
                                 sg.Button(image_data=ABOUT_ICON, key="about", border_width=0, button_color=BUTTON_COLOR),
                             ],
                             [sg.Multiline(
                                 expand_x=True,
                                 expand_y=True,
                                 key="console",
                                 write_only=True,
                                 autoscroll=True,
                                 reroute_stdout=True
                             )]
                         ],
-                        key='console_tab',
+                        key='errores_tab',
                     ),
                     sg.Tab(
                         'Configuracion'.center(13),
                         [
                             [
                                 sg.Column([[
                                     sg.Button(image_data=EDIT_ICON, key="editar_configurar", border_width=0, button_color=BUTTON_COLOR),
```

### Comparing `satdigitalinvoice-4.0.6/satdigitalinvoice/localdb.py` & `satdigitalinvoice-4.0.7/satdigitalinvoice/localdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -185,15 +185,15 @@
 
     def status_sat(self, cfdi: SatCFDI, update=False):
         if update:
             res = sat_manager.status(cfdi)
             if res["ValidacionEFOS"] == "200":
                 self.status_merge(
                     uuid=cfdi.uuid,
-                    estatus=estado_to_estatus(res["Estatus"]),
+                    estatus=estado_to_estatus(res["Estado"]),
                     es_cancelable=res["EsCancelable"],
                     estatus_cancelacion=res["EstatusCancelacion"]
                 )
             else:
                 raise ValueError("Error al actualizar estado de %s: %s", cfdi.uuid, res)
             return res
         else:
```

### Comparing `satdigitalinvoice-4.0.6/satdigitalinvoice/log_tools.py` & `satdigitalinvoice-4.0.7/satdigitalinvoice/log_tools.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.6/satdigitalinvoice/markdown_styles/markdown6.css` & `satdigitalinvoice-4.0.7/satdigitalinvoice/markdown_styles/markdown6.css`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.6/satdigitalinvoice/mycfdi.py` & `satdigitalinvoice-4.0.7/satdigitalinvoice/mycfdi.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.6/satdigitalinvoice/schemas/factura.yaml` & `satdigitalinvoice-4.0.7/satdigitalinvoice/schemas/factura.yaml`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.6/satdigitalinvoice/utils.py` & `satdigitalinvoice-4.0.7/satdigitalinvoice/utils.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.6/satdigitalinvoice.egg-info/PKG-INFO` & `satdigitalinvoice-4.0.7/satdigitalinvoice.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satdigitalinvoice
-Version: 4.0.6
+Version: 4.0.7
 Summary: GUI APP to Generate CFDI
 Home-page: https://github.com/SAT-CFDI/python-satdigitalinvoice
 Author: satcfdi@outlook.com
 Author-email: satcfdi@outlook.com
 License: MIT License
 Project-URL: Documentation, https://satdigitalinvoice.readthedocs.io
 Project-URL: Source, https://github.com/SAT-CFDI/python-satdigitalinvoice
```

### Comparing `satdigitalinvoice-4.0.6/satdigitalinvoice.egg-info/SOURCES.txt` & `satdigitalinvoice-4.0.7/satdigitalinvoice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.6/setup.py` & `satdigitalinvoice-4.0.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         package: [
             "markdown_styles/*",
             "schemas/*",
             'images/*',
         ],
     },
     install_requires=[
-        'satcfdi==4.0.18',
+        'satcfdi==4.0.19',
         'diskcache',
         'num2words',
         'PyYAML',
         'babel',
         'markdown2',
         'PySimpleGUI',
         'XlsxWriter',
```

### Comparing `satdigitalinvoice-4.0.6/tests/test_crear_facturas.py` & `satdigitalinvoice-4.0.7/tests/test_crear_facturas.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.6/tests/test_localdb.py` & `satdigitalinvoice-4.0.7/tests/test_localdb.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-4.0.6/tests/test_main.py` & `satdigitalinvoice-4.0.7/tests/test_main.py`

 * *Files identical despite different names*

