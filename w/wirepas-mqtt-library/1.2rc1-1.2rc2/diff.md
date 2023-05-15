# Comparing `tmp/wirepas_mqtt_library-1.2rc1.tar.gz` & `tmp/wirepas_mqtt_library-1.2rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wirepas_mqtt_library-1.2rc1.tar", last modified: Thu Feb  2 15:28:28 2023, max compression
+gzip compressed data, was "wirepas_mqtt_library-1.2rc2.tar", last modified: Fri Mar 31 08:41:21 2023, max compression
```

## Comparing `wirepas_mqtt_library-1.2rc1.tar` & `wirepas_mqtt_library-1.2rc2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 15:28:28.174111 wirepas_mqtt_library-1.2rc1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-02-02 15:28:20.000000 wirepas_mqtt_library-1.2rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6590 2023-02-02 15:28:28.174111 wirepas_mqtt_library-1.2rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-02-02 15:28:20.000000 wirepas_mqtt_library-1.2rc1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-02 15:28:28.174111 wirepas_mqtt_library-1.2rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-02-02 15:28:20.000000 wirepas_mqtt_library-1.2rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 15:28:28.170111 wirepas_mqtt_library-1.2rc1/wirepas_mqtt_library/
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-02-02 15:28:27.000000 wirepas_mqtt_library-1.2rc1/wirepas_mqtt_library/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-02-02 15:28:20.000000 wirepas_mqtt_library-1.2rc1/wirepas_mqtt_library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-02-02 15:28:20.000000 wirepas_mqtt_library-1.2rc1/wirepas_mqtt_library/topic_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    40003 2023-02-02 15:28:20.000000 wirepas_mqtt_library-1.2rc1/wirepas_mqtt_library/wirepas_network_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    14847 2023-02-02 15:28:20.000000 wirepas_mqtt_library-1.2rc1/wirepas_mqtt_library/wirepas_otap_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    12433 2023-02-02 15:28:20.000000 wirepas_mqtt_library-1.2rc1/wirepas_mqtt_library/wirepas_tlv_app_config_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 15:28:28.174111 wirepas_mqtt_library-1.2rc1/wirepas_mqtt_library.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6590 2023-02-02 15:28:27.000000 wirepas_mqtt_library-1.2rc1/wirepas_mqtt_library.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-02-02 15:28:28.000000 wirepas_mqtt_library-1.2rc1/wirepas_mqtt_library.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-02 15:28:27.000000 wirepas_mqtt_library-1.2rc1/wirepas_mqtt_library.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-02-02 15:28:27.000000 wirepas_mqtt_library-1.2rc1/wirepas_mqtt_library.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-02 15:28:27.000000 wirepas_mqtt_library-1.2rc1/wirepas_mqtt_library.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 08:41:21.351408 wirepas_mqtt_library-1.2rc2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-31 08:41:16.000000 wirepas_mqtt_library-1.2rc2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6590 2023-03-31 08:41:21.351408 wirepas_mqtt_library-1.2rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-03-31 08:41:16.000000 wirepas_mqtt_library-1.2rc2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 08:41:21.355408 wirepas_mqtt_library-1.2rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-03-31 08:41:16.000000 wirepas_mqtt_library-1.2rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 08:41:21.351408 wirepas_mqtt_library-1.2rc2/wirepas_mqtt_library/
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-03-31 08:41:20.000000 wirepas_mqtt_library-1.2rc2/wirepas_mqtt_library/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-03-31 08:41:16.000000 wirepas_mqtt_library-1.2rc2/wirepas_mqtt_library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-03-31 08:41:16.000000 wirepas_mqtt_library-1.2rc2/wirepas_mqtt_library/topic_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44648 2023-03-31 08:41:16.000000 wirepas_mqtt_library-1.2rc2/wirepas_mqtt_library/wirepas_network_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16088 2023-03-31 08:41:16.000000 wirepas_mqtt_library-1.2rc2/wirepas_mqtt_library/wirepas_otap_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12433 2023-03-31 08:41:16.000000 wirepas_mqtt_library-1.2rc2/wirepas_mqtt_library/wirepas_tlv_app_config_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 08:41:21.351408 wirepas_mqtt_library-1.2rc2/wirepas_mqtt_library.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6590 2023-03-31 08:41:21.000000 wirepas_mqtt_library-1.2rc2/wirepas_mqtt_library.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-03-31 08:41:21.000000 wirepas_mqtt_library-1.2rc2/wirepas_mqtt_library.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 08:41:21.000000 wirepas_mqtt_library-1.2rc2/wirepas_mqtt_library.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-31 08:41:21.000000 wirepas_mqtt_library-1.2rc2/wirepas_mqtt_library.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-31 08:41:21.000000 wirepas_mqtt_library-1.2rc2/wirepas_mqtt_library.egg-info/top_level.txt
```

### Comparing `wirepas_mqtt_library-1.2rc1/LICENSE` & `wirepas_mqtt_library-1.2rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `wirepas_mqtt_library-1.2rc1/PKG-INFO` & `wirepas_mqtt_library-1.2rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wirepas_mqtt_library
-Version: 1.2rc1
+Version: 1.2rc2
 Summary: Library to interact with a Wirepas Network through MQTT/Protobuf API
 Home-page: https://github.com/wirepas/wirepas-mqtt-library
 Author: Wirepas Ltd
 Author-email: opensource@wirepas.com
 License: Apache-2
 Description: Wirepas MQTT Library
         ====================
```

### Comparing `wirepas_mqtt_library-1.2rc1/README.rst` & `wirepas_mqtt_library-1.2rc2/README.rst`

 * *Files identical despite different names*

### Comparing `wirepas_mqtt_library-1.2rc1/setup.py` & `wirepas_mqtt_library-1.2rc2/setup.py`

 * *Files identical despite different names*

### Comparing `wirepas_mqtt_library-1.2rc1/wirepas_mqtt_library/__about__.py` & `wirepas_mqtt_library-1.2rc2/wirepas_mqtt_library/__about__.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,8 +17,8 @@
 __description__ = "Library to interact with a Wirepas Network through MQTT/Protobuf API"
 __keywords__ = "wirepas connectivity iot mesh gateway backend"
 __license__ = "Apache-2"
 __pkg_name__ = "wirepas_mqtt_library"
 __title__ = "Wirepas Library For Network access"
 __url__ = "https://github.com/wirepas/wirepas-mqtt-library"
 # __version__ will be updated by Github action
-__version__ = "1.2rc1"
+__version__ = "1.2rc2"
```

### Comparing `wirepas_mqtt_library-1.2rc1/wirepas_mqtt_library/topic_helper.py` & `wirepas_mqtt_library-1.2rc2/wirepas_mqtt_library/topic_helper.py`

 * *Files identical despite different names*

### Comparing `wirepas_mqtt_library-1.2rc1/wirepas_mqtt_library/wirepas_network_interface.py` & `wirepas_mqtt_library-1.2rc2/wirepas_mqtt_library/wirepas_network_interface.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     format.
 
     Most of the calls can be called in a blocking mode (ie, blocking until gateway response is received)
     or in an asynchronous way by specifying a callback to receive the response.
 
     """
     # Timeout in s to wait for connection
-    _TIMEOUT_GW_CONNECTION_S = 4
+    _TIMEOUT_NETWORK_CONNECTION_S = 4
 
     # Timeout in s to wait for status message after subscription to
     # topic and connection is established
     _TIMEOUT_GW_STATUS_S = 2
 
     # Timeout in s to receive config from gw
     _TIMEOUT_GW_CONFIG_S = 2
@@ -126,15 +126,16 @@
         # for the full config
         self._initial_discovery_done = False
 
         self._gateways = {}
         # Dictionary to store request id, associated cb
         self._ongoing_requests = {}
 
-        self._data_filters = {}
+        self._data_uplink_filters = {}
+        self._data_downlink_filters = {}
         self._on_config_changed_cb = None
 
         # Create rx queue and start dispatch thread
         self._task_queue = _TaskQueue(num_worker_thread)
 
         # Save user option parameters
         self._strict_mode = strict_mode
@@ -181,19 +182,27 @@
         # Register for Data topic
         all_data_topic = TopicGenerator.make_received_data_topic()
         self._mqtt_client.subscribe(all_data_topic, qos=1)
         self._mqtt_client.message_callback_add(all_data_topic,
                                                self._on_data_received)
 
         # Register for all responses
+        # TODO must be part of TopicGenerator
         all_responses_topic = "gw-response/#"
         self._mqtt_client.subscribe(all_responses_topic, 1)
         self._mqtt_client.message_callback_add(all_responses_topic,
                                                self._on_response_received)
 
+
+        # Register for all sent data
+        all_send_data_topic = TopicGenerator.make_send_data_request_topic()
+        self._mqtt_client.subscribe(all_send_data_topic, 1)
+        self._mqtt_client.message_callback_add(all_send_data_topic,
+                                               self._on_downlink_data_received)
+
         self._connection_time = time()
 
         logging.info("..Connected to MQTT")
         self._connected.set()
         if self._connection_cb is not None:
             self._task_queue.add_task(self._connection_cb, True, self.ConnectionErrorCode.OK)
 
@@ -214,21 +223,14 @@
             return
 
         try:
             status = wmm.StatusEvent.from_payload(message.payload)
 
             if status.state == wmm.GatewayState.ONLINE:
                 self._gateways[status.gw_id] = self._Gateway(status.gw_id, True)
-                request = wmm.GetConfigsRequest()
-                self._publish(TopicGenerator.make_get_configs_request_topic(status.gw_id),
-                              request.payload,
-                              1)
-
-                # Call update gateway config when receiving it
-                self._wait_for_response(self._update_gateway_configs, request.req_id)
             else:
                 # Gateway is offline, remove config (Override any old config)
                 self._gateways[status.gw_id] = self._Gateway(status.gw_id, False)
                 # Config has changed, notify any subscriber
                 if self._on_config_changed_cb is not None:
                     self._task_queue.add_task(self._on_config_changed_cb)
 
@@ -268,43 +270,63 @@
     def _on_data_received(self, client, userdata, message):
         try:
             data = wmm.ReceivedDataEvent.from_payload(message.payload)
             if data.network_address is None:
                 # Network id is from topic
                 _, _, network_address, _, _ = TopicParser.parse_received_data_topic(message.topic)
                 data.network_address = network_address
-            self._task_queue.add_task(self._dispatch_data, data)
+            self._task_queue.add_task(self._dispatch_uplink_data, data)
         except wmm.GatewayAPIParsingException as e:
             logging.error(str(e))
 
-    def _dispatch_data(self, data):
-        for f in self._data_filters.values():
+    def _dispatch_uplink_data(self, data):
+        for f in self._data_uplink_filters.values():
             f.filter_and_dispatch(data)
 
     def _publish(self, topic, payload, qos=1, retain=False):
         try:
             self._mqtt_client.publish(topic,
                                       payload,
                                       qos=qos,
                                       retain=retain)
         except Exception as e:
             logging.error(str(e))
 
     def _call_cb(self, response, *args):
         try:
-            cb, param = self._ongoing_requests[response.req_id]
+            for cb, param in self._ongoing_requests[response.req_id]:
             # Add caller param after response error code and add any additional param at the end
-            cb(response.res, param, *args)
-            # Cb called, remove key
+                cb(response.res, param, *args)
+                # Cb called, remove key
+            
             del self._ongoing_requests[response.req_id]
         except KeyError:
             # No cb set, just pass (could be timeout that expired)
             logging.debug("Response but no associated cb: %s" % response.req_id)
             pass
 
+    def _on_downlink_data_received(self, client, userdata, message):
+        try:
+            data = wmm.SendDataRequest.from_payload(message.payload)
+
+            # retrieve missing info from message by reading topic
+            gw_id, sink_id = TopicParser.parse_send_data_topic(message.topic)
+            data.__dict__.update({'gw_id': gw_id})
+            data.__dict__.update({'sink_id': sink_id})
+
+            logging.debug("Received message with id: %s", data.req_id)
+            self._wait_for_response(self._dispatch_downlink_data, data.req_id, param=data)
+           
+        except wmm.GatewayAPIParsingException as e:
+            logging.error(str(e))
+
+    def _dispatch_downlink_data(self, response, data):
+        for f in self._data_downlink_filters.values():
+            f.filter_and_dispatch(data, response)
+
     def _on_response_received(self, client, userdata, message):
         # Topic are as followed: gw-response/cmd/...
         cmd = message.topic.split("/")[1]
         logging.debug("Response for: %s" % cmd)
         handler = self._call_cb
         additional_params = None
         try:
@@ -344,48 +366,75 @@
                 self._task_queue.add_task(handler, response)
             else:
                 self._task_queue.add_task(handler, response, additional_params)
 
         except wmm.GatewayAPIParsingException as e:
             logging.error(str(e))
 
+    def _wait_for_connection(fn):
+        # Decorator to handle waiting for connection to mqtt
+        def wrapper(*args, **kwargs):
+            args[0]._connected.wait(args[0]._TIMEOUT_NETWORK_CONNECTION_S)
+            if not args[0]._connected.is_set():
+                raise TimeoutError("Cannot connect to broker")
+
+            # Check if enough time was elapsed since we connect to receive all status
+            delay = (args[0]._connection_time + args[0]._TIMEOUT_GW_STATUS_S) - time()
+            if delay > 0:
+                sleep(delay)
+
+            return fn(*args, **kwargs)
+        wrapper.__doc__ = fn.__doc__
+        return wrapper
+
+    def _ask_gateway_config(self, gw_id):
+        request = wmm.GetConfigsRequest()
+        self._publish(TopicGenerator.make_get_configs_request_topic(gw_id),
+                        request.payload,
+                        1)
+
+        # Call update gateway config when receiving it
+        self._wait_for_response(self._update_gateway_configs, request.req_id)
+
     def _wait_for_configs(fn):
         # Decorator to handle waiting for enough time for the setup
         # of the network interface
         def wrapper(*args, **kwargs):
             # args[0] is self
-            if not args[0]._initial_discovery_done:
-                # Wait for connection
-                args[0]._connected.wait(args[0]._TIMEOUT_GW_CONNECTION_S)
-                if not args[0]._connected.is_set():
-                    raise TimeoutError("Cannot connect to broker")
-
-                # Check if enough time was elapsed since we connect to receive all status
-                delay = (args[0]._connection_time + args[0]._TIMEOUT_GW_STATUS_S) - time()
-                if delay > 0:
-                    sleep(delay)
-
-                # Check if we are still waiting for configs
-                for gw in args[0]._gateways.copy().values():
-                    if gw.online:
-                        gw.config_received_event.wait(args[0]._TIMEOUT_GW_CONFIG_S)
-                        if not gw.config_received_event.is_set():
-                            logging.error("Config timeout for gw %s" % gw.id)
-                            logging.error("Is the gateway really online? If not, its status can be cleared by "
-                                          "calling clear_gateway_status(\"%s\")", gw.id)
-                            # Mark the config as received to avoid waiting for it next time
-                            # It may still come later
-                            gw.config_received_event.set()
-                            if args[0]._strict_mode:
-                                logging.error("This Timeout will generate an exception but you can"
-                                              "avoid it by starting WirepasNetworkInteface with strict_mode=False")
-                                raise TimeoutError("Cannot get config from online GW %s" % gw.id)
 
-                # Discovery done, no need to do it again
-                args[0]._initial_discovery_done = True
+            gateways_subset = None
+            # Check for missing gateway config
+            if ("gateway" in kwargs):
+                gateways_subset = kwargs['gateway']
+
+            for gw in args[0]._gateways.copy().values():
+                if gateways_subset is not None and gw.id not in gateways_subset:
+                    # Not interested by this gateway, so no need for the config
+                    continue
+
+                if gw.online:
+                    if gw.config_received_event.is_set():
+                        # We have already received the config
+                        continue
+
+                    # Time to ask the gateway config
+                    args[0]._ask_gateway_config(gw.id)
+
+                    gw.config_received_event.wait(args[0]._TIMEOUT_GW_CONFIG_S)
+                    if not gw.config_received_event.is_set():
+                        logging.error("Config timeout for gw %s" % gw.id)
+                        logging.error("Is the gateway really online? If not, its status can be cleared by "
+                                        "calling clear_gateway_status(\"%s\")", gw.id)
+                        # Mark the config as received to avoid waiting for it next time
+                        # It may still come later
+                        gw.config_received_event.set()
+                        if args[0]._strict_mode:
+                            logging.error("This Timeout will generate an exception but you can "
+                                            "avoid it by starting WirepasNetworkInteface with strict_mode=False")
+                            raise TimeoutError("Cannot get config from online GW %s", gw.id)
 
             return fn(*args, **kwargs)
         wrapper.__doc__ = fn.__doc__
         return wrapper
 
     def close(self):
         """Explicitly close this network interface as well as the worker threads
@@ -403,14 +452,15 @@
         .. warning:: the instance of WNI must not be used anymore after this call. Any other method call requiring the broker
             connection after this one will end up in TimeoutError exception
         """
         self._mqtt_client.disconnect()
         self._task_queue.terminate()
 
 
+    @_wait_for_connection
     @_wait_for_configs
     def get_sinks(self, network_address=None, gateway=None):
         """
         get_sinks(self, network_address=None, gateway=None)
         Get list of current sink connected to this broker
 
         :param network_address: If specified, only sinks with matching network addresses are returned
@@ -470,15 +520,15 @@
                         # Network address is unset so doesn't match
                         continue
 
                 sinks.append((gw.id, sink['sink_id'], sink))
 
         return sinks
 
-    @_wait_for_configs
+    @_wait_for_connection
     def get_gateways(self, only_online=True):
         """
         get_gateways(self, only_online=True)
         Get list of current gateways connected to this broker
 
         :param only_online: if True (default) only online gateways are returned
         :return: List of gateway name
@@ -487,14 +537,15 @@
         if only_online:
             gateways = list(filter(lambda x: self._gateways[x].online, self._gateways))
         else:
             gateways = self._gateways.keys()
 
         return gateways
 
+    @_wait_for_connection
     def clear_gateway_status(self, gw_id):
         """
         Clear a gateway status
 
         :param gw_id: Id of gateway the sink is attached
         :type gw_id: str
 
@@ -503,19 +554,24 @@
             - An offline gateway that will never be back online (removed from network)
             - A sticky gateway online status that is not here anymore (bug from gateway)
             - A malformed gateway status (bug from gateway)
         """
         topic = TopicGenerator.make_status_topic(gw_id)
         self._publish(topic, None, qos=1, retain=True)
 
+    def _add_to_ongoing_request(self, req_id, cb, param=None):
+        try: 
+            self._ongoing_requests[req_id].append((cb, param))
+        except KeyError:
+            self._ongoing_requests[req_id]= [(cb, param)]
 
     def _wait_for_response(self, cb, req_id, timeout=2, param=None):
         if cb is not None:
             # Unblocking call, cb will be called later
-            self._ongoing_requests[req_id] = cb, param
+            self._add_to_ongoing_request(req_id, cb, param)
             return None
 
         # No cb specified so blocking call
         res = None
         response_event = Event()
 
         def unlock(response, param, *args):
@@ -523,23 +579,25 @@
 
             if args.__len__() == 0:
                 res = response
             else:
                 res = response, *args
             response_event.set()
 
-        self._ongoing_requests[req_id] = unlock, None
+        self._add_to_ongoing_request(req_id, unlock)
+
         if not response_event.wait(timeout):
             # Timeout
             del self._ongoing_requests[req_id]
             raise TimeoutError("Cannot get response for request")
 
         return res
 
-    def send_message(self, gw_id, sink_id, dest, src_ep, dst_ep, payload, qos=0, csma_ca_only=False, cb=None, param=None):
+    @_wait_for_connection
+    def send_message(self, gw_id, sink_id, dest, src_ep, dst_ep, payload, qos=0, csma_ca_only=False, hop_limit=0, cb=None, param=None):
         """
         send_message(self, gw_id, sink_id, dest, src_ep, dst_ep, payload, qos=0, csma_ca_only=False, cb=None, param=None)
         Send a message to wirepas network from a given sink
 
         :param gw_id: Id of gateway the sink is attached
         :type gw_id: str
         :param sink_id: Id of sink
@@ -548,14 +606,16 @@
         :param src_ep: source endpoint
         :param dst_ep: destination endpoint
         :param qos:  Quality of service to use (0 or 1) (default is 0)
         :param payload: payload to send
         :type payload: bytearray
         :param csma_ca_only: Is packet only for csma-ca nodes
         :type csma_ca_only: bool
+        :param hop_limit(int): maximum number of hops this message can do to reach its destination (<16)
+        :type hop_limit: int
         :param cb: If set, callback to be asynchronously called when gateway answer.
             If None, call is blocking.
 
             .. note:: Expected signature:
 
                 on_message_sent_cb(gw_error_code, param)
 
@@ -568,23 +628,24 @@
         :param param: Optional parameter that will be passed to callback
         :type param: object
         :return: None if cb is set or error code from gateway is synchronous call
         :rtype: :obj:`~wirepas_mesh_messaging.gateway_result_code.GatewayResultCode`
 
         :raises TimeoutError: Raised if cb is None and response is not received within 2 sec
         """
-        request = wmm.SendDataRequest(dest, src_ep, dst_ep, qos, payload, is_unack_csma_ca=csma_ca_only)
+        request = wmm.SendDataRequest(dest, src_ep, dst_ep, qos, payload, is_unack_csma_ca=csma_ca_only, hop_limit=hop_limit)
 
         self._publish(TopicGenerator.make_send_data_request_topic(gw_id, sink_id),
                       request.payload,
                       1)
 
         return self._wait_for_response(cb, request.req_id, param=param)
 
-    def upload_scratchpad(self, gw_id, sink_id, seq, scratchpad=None, cb=None, param=None):
+    @_wait_for_connection
+    def upload_scratchpad(self, gw_id, sink_id, seq, scratchpad=None, cb=None, param=None, timeout=60):
         """
         upload_scratchpad(self, gw_id, sink_id, seq, scratchpad=None, cb=None, param=None)
         Upload a scratchpad on a given sink
 
         :param gw_id: Id of gateway the sink is attached
         :type gw_id: str
         :param sink_id: Id of sink
@@ -600,32 +661,34 @@
             .. code-block:: python
 
                  on_scratchpad_uploaded_cb(gw_error_code, param)
 
             - gw_error_code: :obj:`~wirepas_mesh_messaging.gateway_result_code.GatewayResultCode`
             - param: param given when doing this call
 
-            .. warning:: If unset, call is synchronous and caller can be blocked for up to 60 seconds
+            .. warning:: If unset, call is synchronous and caller can be blocked for up to specified timeout
 
         :type cb: function
         :param param: Optional parameter that will be passed to callback
         :type param: object
+        :param timeout: Timeout in second to wait for the upload (default 60s)
+        :type timeout: int
         :return: None if cb is set or error code from gateway is synchronous call
         :rtype: :obj:`~wirepas_mesh_messaging.gateway_result_code.GatewayResultCode`
 
-        :raises TimeoutError: Raised if cb is None and response is not received within 60 sec
+        :raises TimeoutError: Raised if cb is None and response is not received within the specified timeout
         """
         request = wmm.UploadScratchpadRequest(seq, sink_id, scratchpad=scratchpad)
 
         self._publish(TopicGenerator.make_otap_load_scratchpad_request_topic(gw_id, sink_id),
                       request.payload,
                       1)
-        return self._wait_for_response(cb, request.req_id, timeout=60, param=param)
+        return self._wait_for_response(cb, request.req_id, timeout=timeout, param=param)
 
-    @_wait_for_configs
+    @_wait_for_connection
     def process_scratchpad(self, gw_id, sink_id, cb=None, param=None):
         """
         process_scratchpad(self, gw_id, sink_id, cb=None, param=None)
         Process scratchpad on a given sink
 
         :param gw_id: Id of gateway the sink is attached
         :type gw_id: str
@@ -655,15 +718,15 @@
         request = wmm.ProcessScratchpadRequest(sink_id)
 
         self._publish(TopicGenerator.make_otap_process_scratchpad_request_topic(gw_id, sink_id),
                       request.payload,
                       1)
         return self._wait_for_response(cb, request.req_id, timeout=60, param=param)
 
-    @_wait_for_configs
+    @_wait_for_connection
     def get_scratchpad_status(self, gw_id, sink_id, cb=None, param=None):
         """
         get_scratchpad_status(self, gw_id, sink_id, cb=None, param=None)
         Get scratchpad status of a given sink
 
         :param gw_id: Id of gateway the sink is attached
         :type gw_id: str
@@ -707,15 +770,15 @@
         request = wmm.GetScratchpadStatusRequest(sink_id)
 
         self._publish(TopicGenerator.make_otap_status_request_topic(gw_id, sink_id),
                       request.payload,
                       1)
         return self._wait_for_response(cb, request.req_id, param=param)
 
-    @_wait_for_configs
+    @_wait_for_connection
     def set_target_scratchpad(self, gw_id, sink_id, action, cb=None, param=None):
         """
         set_target_scratchpad(self, gw_id, sink_id, action, cb=None, param=None)
         Set target scratchpad on a given sink
 
         :param gw_id: Id of gateway the sink is attached
         :type gw_id: str
@@ -749,41 +812,82 @@
 
         self._publish(TopicGenerator.make_otap_set_target_scratchpad_request_topic(gw_id, sink_id),
                       request.payload,
                       1)
         return self._wait_for_response(cb, request.req_id, param=param)
 
     def register_data_cb(self, cb, gateway=None, sink=None, network=None, src_ep=None, dst_ep=None):
+        """Deprecated
+        Replaced by :meth:`~wirepas_mqtt_library.wirepas_network_interface.WirepasNetworkInterface.register_uplink_traffic_cb`
+        Only name has changed
+        """
+        return self.register_uplink_traffic_cb(cb, gateway, sink, network, src_ep, dst_ep)
+
+    def unregister_data_cb(self, id):
+        """Deprecated
+        Replaced by :meth:`~wirepas_mqtt_library.wirepas_network_interface.WirepasNetworkInterface.unregister_uplink_traffic_cb`
+        Only name has changed
+        """
+        return self.unregister_uplink_traffic_cb(id)
+
+    def register_uplink_traffic_cb(self, cb, gateway=None, sink=None, network=None, src_ep=None, dst_ep=None):
         """
-        Register a data filter to received filtered data
+        Register a data filter to received uplink filtered data
 
         :param cb: Callback to be called when a matching packet is received
         :param gateway: Filter on a given gateway (None for all)
         :param sink: Filter on a given sink (None for all)
         :param network: Filter on a given network (None for all)
         :param src_ep: Filter on a given source endpoint (None for all)
         :param dst_ep: Filter on a given destination endpoint (None for all)
         :return: The id of this filter, to be used when removing it with
             :meth:`~wirepas_mqtt_library.wirepas_network_interface.WirepasNetworkInterface.unregister_data_cb`
         """
         new_filter = _DataFilter(cb, gateway, sink, network, src_ep, dst_ep)
-        self._data_filters[id(new_filter)] = new_filter
+        self._data_uplink_filters[id(new_filter)] = new_filter
 
         return id(new_filter)
 
-    def unregister_data_cb(self, id):
+    def unregister_uplink_traffic_cb(self, id):
+        """Unregister uplink data callback previously registered
+        with :meth:`~wirepas_mqtt_library.wirepas_network_interface.WirepasNetworkInterface.register_uplink_traffic_cb`
+
+        :param id: id returned when adding the filter
+        :raises KeyError: if id doesn't exist
+        """
+        del self._data_uplink_filters[id]
+
+    def register_downlink_traffic_cb(self, cb, gateway=None, sink=None, src_ep=None, dst_ep=None):
+        """
+        Register a data filter to received downlink filtered data
+
+        :param cb: Callback to be called when a matching packet is received
+        :param gateway: Filter on a given gateway (None for all)
+        :param sink: Filter on a given sink (None for all)
+        :param src_ep: Filter on a given source endpoint (None for all)
+        :param dst_ep: Filter on a given destination endpoint (None for all)
+        :return: The id of this filter, to be used when removing it with
+            :meth:`~wirepas_mqtt_library.wirepas_network_interface.WirepasNetworkInterface.unregister_downlink_traffic_cb`
+        """
+        # Downlink traffic do not have network address field. It could be determined based on gateway/sink config
+        new_filter = _DataFilter(cb, gateway, sink, None, src_ep, dst_ep)
+        self._data_downlink_filters[id(new_filter)] = new_filter
+
+        return id(new_filter)
+
+    def unregister_downlink_traffic_cb(self, id):
         """Unregister data callback previously registered
-        with :meth:`~wirepas_mqtt_library.wirepas_network_interface.WirepasNetworkInterface.register_data_cb`
+        with :meth:`~wirepas_mqtt_library.wirepas_network_interface.WirepasNetworkInterface.register_downlink_traffic_cb`
 
         :param id: id returned when adding the filter
         :raises KeyError: if id doesn't exist
         """
-        del self._data_filters[id]
+        del self._data_downlink_filters[id]
 
-    @_wait_for_configs
+    @_wait_for_connection
     def set_sink_config(self, gw_id, sink_id, new_config, cb=None, param=None):
         """
         set_sink_config(self, gw_id, sink_id, new_config, cb=None, param=None)
         Set the config of a sink
 
         Configuration is sent as dictionary. Call can be clocking or unblocking
         depending on ``cb`` parameter.
@@ -838,14 +942,15 @@
 
         self._publish(TopicGenerator.make_set_config_request_topic(gw_id, sink_id),
                       request.payload,
                       1)
         # Extend default delay as it may require a reboot of sink
         return self._wait_for_response(cb, request.req_id, timeout=5, param=param)
 
+    @_wait_for_connection
     @_wait_for_configs
     def set_config_changed_cb(self, cb):
         """
         set_config_changed_cb(self, cb)
         Set a callback to be called when a config has changed on any of
         the attached gateway
 
@@ -891,15 +996,15 @@
         else:
             self.dst_ep = dst_ep
 
         if cb is None:
             raise ValueError("Callback must be specified")
         self.callback = cb
 
-    def filter_and_dispatch(self, message):
+    def filter_and_dispatch(self, message, *args):
         if self.gateway is not None and message.gw_id not in self.gateway:
             return
 
         if self.sink is not None and message.sink_id not in self.sink:
             return
 
         if self.network is not None and message.network_address not in self.network:
@@ -908,15 +1013,15 @@
         if self.src_ep is not None and message.source_endpoint not in self.src_ep:
             return
 
         if self.dst_ep is not None and message.destination_endpoint not in self.dst_ep:
             return
 
         # Message is not filtered and can be dispatched
-        self.callback(message)
+        self.callback(message, *args)
 
 
 class _TaskQueue(Queue):
     def __init__(self, num_worker=1):
         self._num_worker = num_worker
 
         Queue.__init__(self)
```

### Comparing `wirepas_mqtt_library-1.2rc1/wirepas_mqtt_library/wirepas_otap_helper.py` & `wirepas_mqtt_library-1.2rc2/wirepas_mqtt_library/wirepas_otap_helper.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # Copyright 2021 Wirepas Ltd. All Rights Reserved.
 #
 # See file LICENSE.txt for full license details.
 #
+from threading import Event
+from time import sleep
 import wirepas_mesh_messaging as wmm
 import logging
 from struct import pack, unpack
 from random import randint
 
 
 class WirepasOtapHelper:
@@ -131,47 +133,72 @@
             new_status["target_crc"] = target_crc
             new_status["target_seq"] = target_seq
             new_status["target_delay_m"] = target_delay
             new_status["remaining_delay_m"] = remaining_delay
 
         self._nodes[data.source_address] = new_status
 
-    def load_scratchpad_to_all_sinks(self, scratchpad_file, seq=None):
+    def load_scratchpad_to_all_sinks(self, scratchpad_file, seq=None, timeout=60, delay_between_sinks_s=1):
         """Load the specified scratchpad file on all sinks of the network
 
         :param scratchpad_file: scratchpad file with .otap extension
         :type scratchpad_file: str
         :param seq: optional seq for the scratchpad. If not given a random one is chosen
         :type seq: int
+        :param timeout: maximum time to wait for each scratchpad upload
+        :type timeout: int
+        :param delay_between_sinks_s: time to wait between the sending of a load scratchpad between sinks.
+                                      On large network, it may help to avoid loading the broker too much.
+        :type delay_between_sinks_s: int
         :return: True if scratchpad is correctly loaded on all sinks, false otherwise
         """
+        all_expected_answers = set()
+        all_received = Event()
+        final_result = True
+
         # Read the scratchpad file as binary
         try:
             with open(scratchpad_file, "rb") as f:
                 scratchpad = f.read()
         except Exception as e:
             logging.error("Cannot read scratchpad file: [%s] " % str(e))
             return False
 
         if seq is None:
             seq = randint(1, 254)
 
+        def _on_scratchpad_loaded_cb(gw_error_code, param):
+            nonlocal final_result
+            if gw_error_code != wmm.GatewayResultCode.GW_RES_OK:
+                logging.error("Scratchpad loaded error on [%s][%s]: [%s] " % (param[0], param[1], gw_error_code))
+                final_result = False
+            else:
+                logging.debug("Scratchpad loaded successfully on [%s][%s]" % (param[0], param[1]))
+
+            try:
+                all_expected_answers.remove((param[0], param[1]))
+            except KeyError:
+                logging.error("Answer already received: duplicated for [%s][%s]" % (param[0], param[1]))
+
+            # Check if everybody has answered
+            if all_expected_answers.__len__() == 0:
+                all_received.set()
+
         logging.info("Loading scratchpad with seq = %d to all sinks for network %d" %(seq, self.network))
-        for gw, sink, config in self._sinks:
+        for gw, sink, _ in self._sinks:
             logging.debug("Loading scratchpad to [%s][%s] " % (gw, sink))
-            try:
-                res = self.wni.upload_scratchpad(gw, sink, seq, scratchpad)
-                if res != wmm.GatewayResultCode.GW_RES_OK:
-                    logging.error("Scratchpad loaded error: [%s] " % res)
-                    return False
-                logging.debug("Scratchpad loaded correctly")
-            except TimeoutError:
-                logging.error("Cannot load scratchpad to [%s][%s] => Timeout " % (gw, sink))
-                return False
-        return True
+            self.wni.upload_scratchpad(gw, sink, seq, scratchpad, cb=_on_scratchpad_loaded_cb, param=(gw, sink), timeout=timeout)
+            all_expected_answers.add((gw, sink))
+            sleep(delay_between_sinks_s)
+
+        if not all_received.wait(timeout):
+            logging.error("Some sinks do not answered within timeout %s" % all_expected_answers)
+            final_result = False
+
+        return final_result
 
     def process_scratchpad_on_all_sinks(self):
         """Process the scratchpad locally on all sinks of the network
 
         :return: True if scratchpad is correctly set to be processed on all sinks, false otherwise
         """
         logging.info("Processing scratchpad on all sinks for network %d" % self.network)
```

### Comparing `wirepas_mqtt_library-1.2rc1/wirepas_mqtt_library/wirepas_tlv_app_config_helper.py` & `wirepas_mqtt_library-1.2rc2/wirepas_mqtt_library/wirepas_tlv_app_config_helper.py`

 * *Files identical despite different names*

### Comparing `wirepas_mqtt_library-1.2rc1/wirepas_mqtt_library.egg-info/PKG-INFO` & `wirepas_mqtt_library-1.2rc2/wirepas_mqtt_library.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wirepas-mqtt-library
-Version: 1.2rc1
+Version: 1.2rc2
 Summary: Library to interact with a Wirepas Network through MQTT/Protobuf API
 Home-page: https://github.com/wirepas/wirepas-mqtt-library
 Author: Wirepas Ltd
 Author-email: opensource@wirepas.com
 License: Apache-2
 Description: Wirepas MQTT Library
         ====================
```

