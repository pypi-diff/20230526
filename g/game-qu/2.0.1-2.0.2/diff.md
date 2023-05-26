# Comparing `tmp/game_qu-2.0.1.tar.gz` & `tmp/game_qu-2.0.2.tar.gz`

## Comparing `game_qu-2.0.1.tar` & `game_qu-2.0.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 game_qu-2.0.1/LISCENCE
--rw-r--r--   0        0        0     5220 2020-02-02 00:00:00.000000 game_qu-2.0.1/.idea/workspace.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 game_qu-2.0.1/src/game_qu/__init__.py
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 game_qu-2.0.1/src/game_qu/game_runner.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 game_qu-2.0.1/src/game_qu/library_abstraction.py
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 game_qu-2.0.1/src/game_qu/base/colors.py
--rw-r--r--   0        0        0     5707 2020-02-02 00:00:00.000000 game_qu-2.0.1/src/game_qu/base/engines.py
--rw-r--r--   0        0        0     4496 2020-02-02 00:00:00.000000 game_qu-2.0.1/src/game_qu/base/events.py
--rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 game_qu-2.0.1/src/game_qu/base/file_reader.py
--rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 game_qu-2.0.1/src/game_qu/base/fraction.py
--rw-r--r--   0        0        0     4088 2020-02-02 00:00:00.000000 game_qu-2.0.1/src/game_qu/base/game_movement.py
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 game_qu-2.0.1/src/game_qu/base/game_runner_function.py
--rw-r--r--   0        0        0     3768 2020-02-02 00:00:00.000000 game_qu-2.0.1/src/game_qu/base/history_keeper.py
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 game_qu-2.0.1/src/game_qu/base/id_creator.py
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 game_qu-2.0.1/src/game_qu/base/important_constants.py
--rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 game_qu-2.0.1/src/game_qu/base/important_variables.py
--rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 game_qu-2.0.1/src/game_qu/base/keyboard.py
--rw-r--r--   0        0        0     3948 2020-02-02 00:00:00.000000 game_qu-2.0.1/src/game_qu/base/library_changer.py
--rw-r--r--   0        0        0     2692 2020-02-02 00:00:00.000000 game_qu-2.0.1/src/game_qu/base/library_independant_utility_functions.py
--rw-r--r--   0        0        0     5028 2020-02-02 00:00:00.000000 game_qu-2.0.1/src/game_qu/base/lines.py
--rw-r--r--   0        0        0     9141 2020-02-02 00:00:00.000000 game_qu-2.0.1/src/game_qu/base/paths.py
--rw-r--r--   0        0        0    13518 2020-02-02 00:00:00.000000 game_qu-2.0.1/src/game_qu/base/quadratic_equations.py
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 game_qu-2.0.1/src/game_qu/base/range.py
--rw-r--r--   0        0        0     6001 2020-02-02 00:00:00.000000 game_qu-2.0.1/src/game_qu/base/unique_ids_list.py
--rw-r--r--   0        0        0     9677 2020-02-02 00:00:00.000000 game_qu-2.0.1/src/game_qu/base/utility_functions.py
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 game_qu-2.0.1/src/game_qu/base/velocity_calculator.py
--rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 game_qu-2.0.1/src/game_qu/gui_components/component.py
--rw-r--r--   0        0        0     2633 2020-02-02 00:00:00.000000 game_qu-2.0.1/src/game_qu/gui_components/dimensions.py
--rw-r--r--   0        0        0     6595 2020-02-02 00:00:00.000000 game_qu-2.0.1/src/game_qu/gui_components/grid.py
--rw-r--r--   0        0        0     3652 2020-02-02 00:00:00.000000 game_qu-2.0.1/src/game_qu/gui_components/hud.py
--rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 game_qu-2.0.1/src/game_qu/gui_components/intermediate_screen.py
--rw-r--r--   0        0        0     4720 2020-02-02 00:00:00.000000 game_qu-2.0.1/src/game_qu/gui_components/navigation_screen.py
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 game_qu-2.0.1/src/game_qu/gui_components/screen.py
--rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 game_qu-2.0.1/src/game_qu/gui_components/text_box.py
--rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 game_qu-2.0.1/src/game_qu/gui_components/window.py
--rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 game_qu-2.0.1/src/game_qu/pygame_abstraction/keys.py
--rw-r--r--   0        0        0     6126 2020-02-02 00:00:00.000000 game_qu-2.0.1/src/game_qu/pygame_abstraction/utility_functions.py
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 game_qu-2.0.1/src/game_qu/pygame_abstraction/variables.py
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 game_qu-2.0.1/src/game_qu/pyglet_abstraction/keys.py
--rw-r--r--   0        0        0     6825 2020-02-02 00:00:00.000000 game_qu-2.0.1/src/game_qu/pyglet_abstraction/utility_functions.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 game_qu-2.0.1/src/game_qu/pyglet_abstraction/variables.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 game_qu-2.0.1/README.md
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 game_qu-2.0.1/pyproject.toml
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 game_qu-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 game_qu-2.0.2/LISCENCE
+-rw-r--r--   0        0        0     5330 2020-02-02 00:00:00.000000 game_qu-2.0.2/.idea/workspace.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 game_qu-2.0.2/src/game_qu/__init__.py
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 game_qu-2.0.2/src/game_qu/game_runner.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 game_qu-2.0.2/src/game_qu/library_abstraction.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 game_qu-2.0.2/src/game_qu/base/colors.py
+-rw-r--r--   0        0        0     5707 2020-02-02 00:00:00.000000 game_qu-2.0.2/src/game_qu/base/engines.py
+-rw-r--r--   0        0        0     4496 2020-02-02 00:00:00.000000 game_qu-2.0.2/src/game_qu/base/events.py
+-rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 game_qu-2.0.2/src/game_qu/base/file_reader.py
+-rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 game_qu-2.0.2/src/game_qu/base/fraction.py
+-rw-r--r--   0        0        0     4088 2020-02-02 00:00:00.000000 game_qu-2.0.2/src/game_qu/base/game_movement.py
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 game_qu-2.0.2/src/game_qu/base/game_runner_function.py
+-rw-r--r--   0        0        0     3768 2020-02-02 00:00:00.000000 game_qu-2.0.2/src/game_qu/base/history_keeper.py
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 game_qu-2.0.2/src/game_qu/base/id_creator.py
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 game_qu-2.0.2/src/game_qu/base/important_constants.py
+-rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 game_qu-2.0.2/src/game_qu/base/important_variables.py
+-rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 game_qu-2.0.2/src/game_qu/base/keyboard.py
+-rw-r--r--   0        0        0     3948 2020-02-02 00:00:00.000000 game_qu-2.0.2/src/game_qu/base/library_changer.py
+-rw-r--r--   0        0        0     2692 2020-02-02 00:00:00.000000 game_qu-2.0.2/src/game_qu/base/library_independant_utility_functions.py
+-rw-r--r--   0        0        0     5028 2020-02-02 00:00:00.000000 game_qu-2.0.2/src/game_qu/base/lines.py
+-rw-r--r--   0        0        0     9141 2020-02-02 00:00:00.000000 game_qu-2.0.2/src/game_qu/base/paths.py
+-rw-r--r--   0        0        0    13518 2020-02-02 00:00:00.000000 game_qu-2.0.2/src/game_qu/base/quadratic_equations.py
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 game_qu-2.0.2/src/game_qu/base/range.py
+-rw-r--r--   0        0        0     6001 2020-02-02 00:00:00.000000 game_qu-2.0.2/src/game_qu/base/unique_ids_list.py
+-rw-r--r--   0        0        0     9677 2020-02-02 00:00:00.000000 game_qu-2.0.2/src/game_qu/base/utility_functions.py
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 game_qu-2.0.2/src/game_qu/base/velocity_calculator.py
+-rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 game_qu-2.0.2/src/game_qu/gui_components/component.py
+-rw-r--r--   0        0        0     2633 2020-02-02 00:00:00.000000 game_qu-2.0.2/src/game_qu/gui_components/dimensions.py
+-rw-r--r--   0        0        0     6595 2020-02-02 00:00:00.000000 game_qu-2.0.2/src/game_qu/gui_components/grid.py
+-rw-r--r--   0        0        0     3652 2020-02-02 00:00:00.000000 game_qu-2.0.2/src/game_qu/gui_components/hud.py
+-rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 game_qu-2.0.2/src/game_qu/gui_components/intermediate_screen.py
+-rw-r--r--   0        0        0     4720 2020-02-02 00:00:00.000000 game_qu-2.0.2/src/game_qu/gui_components/navigation_screen.py
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 game_qu-2.0.2/src/game_qu/gui_components/screen.py
+-rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 game_qu-2.0.2/src/game_qu/gui_components/text_box.py
+-rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 game_qu-2.0.2/src/game_qu/gui_components/window.py
+-rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 game_qu-2.0.2/src/game_qu/pygame_abstraction/keys.py
+-rw-r--r--   0        0        0     6126 2020-02-02 00:00:00.000000 game_qu-2.0.2/src/game_qu/pygame_abstraction/utility_functions.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 game_qu-2.0.2/src/game_qu/pygame_abstraction/variables.py
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 game_qu-2.0.2/src/game_qu/pyglet_abstraction/keys.py
+-rw-r--r--   0        0        0     6825 2020-02-02 00:00:00.000000 game_qu-2.0.2/src/game_qu/pyglet_abstraction/utility_functions.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 game_qu-2.0.2/src/game_qu/pyglet_abstraction/variables.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 game_qu-2.0.2/README.md
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 game_qu-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 game_qu-2.0.2/PKG-INFO
```

### Comparing `game_qu-2.0.1/LISCENCE` & `game_qu-2.0.2/LISCENCE`

 * *Files identical despite different names*

### Comparing `game_qu-2.0.1/.idea/workspace.xml` & `game_qu-2.0.2/.idea/workspace.xml`

 * *Files 5% similar despite different names*

#### Comparing `game_qu-2.0.1/.idea/workspace.xml` & `game_qu-2.0.2/.idea/workspace.xml`

```diff
@@ -49,14 +49,17 @@
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="Git.Settings">
     <option name="RECENT_GIT_ROOT_PATH" value="$PROJECT_DIR$"/>
   </component>
+  <component name="MarkdownSettingsMigration">
+    <option name="stateVersion" value="1"/>
+  </component>
   <component name="ProjectId" id="2QIPWLXi9RhYvCt0e7Eygcoes3S"/>
   <component name="ProjectViewState">
     <option name="hideEmptyMiddlePackages" value="true"/>
     <option name="showLibraryContents" value="true"/>
   </component>
   <component name="PropertiesComponent"><![CDATA[{
   "keyToString": {
```

### Comparing `game_qu-2.0.1/src/game_qu/base/colors.py` & `game_qu-2.0.2/src/game_qu/base/colors.py`

 * *Files identical despite different names*

### Comparing `game_qu-2.0.1/src/game_qu/base/engines.py` & `game_qu-2.0.2/src/game_qu/base/engines.py`

 * *Files identical despite different names*

### Comparing `game_qu-2.0.1/src/game_qu/base/events.py` & `game_qu-2.0.2/src/game_qu/base/events.py`

 * *Files identical despite different names*

### Comparing `game_qu-2.0.1/src/game_qu/base/file_reader.py` & `game_qu-2.0.2/src/game_qu/base/file_reader.py`

 * *Files identical despite different names*

### Comparing `game_qu-2.0.1/src/game_qu/base/fraction.py` & `game_qu-2.0.2/src/game_qu/base/fraction.py`

 * *Files identical despite different names*

### Comparing `game_qu-2.0.1/src/game_qu/base/game_movement.py` & `game_qu-2.0.2/src/game_qu/base/game_movement.py`

 * *Files identical despite different names*

### Comparing `game_qu-2.0.1/src/game_qu/base/game_runner_function.py` & `game_qu-2.0.2/src/game_qu/base/game_runner_function.py`

 * *Files identical despite different names*

### Comparing `game_qu-2.0.1/src/game_qu/base/history_keeper.py` & `game_qu-2.0.2/src/game_qu/base/history_keeper.py`

 * *Files identical despite different names*

### Comparing `game_qu-2.0.1/src/game_qu/base/id_creator.py` & `game_qu-2.0.2/src/game_qu/base/id_creator.py`

 * *Files identical despite different names*

### Comparing `game_qu-2.0.1/src/game_qu/base/important_variables.py` & `game_qu-2.0.2/src/game_qu/base/important_variables.py`

 * *Files identical despite different names*

### Comparing `game_qu-2.0.1/src/game_qu/base/keyboard.py` & `game_qu-2.0.2/src/game_qu/base/keyboard.py`

 * *Files identical despite different names*

### Comparing `game_qu-2.0.1/src/game_qu/base/library_changer.py` & `game_qu-2.0.2/src/game_qu/base/library_changer.py`

 * *Files identical despite different names*

### Comparing `game_qu-2.0.1/src/game_qu/base/library_independant_utility_functions.py` & `game_qu-2.0.2/src/game_qu/base/library_independant_utility_functions.py`

 * *Files identical despite different names*

### Comparing `game_qu-2.0.1/src/game_qu/base/lines.py` & `game_qu-2.0.2/src/game_qu/base/lines.py`

 * *Files identical despite different names*

### Comparing `game_qu-2.0.1/src/game_qu/base/paths.py` & `game_qu-2.0.2/src/game_qu/base/paths.py`

 * *Files identical despite different names*

### Comparing `game_qu-2.0.1/src/game_qu/base/quadratic_equations.py` & `game_qu-2.0.2/src/game_qu/base/quadratic_equations.py`

 * *Files identical despite different names*

### Comparing `game_qu-2.0.1/src/game_qu/base/range.py` & `game_qu-2.0.2/src/game_qu/base/range.py`

 * *Files identical despite different names*

### Comparing `game_qu-2.0.1/src/game_qu/base/unique_ids_list.py` & `game_qu-2.0.2/src/game_qu/base/unique_ids_list.py`

 * *Files identical despite different names*

### Comparing `game_qu-2.0.1/src/game_qu/base/utility_functions.py` & `game_qu-2.0.2/src/game_qu/base/utility_functions.py`

 * *Files identical despite different names*

### Comparing `game_qu-2.0.1/src/game_qu/base/velocity_calculator.py` & `game_qu-2.0.2/src/game_qu/base/velocity_calculator.py`

 * *Files identical despite different names*

### Comparing `game_qu-2.0.1/src/game_qu/gui_components/component.py` & `game_qu-2.0.2/src/game_qu/gui_components/component.py`

 * *Files identical despite different names*

### Comparing `game_qu-2.0.1/src/game_qu/gui_components/dimensions.py` & `game_qu-2.0.2/src/game_qu/gui_components/dimensions.py`

 * *Files identical despite different names*

### Comparing `game_qu-2.0.1/src/game_qu/gui_components/grid.py` & `game_qu-2.0.2/src/game_qu/gui_components/grid.py`

 * *Files identical despite different names*

### Comparing `game_qu-2.0.1/src/game_qu/gui_components/hud.py` & `game_qu-2.0.2/src/game_qu/gui_components/hud.py`

 * *Files identical despite different names*

### Comparing `game_qu-2.0.1/src/game_qu/gui_components/intermediate_screen.py` & `game_qu-2.0.2/src/game_qu/gui_components/intermediate_screen.py`

 * *Files identical despite different names*

### Comparing `game_qu-2.0.1/src/game_qu/gui_components/navigation_screen.py` & `game_qu-2.0.2/src/game_qu/gui_components/navigation_screen.py`

 * *Files identical despite different names*

### Comparing `game_qu-2.0.1/src/game_qu/gui_components/screen.py` & `game_qu-2.0.2/src/game_qu/gui_components/screen.py`

 * *Files identical despite different names*

### Comparing `game_qu-2.0.1/src/game_qu/gui_components/text_box.py` & `game_qu-2.0.2/src/game_qu/gui_components/text_box.py`

 * *Files identical despite different names*

### Comparing `game_qu-2.0.1/src/game_qu/gui_components/window.py` & `game_qu-2.0.2/src/game_qu/gui_components/window.py`

 * *Files identical despite different names*

### Comparing `game_qu-2.0.1/src/game_qu/pygame_abstraction/keys.py` & `game_qu-2.0.2/src/game_qu/pygame_abstraction/keys.py`

 * *Files identical despite different names*

### Comparing `game_qu-2.0.1/src/game_qu/pygame_abstraction/utility_functions.py` & `game_qu-2.0.2/src/game_qu/pygame_abstraction/utility_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,36 +43,36 @@
     if is_centered:
         text_rectangle.center = [left_edge, top_edge]
 
     else:
         text_rectangle.left = left_edge
         text_rectangle.top = top_edge
 
-    variables.window.blit(rendered_text, text_rectangle)
+    variables.WINDOW.blit(rendered_text, text_rectangle)
 
 def render_image(path_to_image, left_edge, top_edge, length, height):
     """Renders the image onto the screen"""
 
     left_edge, top_edge, length, height = convert_to_int(left_edge, top_edge, length, height)
     image = images.get(path_to_image)
     image = pygame.transform.scale(image, (length, height))
-    variables.window.blit(image, (left_edge, top_edge))
+    variables.WINDOW.blit(image, (left_edge, top_edge))
 
 def render_rectangle(left_edge, top_edge, length, height, color):
     """Renders the rectangle onto the screen"""
 
     left_edge, top_edge, length, height = convert_to_int(left_edge, top_edge, length, height)
-    pygame.draw.rect(variables.window, color, [left_edge, top_edge, length, height])
+    pygame.draw.rect(variables.WINDOW, color, [left_edge, top_edge, length, height])
 
 def set_up_window(length, height, background_color, title):
     """Initializes all the pygame code, so the game be run and rendered"""
 
     if not important_constants.IS_FULL_SCREEN:
         length, height = convert_to_int(length, height)
-        variables.window = pygame.display.set_mode((length, height))
+        variables.WINDOW = pygame.display.set_mode((length, height))
 
     pygame.display.set_caption(title)
     variables.background_color = background_color
 
 
 def key_is_pressed(keyboard_key):
     """:returns: bool; if the 'keyboard_key' is currently pressed this game cycle"""
@@ -129,15 +129,15 @@
     while True:
         start_time = time.time()
         for event in pygame.event.get():
             if event.type == pygame.QUIT:
                 # on_close_function()
                 pygame.quit()
 
-        variables.window.fill(variables.background_color)
+        variables.WINDOW.fill(variables.background_color)
 
         function(start_time, True, True)
         pygame.display.update()
 
 def run_checking_closing():
     """Runs all the pygame code that checks to make sure the game should be closed"""
```

### Comparing `game_qu-2.0.1/src/game_qu/pyglet_abstraction/keys.py` & `game_qu-2.0.2/src/game_qu/pyglet_abstraction/keys.py`

 * *Files identical despite different names*

### Comparing `game_qu-2.0.1/src/game_qu/pyglet_abstraction/utility_functions.py` & `game_qu-2.0.2/src/game_qu/pyglet_abstraction/utility_functions.py`

 * *Files identical despite different names*

