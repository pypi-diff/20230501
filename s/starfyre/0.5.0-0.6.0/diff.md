# Comparing `tmp/starfyre-0.5.0.tar.gz` & `tmp/starfyre-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data
+gzip compressed data, was "starfyre-0.6.0.tar", max compression
```

## Comparing `starfyre-0.5.0.tar` & `starfyre-0.6.0.tar`

### file list

```diff
@@ -1,31 +1,14 @@
--rw-r--r--   0        0        0      410 1970-01-01 00:00:00.000000 starfyre-0.5.0/Cargo.toml
--rw-r--r--   0      501       20      225 2023-02-21 21:24:47.000000 starfyre-0.5.0/.cargo/config
--rw-r--r--   0      501       20     5987 2023-02-24 00:14:57.000000 starfyre-0.5.0/.github/workflows/release-CI.yml
--rw-r--r--   0      501       20      823 2023-02-27 19:03:24.000000 starfyre-0.5.0/.gitignore
--rw-r--r--   0      501       20     1302 2023-02-04 15:04:41.000000 starfyre-0.5.0/LICENCE.md
--rw-r--r--   0      501       20     3775 2023-02-27 19:03:24.000000 starfyre-0.5.0/Makefile
--rw-r--r--   0      501       20     2028 2023-02-27 19:03:24.000000 starfyre-0.5.0/README.md
--rwxr-xr-x   0      501       20      163 2023-02-04 04:03:42.000000 starfyre-0.5.0/build.sh
--rw-r--r--   0      501       20      555 2023-02-04 04:03:42.000000 starfyre-0.5.0/poetry.lock
--rw-r--r--   0      501       20     1229 2023-02-22 22:43:44.000000 starfyre-0.5.0/pyproject.toml
--rwxr-xr-x   0      501       20      140 2023-02-24 00:05:03.000000 starfyre-0.5.0/release-build.sh
--rw-r--r--   0      501       20       24 2023-02-16 20:02:23.000000 starfyre-0.5.0/requirements-dev.txt
--rw-r--r--   0      501       20     1488 2023-01-21 19:32:28.000000 starfyre-0.5.0/src/lib.rs
--rw-r--r--   0      501       20     1871 2023-02-21 21:24:47.000000 starfyre-0.5.0/starfyre/__init__.py
--rw-r--r--   0      501       20     1282 2023-02-21 21:24:47.000000 starfyre-0.5.0/starfyre/component.py
--rw-r--r--   0      501       20     2613 2023-02-21 21:24:47.000000 starfyre-0.5.0/starfyre/dom_methods.py
--rw-r--r--   0      501       20      126 2023-02-21 21:24:47.000000 starfyre-0.5.0/starfyre/global_components.py
--rw-r--r--   0      501       20     7924 2023-02-27 19:03:24.000000 starfyre-0.5.0/starfyre/parser.py
--rw-r--r--   0      501       20     1099 2023-02-21 21:24:47.000000 starfyre-0.5.0/starfyre/store.py
--rw-r--r--   0      501       20     1887 2023-02-15 22:00:53.000000 starfyre-0.5.0/test-application/Makefile
--rw-r--r--   0      501       20      246 2023-02-04 03:44:42.000000 starfyre-0.5.0/test-application/README.md
--rw-r--r--   0      501       20      555 2023-01-08 20:51:13.000000 starfyre-0.5.0/test-application/poetry.lock
--rw-r--r--   0      501       20      959 2023-02-27 19:03:24.000000 starfyre-0.5.0/test-application/public/index.html
--rw-r--r--   0      501       20      330 2023-02-16 20:02:23.000000 starfyre-0.5.0/test-application/pyproject.toml
--rw-r--r--   0      501       20       17 2023-02-15 22:00:53.000000 starfyre-0.5.0/test-application/requirements-dev.txt
--rw-r--r--   0      501       20      391 2023-02-21 21:55:13.000000 starfyre-0.5.0/test-application/src/__init__.py
--rw-r--r--   0      501       20      482 2023-02-21 21:55:14.000000 starfyre-0.5.0/test-application/src/counter.py
--rw-r--r--   0      501       20      377 2023-02-21 21:55:30.000000 starfyre-0.5.0/test-application/src/display.py
--rw-r--r--   0      501       20       79 2023-02-04 00:00:53.000000 starfyre-0.5.0/test-application/src/state.py
--rw-r--r--   0      501       20     7175 2023-02-23 22:04:08.000000 starfyre-0.5.0/Cargo.lock
--rw-r--r--   0        0        0     2712 1970-01-01 00:00:00.000000 starfyre-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     2028 2023-02-27 19:03:24.900264 starfyre-0.6.0/README.md
+-rw-r--r--   0        0        0      454 2023-04-30 23:22:27.844670 starfyre-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1099 2023-04-30 23:09:33.032653 starfyre-0.6.0/starfyre/__init__.py
+-rw-r--r--   0        0        0     1603 2023-04-30 23:09:53.013426 starfyre-0.6.0/starfyre/__main__.py
+-rw-r--r--   0        0        0     4539 2023-04-30 22:55:52.651301 starfyre-0.6.0/starfyre/compiler.py
+-rw-r--r--   0        0        0      535 2023-04-30 22:55:52.651503 starfyre-0.6.0/starfyre/component.py
+-rw-r--r--   0        0        0     4135 2023-04-30 22:55:52.651684 starfyre-0.6.0/starfyre/dom_methods.py
+-rw-r--r--   0        0        0      126 2023-02-21 21:24:47.371882 starfyre-0.6.0/starfyre/global_components.py
+-rw-r--r--   0        0        0        0 2023-04-30 23:03:59.576897 starfyre-0.6.0/starfyre/js/__init__.py
+-rw-r--r--   0        0        0     1093 2023-04-30 23:00:43.156472 starfyre-0.6.0/starfyre/js/store.js
+-rw-r--r--   0        0        0     8837 2023-04-30 22:55:52.651893 starfyre-0.6.0/starfyre/parser.py
+-rw-r--r--   0        0        0     3544 2023-04-30 22:55:52.652044 starfyre-0.6.0/starfyre/transpiler.py
+-rw-r--r--   0        0        0     2774 1970-01-01 00:00:00.000000 starfyre-0.6.0/setup.py
+-rw-r--r--   0        0        0     2566 1970-01-01 00:00:00.000000 starfyre-0.6.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `starfyre-0.5.0/README.md` & `starfyre-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `starfyre-0.5.0/starfyre/dom_methods.py` & `starfyre-0.6.0/starfyre/dom_methods.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,84 +1,141 @@
 import re
 from functools import partial
+from uuid import uuid4
 
-import js
-from pyodide import create_proxy
+from .transpiler import transpile_to_js
+
+
+# # import js
+# from pyodide import create_proxy
 
 
 from .component import Component
 
 
-def assign_event_listeners(component: Component, event_listeners):
-    for event_listener_name, event_listener in event_listeners.items():
-        event_type = event_listener_name.lower()[2:]
-        print(
-            "Assigning event listeners to the component",
-            component,
-            event_type,
-            event_listener,
-        )
-        component.dom.addEventListener(event_type, create_proxy(event_listener))
+def assign_event_listeners(event_listener_name, event_listener):
+    # component.dom.addEventListener(event_type, create_proxy(event_listener))
+    js_event_listener = transpile_to_js(event_listener)
+    html = f" {event_listener_name}='{event_listener.__name__}()' "
+
+    return html, js_event_listener
+
+
+# there should be two renders
+
+
+# render page and render component
+def render_helper(component: Component) -> tuple[str, str, str]:
+    # Add event listeners
+    def is_listener(name):
+        return name.startswith("on")
 
+    def is_attribute(name):
+        return not is_listener(name) and name != "children"
 
-def render(component: Component):
-    parentElement = component.parentDom
+    parentElement = component.parentComponent
+    html = "\n"
+    css = "\n"
+    js = "\n"
     if parentElement is None:
-        parentElement = js.document.createElement("div")
-        parentElement.id = "root"
-        js.document.body.appendChild(parentElement)
-
-    component.parentDom = parentElement
-    # we will add rust later
-    # dom_node = DomNode(element.tag, element.props, element.children, element.event_listeners, element.state or {})
-    # dom_node.set_parent_element(parentDom)
-    # print(dom_node)
+        # instead of creating an element with js
+        # we need to create a div string
+
+        parentElement = Component("div", {"id": "root"}, [], {}, {}, uuid=uuid4())
+        component.parentComponent = parentElement
+
+        # ??
+        # cannot use js
+        # js.document.body.appendChild(parentElement)
 
     tag = component.tag
     props = component.props
     state = component.state
     data = component.data
-    print(data)
+    event_listeners = component.event_listeners
 
     # Create DOM element
     if component.is_text_component:
         # find all the names in "{}" and print them
         matches = re.findall(r"{(.*?)}", data)
         for match in matches:
             if match in state:
                 function = state[match]
                 function = partial(function, component)
                 data = component.data.replace(f"{{{ match }}}", str(function()))
-        dom = js.document.createTextNode(data)
-        print("Text Node", component)
-    else:
-        dom = js.document.createElement(tag)
+            else:
+                print("No match found for", match)
 
-    component.dom = dom
+        component.parentComponent.uuid = component.uuid
+        html += f"{data}\n"
+        component.html = html
+
+        if component.signal:
+            js += f"""
+                component = document.getElementById('{component.uuid}');
+                addDomIdToMap('{component.uuid}', "{ component.signal }");
+                if (component) {{
+                   component.innerText = `${{{ component.signal }}}`;
+                }}
+            """
+
+        return html, css, js
+
+    if component.css:
+        css += f"{ component.css }\n"
 
-    # Add event listeners
-    def isListener(name):
-        return name.startswith("on")
-    def isAttribute(name):
-        return not isListener(name) and name != "children"
+    if component.js:
+        js += f"{component.js}\n"
 
-    assign_event_listeners(component, component.event_listeners)
-    # set attributes
+    html += f"<{tag} id='{component.uuid}' "
 
+    # this is not when the component is a text component
+    prop_string = ""
     for name in props:
-        if isAttribute(name):
-            dom.setAttribute(name, props[name])
+        if is_attribute(name):
+            prop_string += f" {name}='{props[name]}' "
+
+    for name, function in event_listeners.items():
+        if is_listener(name):
+            new_html, new_js = assign_event_listeners(name, function)
+            js += new_js
+            html += new_html
+
+    if html.endswith(">"):
+        html.removesuffix(">")
+
+    if not component.is_text_component:
+        html += f"{prop_string} >"
 
     # Render children
     children = component.children
     # childElements.forEach(childElement => render(childElement, dom));
     for childElement in children:
-        childElement.parentDom = dom
-        render(childElement)
+        childElement.parentElement = component
+        new_html, new_css, new_js = render_helper(childElement)
+        html += new_html
+        css += new_css
+        js += new_js
+
+    html += f"</{tag}>\n"
 
+    component.html = html
+    return html, css, js
     # // Append to parent
     # need to apply batch updates here
     # also create a tree of dom nodes in the first place
-    if parentElement.contains(dom):
-        parentElement.replaceChild(dom, parentElement.childNodes[0])
-    else:
-        parentElement.appendChild(dom)
+    # if parentElement.contains(dom):
+    #     parentElement.replaceChild(dom, parentElement.childNodes[0])
+    # else:
+    #     parentElement.appendChild(dom)
+
+
+def render(component: Component) -> str:
+    html, css, js = render_helper(component)
+    final_html = f"<style>{css}</style>{html}<script>{js}</script>"
+    return final_html
+
+
+def render_root(component: Component) -> str:
+    html, css, js = render_helper(component)
+    final_html = f"<style>{css}</style><div id='root'>{html}</div><script>{js}</script>"
+    return final_html
```

### Comparing `starfyre-0.5.0/starfyre/parser.py` & `starfyre-0.6.0/starfyre/parser.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 import re
 from html.parser import HTMLParser
+from uuid import uuid4
+
+from starfyre.transpiler import transpile
 
 from .component import Component
 
 
 def extract_functions(obj):
     functions = {}
     for key, value in obj.items():
@@ -12,51 +15,51 @@
 
     return functions
 
 
 class RootParser(HTMLParser):
     generic_tags = ["div", "p", "b", "span", "i", "button"]
 
-    def __init__(self, component_local_variables, component_global_variables):
+    def __init__(self, component_local_variables, component_global_variables, css, js):
         super().__init__()
         self.stack: list[tuple[Component, int]] = []
         self.children = []
         self.current_depth = 0
+        self.css = css
+        self.js = js
 
         # these are the event handlers and the props
         self.local_variables = component_local_variables
         self.global_variables = component_global_variables
-        self.components = self.extract_components(component_local_variables)
-        print("These are the self components", self.components)
+
+        self.components = self.extract_components(
+            {**self.local_variables, **self.global_variables}
+        )
         # populate the dict with the components
 
     def extract_components(self, local_functions):
         components = {}
         for key, value in local_functions.items():
             if isinstance(value, Component):
                 components[key] = value
 
         return components
 
     def is_event_listener(self, name):
         return name.startswith("on")
 
-    def is_state(self, function):
-        return "create_signal" in str(function)
-
     def handle_starttag(self, tag, attrs):
         # logic should be to just create an empty component on start
         # and fill the contents on the end tag
         props = {}
         state = {}
         event_listeners = {}
         self.current_depth += 1
 
         for attr in attrs:
-            print("These are the new parse attributes", attr)
             if attr[1].startswith("{") and attr[1].endswith("}"):
                 attr_value = attr[1].strip("{").strip("}").strip(" ")
                 if self.is_event_listener(attr[0]):
                     event_handler = None
                     if attr_value in self.global_variables:
                         event_handler = self.global_variables[attr_value]
 
@@ -83,131 +86,177 @@
         if tag not in self.generic_tags and tag in self.components:
             component = self.components[tag]
             tag = component.tag
             component.props = {**component.props, **props}
             component.state = {**component.state, **state}
             component.event_listeners = {**component.event_listeners, **event_listeners}
             self.stack.append((component, self.current_depth))
-            printable_stack = [element[0].tag for element in self.stack]
-            print(
-                "Encountered a start tag :",
-                tag,
-                printable_stack,
-                "Current depth",
-                self.current_depth,
-            )
 
             return
 
-        # see if the attribute value is a state component
-        # if it is, we use the state component
-
-        # instead of creating a new component, we check if the tag is a global component
-        # then we check the uuid of the global component
-        # if the uuid is not in the stack, we create a new component
-        # if the uuid is in the stack, we use the component from the stack
-        # we are using a hack for now
-
-        # if the component has already been called
-        # and then we evaluate -> it will be in the store but with the wrong name
-        # but we don't care about the name
-        # we can just replace it with the new name
-        # but the issue will be the new props that we can pass
-        # lets not worry about that for now
-
-        component = Component(tag, props, [], event_listeners, state)
+        component = Component(
+            tag,
+            props,
+            [],
+            event_listeners,
+            state,
+            js=self.js,
+            css=self.css,
+            uuid=uuid4(),
+        )
 
         # instead of assiging tags we assign uuids
         self.stack.append((component, self.current_depth))
-        printable_stack = [element[0].tag for element in self.stack]
-        print(
-            "Encountered a start tag :",
-            tag,
-            printable_stack,
-            "Current depth",
-            self.current_depth,
-        )
+        [(element[0].tag, element[1]) for element in self.stack]
 
     def handle_endtag(self, tag):
         # we need to check if the tag is a default component or a custom component
         # if it is a custom component, we get the element from the custom components dict
         if tag not in self.generic_tags and tag in self.components:
             component = self.components[tag]
             tag = component.tag
 
-        print(
-            "Encountered an end tag :",
-            tag,
-            "Current depth",
-            self.current_depth,
-            "Stack",
-            self.stack,
-            "Children",
-            self.children,
-        )
+        # need to check the if this is always true
         parent_node, parent_depth = self.stack[
             -1
         ]  # based on the assumption that the stack is not empty
-        # need to check the if this is always true
 
         while len(self.children) > 0:
             child, child_depth = self.children[0]
-            print("These are the children", child, child_depth)
             if child_depth == parent_depth + 1:
                 self.children.pop(0)
                 self.stack[-1][0].children.insert(0, child)
-                print("Added child", child.tag, "to parent", parent_node.tag)
             else:
                 break  # we have reached the end of the children
 
         self.stack.pop()
-        self.current_depth = parent_depth
-        self.children.insert(0, (parent_node, parent_depth))
+        self.current_depth -= 1
+
+        if parent_node.tag != "style" and parent_node.tag != "script":
+            self.children.insert(0, (parent_node, parent_depth))
+
+    def is_signal(self, str):
+        if not str:
+            return False
+        return "signal" in str
+
+    def inject_uuid(self, signal, uuid):
+        return signal.replace("()", f"('{uuid}')")
 
     def handle_data(self, data):
+        # this is doing too much
+        # lexing
+        # parsing
+
         data = data.strip().strip("\n").strip(" ")
+        # regex to find all the elements that are wrapped in {}
+
         matches = re.findall(r"{(.*?)}", data)
 
         state = {}
-        print("These are the matches in the text data", matches, data)
+
+        parent_node, parent_depth = self.stack[-1]
+        uuid = uuid4()
+        component_signal = ""
 
         for match in matches:
             # match can be a sentece so we will split it
             current_data = None
             if match in self.local_variables:
                 current_data = self.local_variables[match]
             elif match in self.global_variables:
                 current_data = self.global_variables[match]
             else:
-                raise Exception("Variable not found")
+                # we need to handle a case where the eval result is a signal object
+                if self.is_signal(match):
+                    new_js = transpile(match)
+                    new_js = self.inject_uuid(new_js, uuid)
+                    component_signal = new_js.strip("{").strip("}").strip(";")
+                    print("new js", new_js)
+                    # inject uuid in the signal function call
 
-            if not self.is_state(current_data) and not callable(current_data):
-                data = data.replace(match, current_data)
-            elif self.is_state(current_data):
-                state[match] = current_data
+                    current_data = new_js
+
+                else:
+                    eval_result = eval(
+                        match, self.local_variables, self.global_variables
+                    )
+                    if isinstance(eval_result, Component):
+                        self.stack[-1][0].children.append(eval_result)
+                        return
+                    elif isinstance(eval_result, str):
+                        current_data = eval_result
+                    elif isinstance(eval_result, list):
+                        current_data = " ".join([str(i) for i in eval_result])
+                    else:
+                        # we need to handle a case where the eval result is a state object
+
+                        raise Exception("Variable not found")
+
+            if not self.is_signal(current_data) and not callable(current_data):
+                print("current data", current_data)
+                if matches:
+                    data = data.replace("{", "").replace("}", "")
+                data = data.replace(match, str(current_data))
 
         if data == "":
             return
 
         # matches can be of 4 types
         # 1. {{variable}} 2. {{function()}} 3. Props = these are all just local and global variables
         # 4. State
 
         # TODO handle state in text node
 
-        self.current_depth += 1
         # this should never be in the parent stack
         # a text node is a child node as soon as it is created
-        print("Encountered some text data :", data, "Current depth", self.current_depth)
-        self.children.append(
-            (
-                Component("TEXT_NODE", {}, [], {}, state=state, data=data),
-                self.current_depth,
+
+        # add a parent component
+        # on the wrapper div component
+
+        wrapper_div_component = Component(
+            "div",
+            {},
+            [],
+            {},
+            state=state,
+            data=data,
+            css=self.css,
+            js=self.js,
+            signal="",
+            uuid=uuid,
+        )
+
+        wrapper_div_component.children.append(
+            Component(
+                "TEXT_NODE",
+                {},
+                [],
+                {},
+                state=state,
+                data=data,
+                css=self.css,
+                js=self.js,
+                signal=component_signal,
+                uuid=uuid,
             )
         )
-        self.current_depth -= 1
+
+        parent_node.children.insert(0, wrapper_div_component)
+
+        print(
+            "parent node",
+            parent_node.tag,
+            parent_node.children,
+            "for the text node ",
+            data,
+        )
 
     def get_stack(self):
         return self.stack
 
     def get_root(self):
-        return self.children[0][0]
+        if len(self.children) != 0:
+            return self.children[0][0]
+        return Component(
+            "div", {}, [], {}, state={}, data="", css=self.css, js=self.js, uuid=uuid4()
+        )
```

### Comparing `starfyre-0.5.0/PKG-INFO` & `starfyre-0.6.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: starfyre
-Version: 0.5.0
-Classifier: Development Status :: 3 - Alpha
-Classifier: Environment :: Web Environment
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Rust
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
+Version: 0.6.0
+Summary: A Python Framework for writing Reactive web Front-Ends
+License: BSD 2.0
+Author: Sanskar Jethi
+Author-email: sansyrox@gmail.com
+Requires-Python: >=3.10,<4.0
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-License-File: LICENCE.md
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: requests (>=2.29.0,<3.0.0)
+Description-Content-Type: text/markdown
 
 
 <img alt="Starfyre Logo" src="https://user-images.githubusercontent.com/29942790/221331176-609e156a-3896-4c1a-9386-7bf595dfb879.png" width="350" />
 
 # Starfyre ⭐🔥
 
 ## Introduction:
```

