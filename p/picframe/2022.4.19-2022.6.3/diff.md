# Comparing `tmp/picframe-2022.4.19.tar.gz` & `tmp/picframe-2022.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picframe-2022.4.19.tar", last modified: Tue Apr 19 14:58:51 2022, max compression
+gzip compressed data, was "picframe-2022.6.3.tar", last modified: Fri Jun  3 11:29:58 2022, max compression
```

## Comparing `picframe-2022.4.19.tar` & `picframe-2022.6.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-19 14:58:51.410189 picframe-2022.4.19/
--rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-04-19 14:58:38.000000 picframe-2022.4.19/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3409 2022-04-19 14:58:51.410189 picframe-2022.4.19/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2775 2022-04-19 14:58:38.000000 picframe-2022.4.19/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-19 14:58:51.410189 picframe-2022.4.19/picframe/
--rw-r--r--   0 runner    (1001) docker     (121)       93 2022-04-19 14:58:38.000000 picframe-2022.4.19/picframe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      502 2022-04-19 14:58:51.410189 picframe-2022.4.19/picframe/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)    12008 2022-04-19 14:58:38.000000 picframe-2022.4.19/picframe/controller.py
--rw-r--r--   0 runner    (1001) docker     (121)     1938 2022-04-19 14:58:38.000000 picframe-2022.4.19/picframe/geo_reverse.py
--rw-r--r--   0 runner    (1001) docker     (121)     7254 2022-04-19 14:58:38.000000 picframe-2022.4.19/picframe/get_image_meta.py
--rw-r--r--   0 runner    (1001) docker     (121)    24078 2022-04-19 14:58:38.000000 picframe-2022.4.19/picframe/image_cache.py
--rw-r--r--   0 runner    (1001) docker     (121)     6922 2022-04-19 14:58:38.000000 picframe-2022.4.19/picframe/interface_http.py
--rw-r--r--   0 runner    (1001) docker     (121)    22331 2022-04-19 14:58:38.000000 picframe-2022.4.19/picframe/interface_mqtt.py
--rw-r--r--   0 runner    (1001) docker     (121)    14392 2022-04-19 14:58:38.000000 picframe-2022.4.19/picframe/interface_peripherals.py
--rw-r--r--   0 runner    (1001) docker     (121)    21060 2022-04-19 14:58:38.000000 picframe-2022.4.19/picframe/mat_image.py
--rw-r--r--   0 runner    (1001) docker     (121)    18160 2022-04-19 14:58:38.000000 picframe-2022.4.19/picframe/model.py
--rw-r--r--   0 runner    (1001) docker     (121)     5858 2022-04-19 14:58:38.000000 picframe-2022.4.19/picframe/start.py
--rw-r--r--   0 runner    (1001) docker     (121)    26333 2022-04-19 14:58:38.000000 picframe-2022.4.19/picframe/viewer_display.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-19 14:58:51.410189 picframe-2022.4.19/picframe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3409 2022-04-19 14:58:51.000000 picframe-2022.4.19/picframe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      619 2022-04-19 14:58:51.000000 picframe-2022.4.19/picframe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-19 14:58:51.000000 picframe-2022.4.19/picframe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-04-19 14:58:51.000000 picframe-2022.4.19/picframe.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-19 14:58:51.000000 picframe-2022.4.19/picframe.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-04-19 14:58:51.000000 picframe-2022.4.19/picframe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-04-19 14:58:51.000000 picframe-2022.4.19/picframe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      205 2022-04-19 14:58:51.410189 picframe-2022.4.19/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1591 2022-04-19 14:58:38.000000 picframe-2022.4.19/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-19 14:58:51.410189 picframe-2022.4.19/test/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-19 14:58:38.000000 picframe-2022.4.19/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4341 2022-04-19 14:58:38.000000 picframe-2022.4.19/test/test_get_image_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 11:29:58.723932 picframe-2022.6.3/
+-rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-06-03 11:29:47.000000 picframe-2022.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     3408 2022-06-03 11:29:58.723932 picframe-2022.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2775 2022-06-03 11:29:47.000000 picframe-2022.6.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 11:29:58.723932 picframe-2022.6.3/picframe/
+-rw-r--r--   0 runner    (1001) docker     (121)       93 2022-06-03 11:29:47.000000 picframe-2022.6.3/picframe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      502 2022-06-03 11:29:58.723932 picframe-2022.6.3/picframe/_version.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12097 2022-06-03 11:29:47.000000 picframe-2022.6.3/picframe/controller.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1938 2022-06-03 11:29:47.000000 picframe-2022.6.3/picframe/geo_reverse.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7254 2022-06-03 11:29:47.000000 picframe-2022.6.3/picframe/get_image_meta.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24078 2022-06-03 11:29:47.000000 picframe-2022.6.3/picframe/image_cache.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6922 2022-06-03 11:29:47.000000 picframe-2022.6.3/picframe/interface_http.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23748 2022-06-03 11:29:47.000000 picframe-2022.6.3/picframe/interface_mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14392 2022-06-03 11:29:47.000000 picframe-2022.6.3/picframe/interface_peripherals.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21060 2022-06-03 11:29:47.000000 picframe-2022.6.3/picframe/mat_image.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18252 2022-06-03 11:29:47.000000 picframe-2022.6.3/picframe/model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5991 2022-06-03 11:29:47.000000 picframe-2022.6.3/picframe/start.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27258 2022-06-03 11:29:47.000000 picframe-2022.6.3/picframe/viewer_display.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 11:29:58.723932 picframe-2022.6.3/picframe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3408 2022-06-03 11:29:58.000000 picframe-2022.6.3/picframe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      619 2022-06-03 11:29:58.000000 picframe-2022.6.3/picframe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-03 11:29:58.000000 picframe-2022.6.3/picframe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       50 2022-06-03 11:29:58.000000 picframe-2022.6.3/picframe.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-03 11:29:58.000000 picframe-2022.6.3/picframe.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       77 2022-06-03 11:29:58.000000 picframe-2022.6.3/picframe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2022-06-03 11:29:58.000000 picframe-2022.6.3/picframe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      205 2022-06-03 11:29:58.723932 picframe-2022.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1591 2022-06-03 11:29:47.000000 picframe-2022.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-03 11:29:58.723932 picframe-2022.6.3/test/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-03 11:29:47.000000 picframe-2022.6.3/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4341 2022-06-03 11:29:47.000000 picframe-2022.6.3/test/test_get_image_meta.py
```

### Comparing `picframe-2022.4.19/LICENSE` & `picframe-2022.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `picframe-2022.4.19/PKG-INFO` & `picframe-2022.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: picframe
-Version: 2022.4.19
+Version: 2022.6.3
 Summary: Picture frame viewer powered by raspberry with homeassistant integration
 Home-page: https://github.com/helgeerbe/picframe
 Author: Paddy Gaunt, Jeff Godfrey, Helge Erbe
 Author-email: helge@erbehome.de
 License: MIT
 Keywords: picframe viewer raspberry raspi homeassistant hass
 Platform: UNKNOWN
```

### Comparing `picframe-2022.4.19/README.md` & `picframe-2022.6.3/README.md`

 * *Files identical despite different names*

### Comparing `picframe-2022.4.19/picframe/controller.py` & `picframe-2022.6.3/picframe/controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,29 +65,30 @@
         return self.__paused
 
     @paused.setter
     def paused(self, val:bool):
         self.__paused = val
         pic = self.__model.get_current_pics()[0] # only refresh left text
         self.__viewer.reset_name_tm(pic, val, side=0, pair=self.__model.get_current_pics()[1] is not None)
+        self.publish_state()
 
     def next(self):
         self.__next_tm = 0
         self.__viewer.reset_name_tm()
         self.__force_navigate = True
 
     def back(self):
         self.__model.set_next_file_to_previous_file()
         self.__next_tm = 0
         self.__viewer.reset_name_tm()
         self.__force_navigate = True
 
     def delete(self):
         self.__model.delete_file()
-        self.back() # TODO check needed to avoid skipping one as record has been deleted from model.__file_list
+        self.next() # TODO check needed to avoid skipping one as record has been deleted from model.__file_list
         self.__next_tm = 0
 
     def set_show_text(self, txt_key=None, val="ON"):
         if val is True: # allow to be called with boolean from httpserver
             val = "ON"
         self.__viewer.set_show_text(txt_key, val)
         for (side, pic) in enumerate(self.__model.get_current_pics()):
@@ -150,14 +151,15 @@
     def display_is_on(self):
         return self.__viewer.display_is_on
 
     @display_is_on.setter
     def display_is_on(self, on_off):
         self.paused = not on_off
         self.__viewer.display_is_on = on_off
+        self.publish_state()
 
     @property
     def clock_is_on(self):
         return self.__viewer.clock_is_on
 
     @clock_is_on.setter
     def clock_is_on(self, on_off):
@@ -168,14 +170,15 @@
         return self.__model.shuffle
 
     @shuffle.setter
     def shuffle(self, val:bool):
         self.__model.shuffle = val
         self.__model.force_reload()
         self.__next_tm = 0
+        self.publish_state()
 
     @property
     def fade_time(self):
         return self.__model.fade_time
 
     @fade_time.setter
     def fade_time(self, time):
@@ -198,15 +201,15 @@
     @property
     def brightness(self):
         return self.__viewer.get_brightness()
 
     @brightness.setter
     def brightness(self, val):
         self.__viewer.set_brightness(float(val))
-        self.__next_tm = 0
+        self.publish_state()
 
     @property
     def matting_images(self):
         return self.__viewer.get_matting_images()
 
     @matting_images.setter
     def matting_images(self, val):
```

### Comparing `picframe-2022.4.19/picframe/geo_reverse.py` & `picframe-2022.6.3/picframe/geo_reverse.py`

 * *Files identical despite different names*

### Comparing `picframe-2022.4.19/picframe/get_image_meta.py` & `picframe-2022.6.3/picframe/get_image_meta.py`

 * *Files identical despite different names*

### Comparing `picframe-2022.4.19/picframe/image_cache.py` & `picframe-2022.6.3/picframe/image_cache.py`

 * *Files identical despite different names*

### Comparing `picframe-2022.4.19/picframe/interface_http.py` & `picframe-2022.6.3/picframe/interface_http.py`

 * *Files identical despite different names*

### Comparing `picframe-2022.4.19/picframe/interface_mqtt.py` & `picframe-2022.6.3/picframe/interface_mqtt.py`

 * *Files 11% similar despite different names*

```diff
@@ -42,117 +42,120 @@
             self.__client.connect(server, port, 60)
             self.__client.will_set("homeassistant/switch/" + mqtt_config['device_id'] + "/available", "offline", qos=0, retain=True)
             self.__client.on_connect = self.on_connect
             self.__client.on_message = self.on_message
             self.__device_id = mqtt_config['device_id']
             self.__device_url = mqtt_config['device_url']
         except Exception as e:
-            self.__logger.info("MQTT not set up because of: {}".format(e))
+            self.__logger.error("MQTT not set up because of: {}".format(e))
+            raise
 
     def start(self):
         try:
             self.__controller.publish_state = self.publish_state
             self.__client.loop_start()
         except Exception as e:
-            self.__logger.info("MQTT not started because of: {}".format(e))
+            self.__logger.error("MQTT not started because of: {}".format(e))
+            raise
 
     def stop(self):
         try:
             self.__controller.publish_state = None
             self.__client.loop_stop()
         except Exception as e:
-            self.__logger.info("MQTT stopping failed because of: {}".format(e))
+            self.__logger.error("MQTT stopping failed because of: {}".format(e))
 
 
     def on_connect(self, client, userdata, flags, rc):
         if rc != 0:
             self.__logger.warning("Can't connect with mqtt broker. Reason = {0}".format(rc))
             return
         self.__logger.info('Connected with mqtt broker')
 
-        sensor_topic_head = "homeassistant/sensor/" + self.__device_id
-        number_topic_head = "homeassistant/number/" + self.__device_id
-        select_topic_head = "homeassistant/select/" + self.__device_id
-        switch_topic_head = "homeassistant/switch/" + self.__device_id
-
         # send last will and testament
-        available_topic = switch_topic_head + "/available"
+        available_topic = "homeassistant/switch/" + self.__device_id + "/available"
         client.publish(available_topic, "online", qos=0, retain=True)
 
         ## sensors
-        self.__setup_sensor(client, sensor_topic_head, "date_from", "mdi:calendar-arrow-left", available_topic, entity_category="config")
-        self.__setup_sensor(client, sensor_topic_head, "date_to", "mdi:calendar-arrow-right", available_topic, entity_category="config")
-        self.__setup_sensor(client, sensor_topic_head, "location_filter", "mdi:map-search", available_topic, entity_category="config")
-        self.__setup_sensor(client, sensor_topic_head, "tags_filter", "mdi:image-search", available_topic, entity_category="config")
-        self.__setup_sensor(client, sensor_topic_head, "image_counter", "mdi:camera-burst", available_topic, entity_category="diagnostic")
-        self.__setup_sensor(client, sensor_topic_head, "image", "mdi:file-image", available_topic, has_attributes=True, entity_category="diagnostic")
+        self.__setup_sensor(client, "date_from", "mdi:calendar-arrow-left", available_topic, entity_category="config")
+        self.__setup_sensor(client, "date_to", "mdi:calendar-arrow-right", available_topic, entity_category="config")
+        self.__setup_sensor(client, "location_filter", "mdi:map-search", available_topic, entity_category="config")
+        self.__setup_sensor(client, "tags_filter", "mdi:image-search", available_topic, entity_category="config")
+        self.__setup_sensor(client, "image_counter", "mdi:camera-burst", available_topic, entity_category="diagnostic")
+        self.__setup_sensor(client, "image", "mdi:file-image", available_topic, has_attributes=True, entity_category="diagnostic")
 
         ## numbers
-        self.__setup_number(client, number_topic_head, "brightness", 0.0, 1.0, 0.1, "mdi:brightness-6", available_topic)
-        self.__setup_number(client, number_topic_head, "time_delay", 1, 400, 1, "mdi:image-plus", available_topic)
-        self.__setup_number(client, number_topic_head, "fade_time", 1, 50, 1,"mdi:image-size-select-large", available_topic)
-        self.__setup_number(client, number_topic_head, "matting_images", 0.0, 1.0, 0.01, "mdi:image-frame", available_topic)
+        self.__setup_number(client, "brightness", 0.0, 1.0, 0.1, "mdi:brightness-6", available_topic)
+        self.__setup_number(client, "time_delay", 1, 400, 1, "mdi:image-plus", available_topic)
+        self.__setup_number(client, "fade_time", 1, 50, 1,"mdi:image-size-select-large", available_topic)
+        self.__setup_number(client, "matting_images", 0.0, 1.0, 0.01, "mdi:image-frame", available_topic)
 
         ## selects
         _, dir_list = self.__controller.get_directory_list()
         dir_list.sort()
-        self.__setup_select(client, select_topic_head, "directory", dir_list, "mdi:folder-multiple-image", available_topic, init=True)
+        self.__setup_select(client, "directory", dir_list, "mdi:folder-multiple-image", available_topic, init=True)
         command_topic = self.__device_id + "/directory"
         client.subscribe(command_topic, qos=0)
 
         ## switches
-        self.__setup_switch(client, switch_topic_head, "_text_refresh", "mdi:refresh", available_topic, entity_category="config")
-        self.__setup_switch(client, switch_topic_head, "_delete", "mdi:delete", available_topic)
-        self.__setup_switch(client, switch_topic_head, "_name_toggle", "mdi:subtitles", available_topic,
+        self.__setup_switch(client, "_text_refresh", "mdi:refresh", available_topic, entity_category="config")
+        self.__setup_switch(client, "_name_toggle", "mdi:subtitles", available_topic,
                             self.__controller.text_is_on("name"), entity_category="config")
-        self.__setup_switch(client, switch_topic_head, "_title_toggle", "mdi:subtitles", available_topic,
+        self.__setup_switch(client, "_title_toggle", "mdi:subtitles", available_topic,
                             self.__controller.text_is_on("title"), entity_category="config")
-        self.__setup_switch(client, switch_topic_head, "_caption_toggle", "mdi:subtitles", available_topic,
+        self.__setup_switch(client, "_caption_toggle", "mdi:subtitles", available_topic,
                             self.__controller.text_is_on("caption"), entity_category="config")
-        self.__setup_switch(client, switch_topic_head, "_date_toggle", "mdi:calendar-today", available_topic,
+        self.__setup_switch(client, "_date_toggle", "mdi:calendar-today", available_topic,
                             self.__controller.text_is_on("date"), entity_category="config")
-        self.__setup_switch(client, switch_topic_head, "_location_toggle", "mdi:crosshairs-gps", available_topic,
+        self.__setup_switch(client, "_location_toggle", "mdi:crosshairs-gps", available_topic,
                             self.__controller.text_is_on("location"), entity_category="config")
-        self.__setup_switch(client, switch_topic_head, "_directory_toggle", "mdi:folder", available_topic,
+        self.__setup_switch(client, "_directory_toggle", "mdi:folder", available_topic,
                             self.__controller.text_is_on("directory"), entity_category="config")
-        self.__setup_switch(client, switch_topic_head, "_text_off", "mdi:badge-account-horizontal-outline", available_topic, entity_category="config")
-        self.__setup_switch(client, switch_topic_head, "_display", "mdi:panorama", available_topic,
+        self.__setup_switch(client, "_text_off", "mdi:badge-account-horizontal-outline", available_topic, entity_category="config")
+        self.__setup_switch(client, "_display", "mdi:panorama", available_topic,
                             self.__controller.display_is_on)
-        self.__setup_switch(client, switch_topic_head, "_clock", "mdi:clock-outline", available_topic,
+        self.__setup_switch(client, "_clock", "mdi:clock-outline", available_topic,
                             self.__controller.clock_is_on, entity_category="config")
-        self.__setup_switch(client, switch_topic_head, "_shuffle", "mdi:shuffle-variant", available_topic,
+        self.__setup_switch(client, "_shuffle", "mdi:shuffle-variant", available_topic,
                             self.__controller.shuffle)
-        self.__setup_switch(client, switch_topic_head, "_paused", "mdi:pause", available_topic,
+        self.__setup_switch(client, "_paused", "mdi:pause", available_topic,
                             self.__controller.paused)
-        self.__setup_switch(client, switch_topic_head, "_back", "mdi:skip-previous", available_topic)
-        self.__setup_switch(client, switch_topic_head, "_next", "mdi:skip-next", available_topic)
+
+        # buttons
+        self.__setup_button(client, "_delete", "mdi:delete", available_topic)
+        self.__setup_button(client, "_back", "mdi:skip-previous", available_topic)
+        self.__setup_button(client, "_next", "mdi:skip-next", available_topic)
 
         client.subscribe(self.__device_id + "/purge_files", qos=0) # close down without killing!
         client.subscribe(self.__device_id + "/stop", qos=0) # close down without killing!
 
-    def __setup_sensor(self, client, sensor_topic_head, topic, icon, available_topic, has_attributes=False, entity_category=None):
+    def __setup_sensor(self, client, topic, icon, available_topic, has_attributes=False, entity_category=None):
+        sensor_topic_head = "homeassistant/sensor/" + self.__device_id
         config_topic = sensor_topic_head + "_" + topic + "/config"
         name = self.__device_id + "_" + topic
         dict = {"name": name,
                 "icon": icon,
-                "state_topic": sensor_topic_head + "/state",
                 "value_template": "{{ value_json." + topic + "}}",
                 "avty_t": available_topic,
                 "uniq_id": name,
                 "dev":{"ids":[self.__device_id]}}
         if has_attributes == True:
+            dict["state_topic"] = sensor_topic_head + "_" + topic + "/state"
             dict["json_attributes_topic"] = sensor_topic_head + "_" + topic + "/attributes"
+        else:
+            dict["state_topic"] = sensor_topic_head + "/state"
         if entity_category:
             dict["entity_category"] = entity_category
                                      
         config_payload = json.dumps(dict)
         client.publish(config_topic, config_payload, qos=0, retain=True)
         client.subscribe(self.__device_id + "/" + topic, qos=0)
 
-    def __setup_number(self, client, number_topic_head, topic, min, max, step, icon, available_topic):
+    def __setup_number(self, client, topic, min, max, step, icon, available_topic):
+        number_topic_head = "homeassistant/number/" + self.__device_id
         config_topic = number_topic_head + "_" + topic + "/config"
         command_topic = self.__device_id + "/" + topic
         state_topic = "homeassistant/sensor/" + self.__device_id + "/state"
         name = self.__device_id + "_" + topic
         config_payload = json.dumps({"name": name,
                                     "min": min,
                                     "max": max,
@@ -164,15 +167,16 @@
                                     "value_template": "{{ value_json." + topic + "}}",
                                     "avty_t": available_topic,
                                     "uniq_id": name,
                                     "dev":{"ids":[self.__device_id]}})
         client.publish(config_topic, config_payload, qos=0, retain=True)
         client.subscribe(command_topic, qos=0)
 
-    def __setup_select(self, client, select_topic_head, topic, options, icon, available_topic, init=False):
+    def __setup_select(self, client, topic, options, icon, available_topic, init=False):
+        select_topic_head = "homeassistant/select/" + self.__device_id
         config_topic = select_topic_head + "_" + topic + "/config"
         command_topic = self.__device_id + "/" + topic
         state_topic = "homeassistant/sensor/" + self.__device_id + "/state"
         name = self.__device_id + "_" + topic
 
         config_payload = json.dumps({"name": name,
                                     "entity_category": "config",
@@ -184,16 +188,17 @@
                                     "avty_t": available_topic,
                                     "uniq_id": name,
                                     "dev":{"ids":[self.__device_id]}})
         client.publish(config_topic, config_payload, qos=0, retain=True)
         if init:
             client.subscribe(command_topic, qos=0)
 
-    def __setup_switch(self, client, switch_topic_head, topic, icon,
+    def __setup_switch(self, client, topic, icon,
                        available_topic, is_on=False, entity_category=None):
+        switch_topic_head = "homeassistant/switch/" + self.__device_id
         config_topic = switch_topic_head + topic + "/config"
         command_topic = switch_topic_head + topic + "/set"
         state_topic = switch_topic_head + topic + "/state"
         dict = {"name": self.__device_id + topic,
                 "icon": icon,
                 "command_topic": command_topic,
                 "state_topic": state_topic,
@@ -211,17 +216,44 @@
             dict["entity_category"] = entity_category
         config_payload = json.dumps(dict)
 
         client.subscribe(command_topic , qos=0)
         client.publish(config_topic, config_payload, qos=0, retain=True)
         client.publish(state_topic, "ON" if is_on else "OFF", qos=0, retain=True)
 
+    def __setup_button(self, client, topic, icon,
+                       available_topic, entity_category=None):
+        button_topic_head = "homeassistant/button/" + self.__device_id
+        config_topic = button_topic_head + topic + "/config"
+        command_topic = button_topic_head + topic + "/set"
+        dict = {"name": self.__device_id + topic,
+                "icon": icon,
+                "command_topic": command_topic,
+                "payload_press": "ON",
+                "avty_t": available_topic,
+                "uniq_id": self.__device_id + topic,
+                "dev": {
+                "ids": [self.__device_id],
+                "name": self.__device_id,
+                "mdl": "PictureFrame",
+                "sw": __version__,
+                "mf": "pi3d PictureFrame project"}}
+        if self.__device_url :
+            dict["dev"]["cu"] = self.__device_url
+        if entity_category:
+            dict["entity_category"] = entity_category
+        config_payload = json.dumps(dict)
+
+        client.subscribe(command_topic , qos=0)
+        client.publish(config_topic, config_payload, qos=0, retain=True)
+
     def on_message(self, client, userdata, message):
         msg = message.payload.decode("utf-8")
         switch_topic_head = "homeassistant/switch/" + self.__device_id
+        button_topic_head = "homeassistant/button/" + self.__device_id
 
         ###### switches ######
         # display
         if message.topic == switch_topic_head + "_display/set":
             state_topic = switch_topic_head + "_display/state"
             if msg == "ON":
                 self.__controller.display_is_on = True
@@ -253,30 +285,24 @@
             if msg == "ON":
                 self.__controller.paused = True
                 client.publish(state_topic, "ON", retain=True)
             elif msg == "OFF":
                 self.__controller.paused = False
                 client.publish(state_topic, "OFF", retain=True)
         # back buttons
-        elif message.topic == switch_topic_head + "_back/set":
-            state_topic = switch_topic_head + "_back/state"
+        elif message.topic == button_topic_head + "_back/set":
             if msg == "ON":
-                client.publish(state_topic, "OFF", retain=True)
                 self.__controller.back()
         # next buttons
-        elif message.topic == switch_topic_head + "_next/set":
-            state_topic = switch_topic_head + "_next/state"
+        elif message.topic == button_topic_head + "_next/set":
             if msg == "ON":
-                client.publish(state_topic, "OFF", retain=True)
                 self.__controller.next()
         # delete
-        elif message.topic == switch_topic_head + "_delete/set":
-            state_topic = switch_topic_head + "_delete/state"
+        elif message.topic == button_topic_head + "_delete/set":
             if msg == "ON":
-                client.publish(state_topic, "OFF", retain=True)
                 self.__controller.delete()
         # title on
         elif message.topic == switch_topic_head + "_title_toggle/set":
             state_topic = switch_topic_head + "_title_toggle/state"
             if msg in ("ON", "OFF"):
                 self.__controller.set_show_text("title", msg)
                 client.publish(state_topic, msg, retain=True)
@@ -377,57 +403,78 @@
         elif message.topic == self.__device_id + "/purge_files":
             self.__controller.purge_files()
 
         # stop loops and end program
         elif message.topic == self.__device_id + "/stop":
             self.__controller.stop()
 
-    def publish_state(self, image, image_attr):
-        sensor_topic_head =  "homeassistant/sensor/" + self.__device_id
+    def publish_state(self, image=None, image_attr=None):
+        sensor_topic_head = "homeassistant/sensor/" + self.__device_id
         switch_topic_head = "homeassistant/switch/" + self.__device_id
-        select_topic_head = "homeassistant/select/" + self.__device_id
-        sensor_state_topic = sensor_topic_head + "/state"
+        available_topic = switch_topic_head + "/available"
 
         sensor_state_payload = {}
+        image_state_payload = {}
+
+        ## image
+        # image attributes
+        if image_attr is not None:
+            attributes_topic = sensor_topic_head + "_image/attributes"
+            self.__logger.debug("Send image attributes: %s", image_attr)
+            self.__client.publish(attributes_topic, json.dumps(image_attr), qos=0, retain=False)
+        # image sensor
+        if image is not None:
+            _, tail = os.path.split(image)
+            image_state_payload["image"] = tail
+            image_state_topic = sensor_topic_head + "_image/state"
+            self.__logger.info("Send image state: %s", image_state_payload)
+            self.__client.publish(image_state_topic, json.dumps(image_state_payload), qos=0, retain=False)
 
         ## sensor
         # directory sensor
         actual_dir, dir_list = self.__controller.get_directory_list()
         sensor_state_payload["directory"] = actual_dir
         # image counter sensor
         sensor_state_payload["image_counter"] = str(self.__controller.get_number_of_files())
-        # image sensor
-        _, tail = os.path.split(image)
-        sensor_state_payload["image"] = tail
         # date_from
         sensor_state_payload["date_from"] = int(self.__controller.date_from)
         # date_to
         sensor_state_payload["date_to"] = int(self.__controller.date_to)
         # location_filter
         sensor_state_payload["location_filter"] = self.__controller.location_filter
         # tags_filter
         sensor_state_payload["tags_filter"] = self.__controller.tags_filter
-
         ## number state
         # time_delay
         sensor_state_payload["time_delay"] = self.__controller.time_delay
         # fade_time
         sensor_state_payload["fade_time"] = self.__controller.fade_time
         # brightness
         sensor_state_payload["brightness"] = self.__controller.brightness
         # matting_images
         sensor_state_payload["matting_images"] = self.__controller.matting_images
 
-        # send last will and testament
-        available_topic = switch_topic_head + "/available"
-        self.__client.publish(available_topic, "online", qos=0, retain=True)
-
         #pulish sensors
-        attributes_topic = sensor_topic_head + "_image/attributes"
-        self.__logger.debug("Send image attributes: %s", image_attr)
-        self.__client.publish(attributes_topic, json.dumps(image_attr), qos=0, retain=False)
         dir_list.sort()
-        self.__setup_select(self.__client, select_topic_head, "directory", dir_list, "mdi:folder-multiple-image", available_topic, init=False)
+        self.__setup_select(self.__client, "directory", dir_list, "mdi:folder-multiple-image", available_topic, init=False)
 
         self.__logger.info("Send sensor state: %s", sensor_state_payload)
+        sensor_state_topic = sensor_topic_head + "/state"
         self.__client.publish(sensor_state_topic, json.dumps(sensor_state_payload), qos=0, retain=False)
 
+        # publish state of switches
+        # pause
+        state_topic = switch_topic_head + "_paused/state"
+        payload = "ON" if self.__controller.paused else "OFF"
+        self.__client.publish(state_topic, payload, retain=True)
+        # shuffle
+        state_topic = switch_topic_head + "_shuffle/state"
+        payload = "ON" if self.__controller.shuffle else "OFF"
+        self.__client.publish(state_topic, payload, retain=True)
+        # display
+        state_topic = switch_topic_head + "_display/state"
+        payload = "ON" if self.__controller.display_is_on else "OFF"
+        self.__client.publish(state_topic, payload, retain=True)
+
+        # send last will and testament
+        self.__client.publish(available_topic, "online", qos=0, retain=True)
+
```

### Comparing `picframe-2022.4.19/picframe/interface_peripherals.py` & `picframe-2022.6.3/picframe/interface_peripherals.py`

 * *Files identical despite different names*

### Comparing `picframe-2022.4.19/picframe/mat_image.py` & `picframe-2022.6.3/picframe/mat_image.py`

 * *Files identical despite different names*

### Comparing `picframe-2022.4.19/picframe/model.py` & `picframe-2022.6.3/picframe/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
         'shader': '~/picframe_data/data/shaders/blend_new',
         'show_text_fm': '%b %d, %Y',
         'show_text_tm': 20.0,
         'show_text_sz': 40,
         'show_text': "name location",
         'text_justify': 'L',
         'text_bkg_hgt': 0.25,
+        'text_opacity': 1.0,
         'fit': False,
         #'auto_resize': True,
         'kenburns': False,
         'display_x': 0,
         'display_y': 0,
         'display_w': None,
         'display_h': None,
@@ -44,17 +45,19 @@
         'inner_mat_use_texture': False,
         'outer_mat_use_texture': True,
         'mat_resource_folder': '~/picframe_data/data/mat',
         'show_clock': False,
         'clock_justify': "R",
         'clock_text_sz': 120,
         'clock_format': "%I:%M",
+        'clock_opacity': 1.0,
         #'codepoints': "1234567890AÄÀÆÅÃBCÇDÈÉÊEËFGHIÏÍJKLMNÑOÓÖÔŌØPQRSTUÚÙÜVWXYZaáàãæåäbcçdeéèêëfghiíïjklmnñoóôōøöpqrsßtuúüvwxyz., _-+*()&/`´'•" # limit to 121 ie 11x11 grid_size
         'menu_text_sz': 40,
         'menu_autohide_tm': 10.0,
+        'geo_suppress_list': [],
     },
     'model': {
 
         'pic_dir': '~/Pictures',
         'no_files_img': '~/picframe_data/data/no_pictures.jpg',
         'follow_links': False,
         'subdirectory': '',
```

### Comparing `picframe-2022.4.19/picframe/start.py` & `picframe-2022.6.3/picframe/start.py`

 * *Files 3% similar despite different names*

```diff
@@ -134,16 +134,22 @@
     v = viewer_display.ViewerDisplay(m.get_viewer_config())
     c = controller.Controller(m, v)
     c.start()
 
     mqtt_config = m.get_mqtt_config()
     if mqtt_config['use_mqtt']:
         from picframe import interface_mqtt
-        mqtt = interface_mqtt.InterfaceMQTT(c, mqtt_config)
-        mqtt.start()
+        try:
+            mqtt = interface_mqtt.InterfaceMQTT(c, mqtt_config)
+            mqtt.start()
+        except:
+            logger.error("Can't initialize mqtt. Stopping picframe")
+            sys.exit(1) 
+
+
 
     http_config = m.get_http_config()
     model_config = m.get_model_config()
     if http_config['use_http']:
         server = interface_http.InterfaceHttp(c, http_config['path'], model_config['pic_dir'], model_config['no_files_img'], http_config['port'])
         if http_config['use_ssl']:
             server.socket = ssl.wrap_socket(
```

### Comparing `picframe-2022.4.19/picframe/viewer_display.py` & `picframe-2022.6.3/picframe/viewer_display.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,15 +55,17 @@
         self.__shader = os.path.expanduser(config['shader'])
         self.__show_text_tm = float(config['show_text_tm'])
         self.__show_text_fm = config['show_text_fm']
         self.__show_text_sz = config['show_text_sz']
         self.__show_text = parse_show_text(config['show_text'])
         self.__text_justify = config['text_justify'].upper()
         self.__text_bkg_hgt = config['text_bkg_hgt'] if 0 <= config['text_bkg_hgt'] <= 1 else 0.25
+        self.__text_opacity = config['text_opacity']
         self.__fit = config['fit']
+        self.__geo_suppress_list = config['geo_suppress_list']
         #self.__auto_resize = config['auto_resize']
         self.__kenburns = config['kenburns']
         if self.__kenburns:
             self.__kb_up = True
             self.__fit = False
             self.__blur_edges = False
         if self.__blur_zoom < 1.0:
@@ -92,14 +94,15 @@
         self.__matter = None
         self.__prev_clock_time = None
         self.__clock_overlay = None
         self.__show_clock = config['show_clock']
         self.__clock_justify = config['clock_justify']
         self.__clock_text_sz = config['clock_text_sz']
         self.__clock_format = config['clock_format']
+        self.__clock_opacity = config['clock_opacity']
         ImageFile.LOAD_TRUNCATED_IMAGES = True # occasional damaged file hangs app
 
     @property
     def display_is_on(self):
         try: # vcgencmd only applies to raspberry pi
             state = str(subprocess.check_output(["vcgencmd", "display_power"]))
             if (state.find("display_power=1") != -1):
@@ -354,29 +357,39 @@
                 info_strings.append(pic.caption)
             if (self.__show_text & 4) == 4: # name
                 info_strings.append(os.path.basename(pic.fname))
             if (self.__show_text & 8) == 8 and pic.exif_datetime > 0: # date
                 fdt = time.strftime(self.__show_text_fm, time.localtime(pic.exif_datetime))
                 info_strings.append(fdt)
             if (self.__show_text & 16) == 16 and pic.location is not None: # location
-                info_strings.append(pic.location) #TODO need to sanitize and check longer than 0 for real
+                location = pic.location
+                # search for and remove substrings from the location text
+                if self.__geo_suppress_list is not None:
+                    for part in self.__geo_suppress_list:
+                        location = location.replace(part, "")
+                    # remove any redundant concatination strings once the substrings have been removed
+                    location = location.replace(" ,", "")
+                    # remove any trailing commas or spaces from the location
+                    location = location.strip(", ")
+                info_strings.append(location) #TODO need to sanitize and check longer than 0 for real
             if (self.__show_text & 32) == 32: # folder
                 info_strings.append(os.path.basename(os.path.dirname(pic.fname)))
             if paused:
                 info_strings.append("PAUSED")
         final_string = " • ".join(info_strings)
 
         block = None
         if len(final_string) > 0:
             if side == 0 and not pair:
                 c_rng = self.__display.width - 100 # range for x loc from L to R justified
             else:
                 c_rng = self.__display.width * 0.5 - 100 # range for x loc from L to R justified
             block = pi3d.FixedString(self.__font_file, final_string, shadow_radius=3, font_size=self.__show_text_sz,
-                                    shader=self.__flat_shader, justify=self.__text_justify, width=c_rng)
+                                    shader=self.__flat_shader, justify=self.__text_justify, width=c_rng,
+                                    color=(255, 255, 255, int(255 * float(self.__text_opacity))))
             adj_x = (c_rng - block.sprite.width) // 2 # half amount of space outside sprite
             if self.__text_justify == "L":
                 adj_x *= -1
             elif self.__text_justify == "C":
                 adj_x = 0
             if side == 0 and not pair: # i.e. full width
                 x = adj_x
@@ -394,15 +407,16 @@
 
         # --- Only rebuild the FixedString containing the time valud if the time string has changed.
         #     With the default H:M display, this will only rebuild once each minute. Note however,
         #     time strings containing a "seconds" component will rebuild once per second.
         if current_time != self.__prev_clock_time:
             width = self.__display.width - 50
             self.__clock_overlay = pi3d.FixedString(self.__font_file, current_time, font_size=self.__clock_text_sz,
-                shader=self.__flat_shader, width=width, shadow_radius=3)
+                shader=self.__flat_shader, width=width, shadow_radius=3,
+                color=(255, 255, 255, int(255 * float(self.__clock_opacity))))
             x = (width - self.__clock_overlay.sprite.width) // 2
             if self.__clock_justify == "L":
                 x *= -1
             elif self.__clock_justify == "C":
                 x = 0
             y = (self.__display.height - self.__clock_text_sz - 20) // 2
             self.__clock_overlay.sprite.position(x, y, 0.1)
```

### Comparing `picframe-2022.4.19/picframe.egg-info/PKG-INFO` & `picframe-2022.6.3/picframe.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: picframe
-Version: 2022.4.19
+Version: 2022.6.3
 Summary: Picture frame viewer powered by raspberry with homeassistant integration
 Home-page: https://github.com/helgeerbe/picframe
 Author: Paddy Gaunt, Jeff Godfrey, Helge Erbe
 Author-email: helge@erbehome.de
 License: MIT
 Keywords: picframe viewer raspberry raspi homeassistant hass
 Platform: UNKNOWN
```

### Comparing `picframe-2022.4.19/picframe.egg-info/SOURCES.txt` & `picframe-2022.6.3/picframe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `picframe-2022.4.19/setup.py` & `picframe-2022.6.3/setup.py`

 * *Files identical despite different names*

### Comparing `picframe-2022.4.19/test/test_get_image_meta.py` & `picframe-2022.6.3/test/test_get_image_meta.py`

 * *Files identical despite different names*

