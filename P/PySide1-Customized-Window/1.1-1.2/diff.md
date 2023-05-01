# Comparing `tmp/PySide1_Customized_Window-1.1-py3-none-any.whl.zip` & `tmp/PySide1_Customized_Window-1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 9524 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat    40952 b- defN 23-Apr-30 06:46 PySide1_Customized_Window.py
--rw-rw-rw-  2.0 fat       10 b- defN 23-Apr-30 08:25 PySide1_Customized_Window-1.1.dist-info/DESCRIPTION.rst
--rw-rw-rw-  2.0 fat      619 b- defN 23-Apr-30 08:25 PySide1_Customized_Window-1.1.dist-info/metadata.json
--rw-rw-rw-  2.0 fat        1 b- defN 23-Apr-30 08:25 PySide1_Customized_Window-1.1.dist-info/top_level.txt
--rw-rw-rw-  2.0 fat       97 b- defN 23-Apr-30 08:25 PySide1_Customized_Window-1.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat      486 b- defN 23-Apr-30 08:25 PySide1_Customized_Window-1.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat      672 b- defN 23-Apr-30 08:25 PySide1_Customized_Window-1.1.dist-info/RECORD
-7 files, 42837 bytes uncompressed, 8314 bytes compressed:  80.6%
+Zip file size: 10240 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat    44960 b- defN 23-May-01 13:19 PySide1_Customized_Window.py
+-rw-rw-rw-  2.0 fat       10 b- defN 23-May-01 13:46 PySide1_Customized_Window-1.2.dist-info/DESCRIPTION.rst
+-rw-rw-rw-  2.0 fat      619 b- defN 23-May-01 13:46 PySide1_Customized_Window-1.2.dist-info/metadata.json
+-rw-rw-rw-  2.0 fat        1 b- defN 23-May-01 13:46 PySide1_Customized_Window-1.2.dist-info/top_level.txt
+-rw-rw-rw-  2.0 fat       97 b- defN 23-May-01 13:46 PySide1_Customized_Window-1.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat      486 b- defN 23-May-01 13:46 PySide1_Customized_Window-1.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      672 b- defN 23-May-01 13:46 PySide1_Customized_Window-1.2.dist-info/RECORD
+7 files, 46845 bytes uncompressed, 9030 bytes compressed:  80.7%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: PySide1_Customized_Window.py
 Comment: 
 
-Filename: PySide1_Customized_Window-1.1.dist-info/DESCRIPTION.rst
+Filename: PySide1_Customized_Window-1.2.dist-info/DESCRIPTION.rst
 Comment: 
 
-Filename: PySide1_Customized_Window-1.1.dist-info/metadata.json
+Filename: PySide1_Customized_Window-1.2.dist-info/metadata.json
 Comment: 
 
-Filename: PySide1_Customized_Window-1.1.dist-info/top_level.txt
+Filename: PySide1_Customized_Window-1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: PySide1_Customized_Window-1.1.dist-info/WHEEL
+Filename: PySide1_Customized_Window-1.2.dist-info/WHEEL
 Comment: 
 
-Filename: PySide1_Customized_Window-1.1.dist-info/METADATA
+Filename: PySide1_Customized_Window-1.2.dist-info/METADATA
 Comment: 
 
-Filename: PySide1_Customized_Window-1.1.dist-info/RECORD
+Filename: PySide1_Customized_Window-1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## PySide1_Customized_Window.py

```diff
@@ -182,20 +182,20 @@
             else:
                 dpi = 96
         except:
             dpi = 96
     return dpi
 
 
-def getdefaultfont():
+def getcaptionfont():
     result = NONCLIENTMETRICS()
     result.cbSize = ctypes.sizeof(NONCLIENTMETRICS)
     ctypes.windll.user32.SystemParametersInfoW(0x29, ctypes.sizeof(NONCLIENTMETRICS), ctypes.pointer(result), 0)
-    defaultfont = result.lfMessageFont.lfFaceName
-    return defaultfont
+    captionfont = result.lfCaptionFont.lfFaceName
+    return captionfont
 
 
 class CustomizedWindow(QWidget):
     '''A customized window based on PySideX.'''
     def __init__(self):
         super(CustomizedWindow, self).__init__()
         self.hwnd = gethwnd(self)
@@ -222,44 +222,44 @@
                 ctypes.windll.user32.SetWindowLongW(self.hwnd, -4, BasicMessageHandlerAddress)
         self.setAttribute(Qt.WA_TranslucentBackground, True)
         self.hwnd = gethwnd(self)
         if ISPYSIDE1:
             ctypes.windll.user32.SetWindowLongW(self.hwnd, -16, 0x40000 | 0x20000 | 0x10000)
         else:
             ctypes.windll.user32.SetWindowLongW(self.hwnd, -16, 0xc00000 | 0x40000 | 0x20000 | 0x10000)
-        ctypes.windll.user32.SetWindowLongW(self.hwnd, -20, 0x200)
         self.isaeroenabled = isAeroEnabled()
         if self.isaeroenabled:
             if self.isblurwindow:
                 self.setBlurEffect()
             else:
                 self.setDWMShadowEffect()
-        self.dpi = getdpiforwindow_winapi(self.hwnd)
+        self.realdpi = getdpiforwindow_winapi(self.hwnd)
+        self.highdpiscalingenabled = False
+        self.highdpiscalefactorroundingpolicy = 3
+        if hasattr(Qt, 'AA_EnableHighDpiScaling'):
+            if QApplication.testAttribute(Qt.AA_EnableHighDpiScaling):
+                self.highdpiscalingenabled = True
+        if hasattr(Qt, 'HighDpiScaleFactorRoundingPolicy'):
+            self.highdpiscalefactorroundingpolicy = 4
+        self.dpi = self.getdpibyrealdpi(self.realdpi)
         dpi = self.dpi
         self.maximizedwindowborderwidth_list = self.getMaximizedWindowBorderWidth()
         self.themecolour = 0
         self.isdarktheme = isdarktheme()
         self.setMinimumSize(int(220.0 * dpi / 96.0), int(48.0 * dpi / 96.0))
-        self.border_width = int(5.0 * dpi / 96.0)
-        self.title_height = int(30.0 * dpi / 96.0)
-        self.menubutton_width = int(46.0 * dpi / 96.0)
-        self.title_font_size = int(13.0 * dpi / 96.0)
-        self.titleiconlayout_margin = int(7.0 * dpi / 96.0)
+        self.updateconstantsfordpi()
         self.inminsizebutton = False
         self.inmaxsizebutton = False
         self.inclosebutton = False
         self.intitlebar = False
         self.intopborder = False
         self.inleftborder = False
         self.inbottomborder = False
         self.inrightborder = False
-        try:
-            self.defaultfont = getdefaultfont()
-        except:
-            self.defaultfont = ''
+        self.captionfont = getcaptionfont()
         self.windowmargin_left = 0
         self.windowmargin_right = 0
         self.windowmargin_top = 0
         self.windowmargin_bottom = 0
         self.mainLayout = QVBoxLayout()
         self.mainLayout.setContentsMargins(0, 0, 0, 0)
         self.mainLayout.setSpacing(0)
@@ -318,14 +318,32 @@
             self.isdarktheme = isdarktheme()
         elif themecolour == 1:
             self.isdarktheme = False
         elif themecolour == 2:
             self.isdarktheme = True
         else:
             raise Exception
+    def setHighDpiScaleFactorRoundingPolicy(self, policy):
+        '''policy=Qt.HighDpiScaleFactorRoundingPolicy.Ceil
+policy=Qt.HighDpiScaleFactorRoundingPolicy.Floor
+policy=Qt.HighDpiScaleFactorRoundingPolicy.PassThrough
+policy=Qt.HighDpiScaleFactorRoundingPolicy.Round
+policy=Qt.HighDpiScaleFactorRoundingPolicy.RoundPreferFloor'''
+        try:
+            policy_dict = {Qt.HighDpiScaleFactorRoundingPolicy.Ceil: 1, Qt.HighDpiScaleFactorRoundingPolicy.Floor: 2, Qt.HighDpiScaleFactorRoundingPolicy.PassThrough: 3, Qt.HighDpiScaleFactorRoundingPolicy.Round: 4, Qt.HighDpiScaleFactorRoundingPolicy.RoundPreferFloor: 5}
+        except:
+            raise Exception('setHighDpiScaleFactorRoundingPolicy is only avaliable on PySideX 5.14 and newer.')
+        try:
+            self.highdpiscalefactorroundingpolicy = policy_dict[policy]
+        except:
+            raise ValueError('Argument policy must be Qt.HighDpiScaleFactorRoundingPolicy.Ceil, Qt.HighDpiScaleFactorRoundingPolicy.Floor, Qt.HighDpiScaleFactorRoundingPolicy.PassThrough, Qt.HighDpiScaleFactorRoundingPolicy.Round or Qt.HighDpiScaleFactorRoundingPolicy.RoundPreferFloor.')
+        dpi = self.getdpibyrealdpi(self.realdpi)
+        self.dpi = dpi
+        self.setMinimumSize(int(220.0 * dpi / 96.0), int(48.0 * dpi / 96.0))
+        self.updateconstantsfordpi()
     def setWindowTitle2(self, arg__1):
         self.originalSetWindowTitle(arg__1)
         self.paintTitleBarAndClientArea(self.isActiveWindow())
     def setWindowIcon2(self, icon):
         self.originalSetWindowIcon(icon)
         self.paintTitleBarAndClientArea(self.isActiveWindow())
     def paintTitleBarAndClientArea(self, isactivewindow=0, ismaximized=-1):
@@ -334,15 +352,15 @@
         SWP_NOZORDER = 0x4
         hwnd = self.hwnd
         dpi = self.dpi
         title_height = self.title_height
         menubutton_width = self.menubutton_width
         title_font_size = self.title_font_size
         titleiconlayout_margin = self.titleiconlayout_margin
-        defaultfont = self.defaultfont
+        captionfont = self.captionfont
         isblurwindow = self.isblurwindow
         isaeroenabled = self.isaeroenabled
         isdarktheme = self.isdarktheme
         if ismaximized == -1:
             ismaximized = self.isMaximized()
         self.titleBar.setLayout(self.titleBarLayout)
         self.titleBar.setFixedHeight(self.title_height)
@@ -362,15 +380,15 @@
         self.maxSizeButton.setStyleSheet('background:transparent; border-radius:0px')
         self.closeButton.setStyleSheet('background:transparent; border-radius:0px')
         titletextpalette = QPalette()
         self.titleTextLabel.setStyleSheet('''QLabel{
 background:transparent;
 font-family:'%s';
 font-size:%dpx;
-}''' % (defaultfont, title_font_size))
+}''' % (captionfont, title_font_size))
         if isdarktheme:
             try:
                 ctypes.windll.dwmapi.DwmSetWindowAttribute(hwnd, 19, ctypes.byref(ctypes.c_int(1)), ctypes.sizeof(ctypes.c_int(1)))
                 ctypes.windll.dwmapi.DwmSetWindowAttribute(hwnd, 20, ctypes.byref(ctypes.c_int(1)), ctypes.sizeof(ctypes.c_int(1)))
             except: pass
             ctypes.windll.user32.SetWindowPos(hwnd, None, 0, 0, 0, 0, SWP_NOSIZE | SWP_NOMOVE | SWP_NOZORDER)
             if isblurwindow:
@@ -535,15 +553,14 @@
         WM_NCCALCSIZE = 0x83
         WM_NCHITTEST = 0x84
         WM_NCLBUTTONDOWN = 0xa1
         WM_NCLBUTTONUP = 0xa2
         WM_LBUTTONUP = 0x2a2
         WM_DPICHANGED = 0x2e0
         WM_SYSCOMMAND = 0x112
-        WM_THEMECHANGED = 0x31a
         WM_DWMCOMPOSITIONCHANGED = 0x31e
         SW_PARENTOPENING = 0x3
         SC_SIZE = 0xf000
         SC_MOVE = 0xf010
         SC_MINIMIZE = 0xf020
         SC_MAXIMIZE = 0xf030
         SC_CLOSE = 0xf060
@@ -560,26 +577,28 @@
         HTTOPRIGHT = 0xe
         HTBOTTOM = 0xf
         HTBOTTOMLEFT = 0x10
         HTBOTTOMRIGHT = 0x11
         WVR_REDRAW = 0x300
         try:
             dpi = self.dpi
-            border_width = self.border_width
-            title_height = self.title_height
-            menubutton_width = self.menubutton_width
+            realdpi = self.realdpi
+            real_border_width = self.real_border_width
+            real_title_height = self.real_title_height
+            real_menubutton_width = self.real_menubutton_width
             windowmargin_left = self.windowmargin_left
             windowmargin_right = self.windowmargin_right
             windowmargin_top = self.windowmargin_top
             windowmargin_bottom = self.windowmargin_bottom
         except:
             dpi = 96
-            border_width = 0
-            title_height = 0
-            menubutton_width = 0
+            realdpi = 96
+            real_border_width = 0
+            real_title_height = 0
+            real_menubutton_width = 0
             windowmargin_left = 0
             windowmargin_right = 0
             windowmargin_top = 0
             windowmargin_bottom = 0
         try:
             windowrect = self.GetWindowRect()
         except:
@@ -595,22 +614,22 @@
         except:
             globalpos = POINT()
             ctypes.windll.user32.GetCursorPos(ctypes.byref(globalpos))
             x = globalpos.x - windowx
             y = globalpos.y - windowy
         width = windowrect.right - windowx
         height = windowrect.bottom - windowy
-        intitlebar = windowmargin_top <= y < title_height + windowmargin_top
-        inminsizebutton = int(width - windowmargin_left - 3 * menubutton_width) <= x < int(width - windowmargin_left - 2 * menubutton_width) and intitlebar
-        inmaxsizebutton = int(width - windowmargin_left - 2 * menubutton_width) <= x < int(width - windowmargin_left - menubutton_width) and intitlebar
-        inclosebutton = int(width - windowmargin_left - menubutton_width) <= x < int(width - windowmargin_left) and intitlebar
-        intopborder = y <= border_width
-        inleftborder = x <= border_width
-        inbottomborder = int(height - y) <= border_width
-        inrightborder = int(width - x) <= border_width
+        intitlebar = windowmargin_top <= y < real_title_height + windowmargin_top
+        inminsizebutton = int(width - windowmargin_left - 3 * real_menubutton_width) <= x < int(width - windowmargin_left - 2 * real_menubutton_width) and intitlebar
+        inmaxsizebutton = int(width - windowmargin_left - 2 * real_menubutton_width) <= x < int(width - windowmargin_left - real_menubutton_width) and intitlebar
+        inclosebutton = int(width - windowmargin_left - real_menubutton_width) <= x < int(width - windowmargin_left) and intitlebar
+        intopborder = y <= real_border_width
+        inleftborder = x <= real_border_width
+        inbottomborder = int(height - y) <= real_border_width
+        inrightborder = int(width - x) <= real_border_width
         self.inminsizebutton = inminsizebutton
         self.inmaxsizebutton = inmaxsizebutton
         self.inclosebutton = inclosebutton
         self.intitlebar = intitlebar
         self.intopborder = intopborder
         self.inleftborder = inleftborder
         self.inbottomborder = inbottomborder
@@ -678,36 +697,34 @@
             elif wParam == HTCLOSE:
                 self.closeButtonClicked()
             return ctypes.windll.user32.DefWindowProcW(hwnd, message, wParam, lParam)
         if message == WM_LBUTTONUP:
             self.setMenuButtonStyle(0)
         if message == WM_DPICHANGED:
             window_rect = RECT.from_address(lParam)
-            olddpi = self.dpi
-            dpi = wParam >> 16
-            self.dpi = dpi
+            realdpi = wParam >> 16
+            self.realdpi = realdpi
             self.maximizedwindowborderwidth_list = self.getMaximizedWindowBorderWidth()
-            self.setMinimumSize(int(220.0 * dpi / 96.0), int(48.0 * dpi / 96.0))
             x = window_rect.left
             y = window_rect.top
             width = int(window_rect.right - window_rect.left)
             height = int(window_rect.bottom - window_rect.top)
-            self.setGeometry(x, y, width, height)
-            self.border_width = int(5.0 * dpi / 96.0)
-            self.title_height = int(30.0 * dpi / 96.0)
-            self.menubutton_width = int(46.0 * dpi / 96.0)
-            self.title_font_size = int(13.0 * dpi / 96.0)
-            self.titleiconlayout_margin = int(7.0 * dpi / 96.0)
+            if not self.highdpiscalingenabled:
+                self.setGeometry(x, y, width, height)
+            dpi = self.getdpibyrealdpi(realdpi)
+            self.dpi = dpi
+            self.setMinimumSize(int(220.0 * dpi / 96.0), int(48.0 * dpi / 96.0))
+            self.updateconstantsfordpi()
             self.paintTitleBarAndClientArea(self.isActiveWindow())
-            ctypes.windll.user32.CallWindowProcW(self.originalBasicMessageHandler, hwnd, message, wParam, lParam)
-            return 0
         if message == WM_SETTINGCHANGE:
             if self.themecolour == 0 and str(ctypes.cast(lParam, ctypes.c_wchar_p).value) == 'ImmersiveColorSet':
                 self.isdarktheme = isdarktheme()
                 self.paintTitleBarAndClientArea(self.isActiveWindow())
+            if str(ctypes.cast(lParam, ctypes.c_wchar_p).value) == 'WindowMetrics':
+                self.captionfont = getcaptionfont()
         if message == WM_DWMCOMPOSITIONCHANGED:
             self.isaeroenabled = isAeroEnabled()
             if self.isaeroenabled:
                 if self.isblurwindow:
                     self.setBlurEffect()
                 else:
                     self.setDWMShadowEffect()
@@ -781,18 +798,18 @@
         WM_SYSCOMMAND = 0x112
         SC_CLOSE = 0xf060
         ctypes.windll.user32.SendMessageW(self.hwnd, WM_SYSCOMMAND, SC_CLOSE, 0)
     def getMaximizedWindowBorderWidth(self):
         SM_CXSIZEFRAME = 32
         SM_CYSIZEFRAME = 33
         SM_CXPADDEDBORDER = 92
-        dpi = self.dpi
+        realdpi = self.realdpi
         try:
-            borderwidth_x = ctypes.windll.user32.GetSystemMetricsForDpi(SM_CXSIZEFRAME, dpi) + ctypes.windll.user32.GetSystemMetricsForDpi(SM_CXPADDEDBORDER, dpi)
-            borderwidth_y = ctypes.windll.user32.GetSystemMetricsForDpi(SM_CYSIZEFRAME, dpi) + ctypes.windll.user32.GetSystemMetricsForDpi(SM_CXPADDEDBORDER, dpi)
+            borderwidth_x = ctypes.windll.user32.GetSystemMetricsForDpi(SM_CXSIZEFRAME, realdpi) + ctypes.windll.user32.GetSystemMetricsForDpi(SM_CXPADDEDBORDER, realdpi)
+            borderwidth_y = ctypes.windll.user32.GetSystemMetricsForDpi(SM_CYSIZEFRAME, realdpi) + ctypes.windll.user32.GetSystemMetricsForDpi(SM_CXPADDEDBORDER, realdpi)
         except:
             borderwidth_x = ctypes.windll.user32.GetSystemMetrics(SM_CXSIZEFRAME) + ctypes.windll.user32.GetSystemMetrics(SM_CXPADDEDBORDER)
             borderwidth_y = ctypes.windll.user32.GetSystemMetrics(SM_CYSIZEFRAME) + ctypes.windll.user32.GetSystemMetrics(SM_CXPADDEDBORDER)
         return [borderwidth_x, borderwidth_y]
     def nativeEvent(self, eventType, msg):
         '''For PySide2/6, you should define MessageHandler instead of nativeEvent.'''
         WM_NCCALCSIZE = 0x83
@@ -834,26 +851,63 @@
     def setDWMShadowEffect(self):
         hwnd = self.hwnd
         try:
             ctypes.windll.dwmapi.DwmExtendFrameIntoClientArea(hwnd, ctypes.byref(MARGINS(1, 1, 0, 0)))
             return 1
         except:
             return 0
+    def getdpibyrealdpi(self, realdpi):
+        realscalefactor = realdpi / 96.0
+        if self.highdpiscalingenabled:
+            if self.highdpiscalefactorroundingpolicy == 1:
+                if realscalefactor - int(realscalefactor) > 0:
+                    scalefactor = int(realscalefactor + 1)
+                else:
+                    scalefactor = int(realscalefactor)
+            elif self.highdpiscalefactorroundingpolicy == 2:
+                scalefactor = int(realscalefactor)
+            elif self.highdpiscalefactorroundingpolicy == 3:
+                scalefactor = realscalefactor
+            elif self.highdpiscalefactorroundingpolicy == 4:
+                if realscalefactor - int(realscalefactor) >= 0.5:
+                    scalefactor = int(realscalefactor + 1)
+                else:
+                    scalefactor = int(realscalefactor)
+            elif self.highdpiscalefactorroundingpolicy == 5:
+                if realscalefactor - int(realscalefactor) > 0.5:
+                    scalefactor = int(realscalefactor + 1)
+                else:
+                    scalefactor = int(realscalefactor)
+            dpi = int(float(realdpi) / scalefactor)
+        else:
+            dpi = realdpi
+        return dpi
     def setwin11blur(self, hWnd):
         Win11_21H2_ENTRY = 1029
         Win11_21H2_VALUE = 1
         Win11_22H2_ENTRY = 38
         Win11_22H2_VALUE = 3
         Win11_21H2_COMMAND = ctypes.windll.dwmapi.DwmSetWindowAttribute(hWnd, Win11_21H2_ENTRY,
                                                                         ctypes.byref(ctypes.c_int(Win11_21H2_VALUE)),
                                                                         ctypes.sizeof(ctypes.c_int))
         Win11_22H2_COMMAND = ctypes.windll.dwmapi.DwmSetWindowAttribute(hWnd, Win11_22H2_ENTRY,
                                                                         ctypes.byref(ctypes.c_int(Win11_22H2_VALUE)),
                                                                         ctypes.sizeof(ctypes.c_int))
         return (Win11_21H2_COMMAND, Win11_22H2_COMMAND)
+    def updateconstantsfordpi(self):
+        dpi = self.dpi
+        realdpi = self.realdpi
+        self.border_width = int(5.0 * dpi / 96.0)
+        self.title_height = int(30.0 * dpi / 96.0)
+        self.menubutton_width = int(46.0 * dpi / 96.0)
+        self.title_font_size = int(13.0 * dpi / 96.0)
+        self.real_border_width = int(5.0 * realdpi / 96.0)
+        self.real_title_height = int(30.0 * realdpi / 96.0)
+        self.real_menubutton_width = int(46.0 * realdpi / 96.0)
+        self.titleiconlayout_margin = int(7.0 * dpi / 96.0)
     def GetWindowRect(self):
         lpRect = RECT()
         ctypes.windll.user32.GetWindowRect(self.hwnd, ctypes.byref(lpRect))
         return lpRect
     def screenChangedHandler(self):
         hwnd = gethwnd(self.windowHandle())
         SWP_NOSIZE = 0x1
@@ -864,7 +918,27 @@
 
 
 class BlurWindow(CustomizedWindow):
     '''A blur window based on PySideX.
 Blur effect is avaliable on Windows Vista and newer.'''
     def __init__(self):
         super(BlurWindow, self).__init__()
+
+
+if __name__ == '__main__':
+    try:
+        QApplication.setHighDpiScaleFactorRoundingPolicy(Qt.HighDpiScaleFactorRoundingPolicy.PassThrough)
+        QApplication.setAttribute(Qt.AA_EnableHighDpiScaling, True)
+        QApplication.setAttribute(Qt.AA_UseHighDpiPixmaps, True)
+    except: pass
+    app = QApplication(sys.argv)
+    window = BlurWindow()
+    window.setWindowTitle('Window')
+    window.setDarkTheme(2)
+    try:
+        window.setHighDpiScaleFactorRoundingPolicy(Qt.HighDpiScaleFactorRoundingPolicy.PassThrough)
+    except: pass
+    window.resize(int(400.0 * window.dpi / 96.0), int(175.0 * window.dpi / 96.0))
+    window.setWindowIcon(QIcon('Icon.ico'))
+    button = QPushButton('Button', window.clientArea)
+    window.show()
+    app.exec_()
```

## Comparing `PySide1_Customized_Window-1.1.dist-info/metadata.json` & `PySide1_Customized_Window-1.2.dist-info/metadata.json`

 * *Files 2% similar despite different names*

### Pretty-printed

 * *Similarity: 0.9444444444444444%*

 * *Differences: {"'version'": "'1.2'"}*

```diff
@@ -27,9 +27,9 @@
         "GUI",
         "PySide"
     ],
     "metadata_version": "2.0",
     "name": "PySide1-Customized-Window",
     "requires_python": ">=2.6",
     "summary": "A customized window based on PySideX.",
-    "version": "1.1"
+    "version": "1.2"
 }
```

