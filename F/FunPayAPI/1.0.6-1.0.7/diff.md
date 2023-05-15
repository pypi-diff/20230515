# Comparing `tmp/FunPayAPI-1.0.6.tar.gz` & `tmp/FunPayAPI-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FunPayAPI-1.0.6.tar", last modified: Fri May 12 11:54:20 2023, max compression
+gzip compressed data, was "FunPayAPI-1.0.7.tar", last modified: Mon May 15 12:05:55 2023, max compression
```

## Comparing `FunPayAPI-1.0.6.tar` & `FunPayAPI-1.0.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 11:54:20.468076 FunPayAPI-1.0.6/
-drwxrwxrwx   0        0        0        0 2023-05-12 11:54:20.446075 FunPayAPI-1.0.6/FunPayAPI/
--rw-rw-rw-   0        0        0      162 2023-05-10 15:12:44.000000 FunPayAPI-1.0.6/FunPayAPI/__init__.py
--rw-rw-rw-   0        0        0    56140 2023-05-12 11:17:47.000000 FunPayAPI-1.0.6/FunPayAPI/account.py
-drwxrwxrwx   0        0        0        0 2023-05-12 11:54:20.465076 FunPayAPI-1.0.6/FunPayAPI/common/
--rw-rw-rw-   0        0        0        0 2023-05-12 11:30:08.000000 FunPayAPI-1.0.6/FunPayAPI/common/__init__.py
--rw-rw-rw-   0        0        0     4667 2023-05-11 19:19:43.000000 FunPayAPI-1.0.6/FunPayAPI/common/enums.py
--rw-rw-rw-   0        0        0     6509 2023-05-12 11:25:10.000000 FunPayAPI-1.0.6/FunPayAPI/common/exceptions.py
--rw-rw-rw-   0        0        0     8033 2023-04-14 18:22:19.000000 FunPayAPI-1.0.6/FunPayAPI/common/utils.py
--rw-rw-rw-   0        0        0    38990 2023-05-11 19:44:24.000000 FunPayAPI-1.0.6/FunPayAPI/types.py
-drwxrwxrwx   0        0        0        0 2023-05-12 11:54:20.467077 FunPayAPI-1.0.6/FunPayAPI/updater/
--rw-rw-rw-   0        0        0        0 2023-05-12 11:30:17.000000 FunPayAPI-1.0.6/FunPayAPI/updater/__init__.py
--rw-rw-rw-   0        0        0     8216 2023-05-11 19:12:41.000000 FunPayAPI-1.0.6/FunPayAPI/updater/events.py
--rw-rw-rw-   0        0        0    20333 2023-05-12 11:15:09.000000 FunPayAPI-1.0.6/FunPayAPI/updater/runner.py
-drwxrwxrwx   0        0        0        0 2023-05-12 11:54:20.461075 FunPayAPI-1.0.6/FunPayAPI.egg-info/
--rw-rw-rw-   0        0        0     3602 2023-05-12 11:54:20.000000 FunPayAPI-1.0.6/FunPayAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      450 2023-05-12 11:54:20.000000 FunPayAPI-1.0.6/FunPayAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 11:54:20.000000 FunPayAPI-1.0.6/FunPayAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-05-12 11:54:20.000000 FunPayAPI-1.0.6/FunPayAPI.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-12 11:54:20.000000 FunPayAPI-1.0.6/FunPayAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35801 2023-05-11 21:13:41.000000 FunPayAPI-1.0.6/LICENSE
--rw-rw-rw-   0        0        0     3602 2023-05-12 11:54:20.467077 FunPayAPI-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     3011 2023-05-12 11:49:15.000000 FunPayAPI-1.0.6/README.md
--rw-rw-rw-   0        0        0       42 2023-05-12 11:54:20.468076 FunPayAPI-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0      928 2023-05-12 11:54:09.000000 FunPayAPI-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 12:05:55.271564 FunPayAPI-1.0.7/
+drwxrwxrwx   0        0        0        0 2023-05-15 12:05:55.240563 FunPayAPI-1.0.7/FunPayAPI/
+-rw-rw-rw-   0        0        0      162 2023-05-10 15:12:44.000000 FunPayAPI-1.0.7/FunPayAPI/__init__.py
+-rw-rw-rw-   0        0        0    60938 2023-05-15 11:55:25.000000 FunPayAPI-1.0.7/FunPayAPI/account.py
+drwxrwxrwx   0        0        0        0 2023-05-15 12:05:55.265563 FunPayAPI-1.0.7/FunPayAPI/common/
+-rw-rw-rw-   0        0        0        0 2023-05-12 17:46:25.000000 FunPayAPI-1.0.7/FunPayAPI/common/__init__.py
+-rw-rw-rw-   0        0        0     4842 2023-05-14 16:49:23.000000 FunPayAPI-1.0.7/FunPayAPI/common/enums.py
+-rw-rw-rw-   0        0        0     7842 2023-05-14 23:54:13.000000 FunPayAPI-1.0.7/FunPayAPI/common/exceptions.py
+-rw-rw-rw-   0        0        0     8033 2023-04-14 18:22:19.000000 FunPayAPI-1.0.7/FunPayAPI/common/utils.py
+-rw-rw-rw-   0        0        0    38383 2023-05-14 23:53:13.000000 FunPayAPI-1.0.7/FunPayAPI/types.py
+drwxrwxrwx   0        0        0        0 2023-05-15 12:05:55.270564 FunPayAPI-1.0.7/FunPayAPI/updater/
+-rw-rw-rw-   0        0        0        0 2023-05-12 17:46:18.000000 FunPayAPI-1.0.7/FunPayAPI/updater/__init__.py
+-rw-rw-rw-   0        0        0     8216 2023-05-11 19:12:41.000000 FunPayAPI-1.0.7/FunPayAPI/updater/events.py
+-rw-rw-rw-   0        0        0    20435 2023-05-15 12:03:15.000000 FunPayAPI-1.0.7/FunPayAPI/updater/runner.py
+drwxrwxrwx   0        0        0        0 2023-05-15 12:05:55.254563 FunPayAPI-1.0.7/FunPayAPI.egg-info/
+-rw-rw-rw-   0        0        0     3602 2023-05-15 12:05:55.000000 FunPayAPI-1.0.7/FunPayAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      450 2023-05-15 12:05:55.000000 FunPayAPI-1.0.7/FunPayAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 12:05:55.000000 FunPayAPI-1.0.7/FunPayAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-05-15 12:05:55.000000 FunPayAPI-1.0.7/FunPayAPI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-15 12:05:55.000000 FunPayAPI-1.0.7/FunPayAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35801 2023-05-11 21:13:41.000000 FunPayAPI-1.0.7/LICENSE
+-rw-rw-rw-   0        0        0     3602 2023-05-15 12:05:55.271564 FunPayAPI-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3011 2023-05-12 11:49:15.000000 FunPayAPI-1.0.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-15 12:05:55.272563 FunPayAPI-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      928 2023-05-15 12:05:39.000000 FunPayAPI-1.0.7/setup.py
```

### Comparing `FunPayAPI-1.0.6/FunPayAPI/account.py` & `FunPayAPI-1.0.7/FunPayAPI/account.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from __future__ import annotations
-from typing import TYPE_CHECKING, Literal, Any, Optional
+from typing import TYPE_CHECKING, Literal, Any, Optional, IO
 if TYPE_CHECKING:
     from .updater.runner import Runner
 
 from requests_toolbelt import MultipartEncoder
 from bs4 import BeautifulSoup
 import requests
 import logging
 import random
 import string
 import json
 import time
 
 from . import types
-from .common import exceptions, utils
+from .common import exceptions, utils, enums
 
 
 logger = logging.getLogger("FunPayAPI.account")
 
 
 class Account:
     """
@@ -49,18 +49,14 @@
         """HTML основной страницы FunPay."""
         self.app_data: dict | None = None
         """Appdata."""
         self.id: int | None = None
         """ID аккаунта."""
         self.username: str | None = None
         """Никнейм аккаунта."""
-        self.balance: int | None = None
-        """Баланс аккаунта."""
-        self.currency: str | None = None
-        """Валюта аккаунта."""
         self.active_sales: int | None = None
         """Активные продажи."""
         self.active_purchases: int | None = None
         """Активные покупки."""
 
         self.csrf_token: str | None = None
         """CSRF токен."""
@@ -86,15 +82,15 @@
 
     def method(self, request_method: Literal["post", "get"], api_method: str, headers: dict, payload: Any,
                exclude_phpsessid: bool = False, raise_not_200: bool = False) -> requests.Response:
         """
         Отправляет запрос к FunPay. Добавляет в заголовки запроса user_agent и куки.
 
         :param request_method: метод запроса ("get" / "post").
-        :type request_method: Literal["post", "get"]
+        :type request_method: :obj:`str` `post` or `get`
 
         :param api_method: метод API / полная ссылка.
         :type api_method: :obj:`str`
 
         :param headers: заголовки запроса.
         :type headers: :obj:`dict`
 
@@ -122,15 +118,16 @@
             raise exceptions.UnauthorizedError(response)
         elif response.status_code != 200 and raise_not_200:
             raise exceptions.RequestFailedError(response)
         return response
 
     def get(self, update_phpsessid: bool = False) -> Account:
         """
-        Получает / обновляет данные об аккаунте.
+        Получает / обновляет данные об аккаунте. Необходимо вызывать каждые 40-60 минут, дабы обновить
+        :py:obj:`.Account.phpsessid`.
 
         :param update_phpsessid: обновить :py:obj:`.Account.phpsessid` или использовать старый.
         :type update_phpsessid: :obj:`bool`, опционально
 
         :return: объект аккаунта с обновленными данными.
         :rtype: :class:`FunPayAPI.account.Account`
         """
@@ -150,79 +147,104 @@
 
         active_sales = parser.find("span", {"class": "badge badge-trade"})
         self.active_sales = int(active_sales.text) if active_sales else 0
 
         active_purchases = parser.find("span", {"class": "badge badge-orders"})
         self.active_purchases = int(active_purchases.text) if active_purchases else 0
 
-        balance_badge = parser.find("span", {"class": "badge badge-balance"})
-        self.balance = float("".join(balance_badge.text.split(" ")[:-1])) if balance_badge else 0
-        self.currency = balance_badge.text.split(" ")[-1] if balance_badge else ""
-
         cookies = response.cookies.get_dict()
         if update_phpsessid or not self.phpsessid:
             self.phpsessid = cookies["PHPSESSID"]
-
-        if not self.is_initiated():
+        if not self.is_initiated:
             self.__setup_categories(html_response)
 
         self.last_update = int(time.time())
         self.html = html_response
         self.__initiated = True
         return self
 
+    def get_balance(self, lot_id: int = 18853876) -> types.Balance:
+        """
+        Получает информацию о балансе пользователя.
+
+        :param lot_id: ID лота, на котором проверять баланс.
+        :type lot_id: :obj:`int`, опционально
+
+        :return: информацию о балансе пользователя.
+        :rtype: :class:`FunPayAPI.types.Balance`
+        """
+        if not self.is_initiated:
+            raise exceptions.AccountNotInitiatedError()
+        response = self.method("get", f"lots/offer?id={lot_id}", {"accept": "*/*"}, {}, raise_not_200=True)
+        html_response = response.content.decode()
+        parser = BeautifulSoup(html_response, "html.parser")
+
+        username = parser.find("div", {"class": "user-link-name"})
+        if not username:
+            raise exceptions.UnauthorizedError(response)
+
+        balances = parser.find("select", {"name": "method"})
+        balance = types.Balance(float(balances["data-balance-total-rub"]), float(balances["data-balance-rub"]),
+                                float(balances["data-balance-total-usd"]), float(balances["data-balance-usd"]),
+                                float(balances["data-balance-total-eur"]), float(balances["data-balance-eur"]))
+        return balance
+
     def get_chat_history(self, chat_id: int | str, last_message_id: int = 99999999999999999999999,
-                         interlocutor_username: str | None = None, from_id: int = 0) -> list[types.Message]:
+                         interlocutor_username: Optional[str] = None, from_id: int = 0) -> list[types.Message]:
         """
         Получает историю указанного чата (до 100 последних сообщений).
 
         :param chat_id: ID чата (или его текстовое обозначение).
         :type chat_id: :obj:`int` or :obj:`str`
 
         :param last_message_id: ID сообщения, с которого начинать историю (фильтр FunPay).
         :type last_message_id: :obj:`int`
 
-        :param interlocutor_username: никнейм собеседника. Упрощает идентификацию авторов сообщения. Не работает, если
-            запрошена история публичного чата.
+        :param interlocutor_username: никнейм собеседника. Не нужно указывать для получения истории публичного чата.
+            Так же не обязательно, но желательно указывать для получения истории личного чата.
         :type interlocutor_username: :obj:`str` or :obj:`None`, опционально.
 
         :param from_id: все сообщения с ID < переданного не попадут в возвращаемый список сообщений.
         :type from_id: :obj:`int`, опционально.
 
         :return: история указанного чата.
         :rtype: :obj:`list` of :class:`FunPayAPI.types.Message`
         """
-        if not self.is_initiated():
+        if not self.is_initiated:
             raise exceptions.AccountNotInitiatedError()
 
         headers = {
             "accept": "*/*",
             "x-requested-with": "XMLHttpRequest"
         }
         payload = {
             "node": chat_id,
             "last_message": last_message_id
         }
-        response = self.method("get", f"https://funpay.com/chat/history?node={chat_id}&last_message={last_message_id}",
+        response = self.method("get", f"chat/history?node={chat_id}&last_message={last_message_id}",
                                headers, payload, raise_not_200=True)
 
         json_response = response.json()
         if not json_response.get("chat") or not json_response["chat"].get("messages"):
             return []
-        interlocutor_id = int(json_response["chat"]["node"]["name"].split("-")[2])
+        if isinstance(chat_id, int):
+            interlocutor_id = int(json_response["chat"]["node"]["name"].split("-")[2])
+        else:
+            interlocutor_id = None
         return self.__parse_messages(json_response["chat"]["messages"], chat_id, interlocutor_id,
                                      interlocutor_username, from_id)
 
-    def get_chats_histories(self, chats_data: dict[int, str | None]) -> dict[int, list[types.Message]]:
+    def get_chats_histories(self, chats_data: dict[int | str, str | None]) -> dict[int, list[types.Message]]:
         """
-        Получает историю сообщений сразу нескольких личных чатов (до 100 сообщений на 1 чат).
+        Получает историю сообщений сразу нескольких чатов
+        (до 50 сообщений на личный чат, до 25 сообщений на публичный чат).
 
         :param chats_data: ID чатов и никнеймы собеседников (None, если никнейм неизвестен)\n
             Например: {48392847: "SLLMK", 58392098: "Amongus", 38948728: None}
-        :type chats_data: :obj:`dict` {:obj:`int`: :obj:`str` or :obj:`None`}
+        :type chats_data: :obj:`dict` {:obj:`int` or :obj:`str`: :obj:`str` or :obj:`None`}
 
         :return: словарь с историями чатов в формате {ID чата: [список сообщений]}
         :rtype: :obj:`dict` {:obj:`int`: :obj:`list` of :class:`FunPayAPI.types.Message`}
         """
         headers = {
             "accept": "*/*",
             "content-type": "application/x-www-form-urlencoded; charset=UTF-8",
@@ -231,63 +253,66 @@
         objects = [{"type": "chat_node", "id": i, "tag": "00000000",
                     "data": {"node": i, "last_message": -1, "content": ""}} for i in chats_data]
         payload = {
             "objects": json.dumps(objects),
             "request": False,
             "csrf_token": self.csrf_token
         }
-        response = self.method("post", "https://funpay.com/runner/", headers, payload, raise_not_200=True)
+        response = self.method("post", "runner/", headers, payload, raise_not_200=True)
         json_response = response.json()
 
         result = {}
         for i in json_response["objects"]:
             if not i.get("data"):
                 result[i.get("id")] = []
                 continue
-            interlocutor_id = int(i["data"]["node"]["name"].split("-")[2])
-            messages = self.__parse_messages(i["data"]["messages"], i.get("id"), interlocutor_id,
-                                             chats_data[i.get("id")])
+            if isinstance(i.get("id"), int):
+                interlocutor_id = int(i["data"]["node"]["name"].split("-")[2])
+                interlocutor_name = chats_data[i.get("id")]
+            else:
+                interlocutor_id = None
+                interlocutor_name = None
+            messages = self.__parse_messages(i["data"]["messages"], i.get("id"), interlocutor_id, interlocutor_name)
             result[i.get("id")] = messages
         return result
 
-    def upload_image(self, image: str | bytes) -> int:
+    def upload_image(self, image: str | IO[bytes]) -> int:
         """
         Выгружает изображение на сервер FunPay для дальнейшей отправки в качестве сообщения.
+        Для отправки изображения в чат рекомендуется использовать метод :meth:`FunPayAPI.account.Account.send_image`.
 
-        :param image: путь до изображения или изображение в виде байтов.
+        :param image: путь до изображения или представление изображения в виде байтов.
         :type image: :obj:`str` or :obj:`bytes`
 
-        :return: ID изображения на FunPay.
+        :return: ID изображения на серверах FunPay.
         :rtype: :obj:`int`
         """
-        if not self.is_initiated():
+        if not self.is_initiated:
             raise exceptions.AccountNotInitiatedError()
 
         if isinstance(image, str):
             with open(image, "rb") as f:
                 img = f.read()
         else:
             img = image
 
         fields = {
             'file': ("funpay_cardinal_image.png", img, "image/png"),
             'file_id': "0"
         }
-        boundary = '----WebKitFormBoundary' \
-                   + ''.join(random.sample(string.ascii_letters + string.digits, 16))
+        boundary = '----WebKitFormBoundary' + ''.join(random.sample(string.ascii_letters + string.digits, 16))
         m = MultipartEncoder(fields=fields, boundary=boundary)
 
         headers = {
             "accept": "*/*",
             "x-requested-with": "XMLHttpRequest",
             "content-type": m.content_type,
         }
 
-        link = "https://funpay.com/file/addChatImage"
-        response = self.method("post", link, headers, m)
+        response = self.method("post", "file/addChatImage", headers, m)
 
         if response.status_code == 400:
             try:
                 json_response = response.json()
                 message = json_response.get("msg")
                 raise exceptions.ImageUploadError(response, message)
             except requests.exceptions.JSONDecodeError:
@@ -295,42 +320,42 @@
         elif response.status_code != 200:
             raise exceptions.RequestFailedError(response)
 
         if not (document_id := response.json().get("fileId")):
             raise exceptions.ImageUploadError(response, None)
         return int(document_id)
 
-    def send_message(self, chat_id: int | str, text: str | None, chat_name: str | None = None,
-                     image_id: int | None = None, add_to_ignore_list: bool = True,
+    def send_message(self, chat_id: int | str, text: Optional[str] = None, chat_name: Optional[str] = None,
+                     image_id: Optional[int] = None, add_to_ignore_list: bool = True,
                      update_last_saved_message: bool = False) -> types.Message:
         """
         Отправляет сообщение в чат.
 
-        :param chat_id: ID чата или чего текстовое обозначение.
+        :param chat_id: ID чата.
         :type chat_id: :obj:`int` or :obj:`str`
 
         :param text: текст сообщения.
-        :type text: :obj:`str` or :obj:`None`
+        :type text: :obj:`str` or :obj:`None`, опционально
 
         :param chat_name: название чата (для возвращаемого объекта сообщения) (не нужно для отправки сообщения в публичный чат).
         :type chat_name: :obj:`str` or :obj:`None`, опционально
 
-        :param image_id: ID изображения.
+        :param image_id: ID изображения. Доступно только для личных чатов.
         :type image_id: :obj:`int` or :obj:`None`, опционально
 
         :param add_to_ignore_list: добавлять ли ID отправленного сообщения в игнорируемый список Runner'а?
         :type add_to_ignore_list: :obj:`bool`, опционально
 
         :param update_last_saved_message: обновлять ли последнее сохраненное сообщение на отправленное в Runner'е?
         :type update_last_saved_message: :obj:`bool`, опционально.
 
         :return: экземпляр отправленного сообщения.
         :rtype: :class:`FunPayAPI.types.Message`
         """
-        if not self.is_initiated():
+        if not self.is_initiated:
             raise exceptions.AccountNotInitiatedError()
 
         headers = {
             "accept": "*/*",
             "content-type": "application/x-www-form-urlencoded; charset=UTF-8",
             "x-requested-with": "XMLHttpRequest"
         }
@@ -339,15 +364,15 @@
             "data": {"node": chat_id, "last_message": -1, "content": text}
         }
 
         if image_id is not None:
             request["data"]["image_id"] = image_id
             request["data"]["content"] = ""
         else:
-            request["data"]["content"] = text
+            request["data"]["content"] = text or ""
 
         objects = [
             {
                 "type": "chat_node",
                 "id": chat_id,
                 "tag": "00000000",
                 "data": {"node": chat_id, "last_message": -1, "content": ""}
@@ -355,79 +380,109 @@
         ]
         payload = {
             "objects": json.dumps(objects),
             "request": json.dumps(request),
             "csrf_token": self.csrf_token
         }
 
-        link = "https://funpay.com/runner/"
-        response = self.method("post", link, headers, payload, raise_not_200=True)
-
+        response = self.method("post", "runner/", headers, payload, raise_not_200=True)
         json_response = response.json()
+        if not (resp := json_response.get("response")):
+            raise exceptions.MessageNotDeliveredError(response, None, chat_id)
 
-        if json_response.get("response"):
-            if json_response.get("response").get("error") is not None:
-                raise exceptions.MessageNotDeliveredError(response, json_response.get("error"), chat_id)
+        if (error_text := resp.get("error")) is not None:
+            raise exceptions.MessageNotDeliveredError(response, error_text, chat_id)
 
-            mes = json_response["objects"][0]["data"]["messages"][-1]
-            parser = BeautifulSoup(mes["html"], "html.parser")
-            try:
-                if image_link := parser.find("a", {"class": "chat-img-link"}):
-                    image_link = image_link.get("href")
-                    message_text = None
-                else:
-                    message_text = parser.find("div", {"class": "message-text"}).text
-            except Exception as e:
-                logger.debug("SEND_MESSAGE RESPONSE")
-                logger.debug(response.content.decode())
-                raise e
-
-            message_obj = types.Message(int(mes["id"]), message_text, chat_id, chat_name,
-                                        self.username, self.id, mes["html"], image_link)
-            if self.runner:
-                if add_to_ignore_list:
-                    self.runner.mark_as_by_bot(chat_id, message_obj.id)
-                if update_last_saved_message:
-                    self.runner.update_last_message(chat_id, message_text)
-            return message_obj
-        else:
-            raise exceptions.MessageNotDeliveredError(response, None, chat_id)
+        mes = json_response["objects"][0]["data"]["messages"][-1]
+        parser = BeautifulSoup(mes["html"], "html.parser")
+        try:
+            if image_link := parser.find("a", {"class": "chat-img-link"}):
+                image_link = image_link.get("href")
+                message_text = None
+            else:
+                message_text = parser.find("div", {"class": "message-text"}).text
+        except Exception as e:
+            logger.debug("SEND_MESSAGE RESPONSE")
+            logger.debug(response.content.decode())
+            raise e
+
+        message_obj = types.Message(int(mes["id"]), message_text, chat_id, chat_name,
+                                    self.username, self.id, mes["html"], image_link)
+        if self.runner and isinstance(chat_id, int):
+            if add_to_ignore_list:
+                self.runner.mark_as_by_bot(chat_id, message_obj.id)
+            if update_last_saved_message:
+                self.runner.update_last_message(chat_id, message_text)
+        return message_obj
+
+    def send_image(self, chat_id: int, image: int | str | IO[bytes], chat_name: Optional[str] = None,
+                   add_to_ignore_list: bool = True, update_last_saved_message: bool = False) -> types.Message:
+        """
+        Отправляет изображение в чат. Доступно только для личных чатов.
+
+        :param chat_id: ID чата.
+        :type chat_id: :obj:`int`
+
+        :param image: ID изображения / путь до изображения / изображение в виде байтов.
+            Если передан путь до изображения или представление изображения в виде байтов, сначала оно будет выгружено
+            с помощью метода :meth:`FunPayAPI.account.Account.upload_image`.
+        :type image: :obj:`int` or :obj:`str` or :obj:`bytes`
+
+        :param chat_name: Название чата (никнейм собеседника). Нужен для возвращаемого объекта.
+        :type chat_name: :obj:`str` or :obj:`None`, опционально
+
+        :param add_to_ignore_list: добавлять ли ID отправленного сообщения в игнорируемый список Runner'а?
+        :type add_to_ignore_list: :obj:`bool`, опционально
+
+        :param update_last_saved_message: обновлять ли последнее сохраненное сообщение на отправленное в Runner'е?
+        :type update_last_saved_message: :obj:`bool`, опционально
 
-    def send_review(self, order_id: str, text: str, rating: int) -> str:
+        :return: объект отправленного сообщения.
+        :rtype: :class:`FunPayAPI.types.Message`
+        """
+        if not self.is_initiated:
+            raise exceptions.AccountNotInitiatedError()
+
+        if not isinstance(image, int):
+            image = self.upload_image(image)
+        result = self.send_message(chat_id, None, chat_name, image, add_to_ignore_list, update_last_saved_message)
+        return result
+
+    def send_review(self, order_id: str, text: str, rating: Literal[1, 2, 3, 4, 5] = 5) -> str:
         """
         Отправляет / редактирует отзыв / ответ на отзыв.
 
         :param order_id: ID заказа.
         :type order_id: :obj:`str`
 
         :param text: текст отзыва.
         :type text: :obj:`str`
 
         :param rating: рейтинг (от 1 до 5).
-        :type rating: :obj:`int`
+        :type rating: :obj:`int`, опционально
 
         :return: ответ FunPay (HTML-код блока отзыва).
         :rtype: :obj:`str`
         """
-        if not self.is_initiated():
+        if not self.is_initiated:
             raise exceptions.AccountNotInitiatedError()
 
         headers = {
             "accept": "*/*",
             "x-requested-with": "XMLHttpRequest"
         }
         payload = {
             "authorId": self.id,
             "text": text,
             "rating": rating,
             "csrf_token": self.csrf_token,
             "orderId": order_id
         }
 
-        response = self.method("post", "https://funpay.com/orders/review", headers, payload)
+        response = self.method("post", "orders/review", headers, payload)
         if response.status_code == 400:
             json_response = response.json()
             msg = json_response.get("msg")
             raise exceptions.FeedbackEditingError(response, msg, order_id)
         elif response.status_code != 200:
             raise exceptions.RequestFailedError(response)
 
@@ -439,28 +494,28 @@
 
         :param order_id: ID заказа.
         :type order_id: :obj:`str`
 
         :return: ответ FunPay (HTML-код блока отзыва).
         :rtype: :obj:`str`
         """
-        if not self.is_initiated():
+        if not self.is_initiated:
             raise exceptions.AccountNotInitiatedError()
 
         headers = {
             "accept": "*/*",
             "x-requested-with": "XMLHttpRequest"
         }
         payload = {
             "authorId": self.id,
             "csrf_token": self.csrf_token,
             "orderId": order_id
         }
 
-        response = self.method("post", "https://funpay.com/orders/reviewDelete", headers, payload)
+        response = self.method("post", "orders/reviewDelete", headers, payload)
 
         if response.status_code == 400:
             json_response = response.json()
             msg = json_response.get("msg")
             raise exceptions.FeedbackEditingError(response, msg, order_id)
         elif response.status_code != 200:
             raise exceptions.RequestFailedError(response)
@@ -470,143 +525,191 @@
     def refund(self, order_id):
         """
         Оформляет возврат средств за заказ.
 
         :param order_id: ID заказа.
         :type order_id: :obj:`str`
         """
-        if not self.is_initiated():
+        if not self.is_initiated:
             raise exceptions.AccountNotInitiatedError()
 
         headers = {
             "accept": "*/*",
             "content-type": "application/x-www-form-urlencoded; charset=UTF-8",
             "x-requested-with": "XMLHttpRequest",
         }
 
         payload = {
             "id": order_id,
             "csrf_token": self.csrf_token
         }
 
-        response = self.method("post", "https://funpay.com/orders/refund", headers, payload, raise_not_200=True)
+        response = self.method("post", "orders/refund", headers, payload, raise_not_200=True)
 
         if response.json().get("error"):
             raise exceptions.RefundError(response, response.json().get("msg"), order_id)
 
-    def get_raise_modal(self, category_id: int, subcategory_id: int) -> dict:
+    def withdraw(self, currency: enums.Currency, wallet: enums.Wallet, amount: int | float, address: str) -> float:
+        """
+        Отправляет запрос на вывод средств.
+
+        :param currency: валюта.
+        :type currency: :class:`FunPayAPI.common.enums.Currency`
+
+        :param wallet: тип кошелька.
+        :type wallet: :class:`FunPayAPI.common.enums.Wallet`
+
+        :param amount: кол-во средств.
+        :type amount: :obj:`int` or :obj:`float`
+
+        :param address: адрес кошелька.
+        :type address: :obj:`str`
+
+        :return: кол-во выведенных средств с учетом комиссии FunPay.
+        :rtype: :obj:`float`
+        """
+        if not self.is_initiated:
+            raise exceptions.AccountNotInitiatedError()
+
+        currencies = {
+            enums.Currency.RUB: "rub",
+            enums.Currency.USD: "usd",
+            enums.Currency.EUR: "eur"
+        }
+
+        wallets = {
+            enums.Wallet.QIWI: "qiwi",
+            enums.Wallet.YOUMONEY: "fps",
+            enums.Wallet.BINANCE: "binance",
+            enums.Wallet.TRC: "usdt_trc",
+            enums.Wallet.CARD_RUB: "card_rub",
+            enums.Wallet.CARD_USD: "card_usd",
+            enums.Wallet.CARD_EUR: "card_eur",
+            enums.Wallet.WEBMONEY: "wmz"
+        }
+        headers = {
+            "accept": "*/*",
+            "x-requested-with": "XMLHttpRequest"
+        }
+        payload = {
+            "csrf_token": self.csrf_token,
+            "currency_id": currencies[currency],
+            "ext_currency_id": wallets[wallet],
+            "wallet": address,
+            "amount_int": str(amount)
+        }
+        response = self.method("post", "withdraw/withdraw", headers, payload, raise_not_200=True)
+        json_response = response.json()
+        if json_response.get("error"):
+            error_message = json_response.get("msg")
+            raise exceptions.WithdrawError(response, error_message)
+        return float(json_response.get("amount_ext"))
+
+    def get_raise_modal(self, category_id: int) -> dict:
         """
         Отправляет запрос на получение modal-формы для поднятия лотов категории (игры).
         !ВНИМАНИЕ! Если на аккаунте только 1 подкатегория, относящаяся переданной категории (игре),
         то FunPay поднимет лоты данной подкатегории без отправления modal-формы с выбором других подкатегорий.
 
         :param category_id: ID категории (игры).
         :type category_id: :obj:`int`
 
-        :param subcategory_id: ID любой подкатегории, относящейся к переданной категории.
-        :type subcategory_id: :obj:`int`
-
         :return: ответ FunPay.
         :rtype: :obj:`dict`
         """
-        if not self.is_initiated():
+        if not self.is_initiated:
             raise exceptions.AccountNotInitiatedError()
+        category = self.get_category(category_id)
+        subcategory = category.get_subcategories()[0]
         headers = {
             "accept": "*/*",
             "content-type": "application/x-www-form-urlencoded; charset=UTF-8",
             "x-requested-with": "XMLHttpRequest"
         }
         payload = {
             "game_id": category_id,
-            "node_id": subcategory_id
+            "node_id": subcategory.id
         }
         response = self.method("post", "https://funpay.com/lots/raise", headers, payload, raise_not_200=True)
         json_response = response.json()
         return json_response
 
-    def raise_subcategories(self, category_id: int, subcategory_id: int, exclude: list[int] | None = None) \
-            -> types.RaiseResponse:
+    def raise_lots(self, category_id: int, subcategories: Optional[list[int | types.SubCategory]] = None,
+                   exclude: list[int] | None = None) -> bool:
         """
         Поднимает все лоты всех подкатегорий переданной категории (игры).
 
         :param category_id: ID категории (игры).
         :type category_id: :obj:`int`
 
-        :param subcategory_id: ID любой подкатегории, относящейся к переданной категории.
-        :type subcategory_id: :obj:`int`
+        :param subcategories: список подкатегорий, которые необходимо поднять. Если не указаны, поднимутся все
+            подкатегории переданной категории.
+        :type subcategories: :obj:`list` of :obj:`int` or :class:`FunPayAPI.types.SubCategory`
 
         :param exclude: ID подкатегорий, которые не нужно поднимать.
         :type exclude: :obj:`list` of :obj:`int`, опционально.
 
-        :return: ответ FunPay.
-        :rtype: :class:`FunPayAPI.types.RaiseResponse`
+        :return: `True`
+        :rtype: :obj:`bool`
         """
-        if not self.is_initiated():
+        if not self.is_initiated:
             raise exceptions.AccountNotInitiatedError()
-        check = self.get_raise_modal(category_id, subcategory_id)
+        if not (category := self.get_category(category_id)):
+            raise Exception("Not Found")  # todo
 
-        if check.get("error") and check.get("msg") and "Подождите" in check.get("msg"):
-            wait_time = utils.parse_wait_time(check.get("msg"))
-            return types.RaiseResponse(False, wait_time, [], check)
-        elif check.get("error"):
-            # Если вернулся ответ с ошибкой и это не "Подождите n времени" - значит творится какая-то дичь.
-            return types.RaiseResponse(False, 10, [], check)
-        elif check.get("error") is not None and not check.get("error"):
-            # Если была всего 1 категория и FunPay ее поднял без отправки modal-окна
-            return types.RaiseResponse(True, 3600,
-                                       [self.get_subcategory(types.SubCategoryTypes.COMMON, subcategory_id)], check)
-        elif check.get("modal"):
-            # Если же появилась модалка,
-            # парсим все чекбоксы и отправляем запрос на поднятие всех категорий, кроме тех,
-            # которые в exclude.
-            parser = BeautifulSoup(check.get("modal"), "html.parser")
-            subcategories = []
-            checkboxes = parser.find_all("div", {"class": "checkbox"})
-            for cb in checkboxes:
-                subcategory_id = int(cb.find("input")["value"])
-                if exclude is None or subcategory_id not in exclude:
-                    subcategories.append(self.get_subcategory(types.SubCategoryTypes.COMMON, subcategory_id))
-
-            headers = {
-                "accept": "*/*",
-                "content-type": "application/x-www-form-urlencoded; charset=UTF-8",
-                "x-requested-with": "XMLHttpRequest"
-            }
-            payload = {
-                "game_id": category_id,
-                "node_id": subcategory_id,
-                "node_ids[]": [i.id for i in subcategories]
-            }
+        exclude = exclude or []
+        if subcategories:
+            subcats = []
+            for i in subcategories:
+                if isinstance(i, types.SubCategory):
+                    if i.type is types.SubCategoryTypes.COMMON and i.category.id == category.id and i.id not in exclude:
+                        subcats.append(i)
+                else:
+                    if not (subcat := category.get_subcategory(types.SubCategoryTypes.COMMON, i)):
+                        continue
+                    subcats.append(subcat)
+        else:
+            subcats = [i for i in category.get_subcategories() if i.type is types.SubCategoryTypes.COMMON and i.id not in exclude]
 
-            response = self.method("post", "https://funpay.com/lots/raise", headers, payload, raise_not_200=True)
-            json_response = response.json()
-            logger.debug(f"Ответ FunPay (поднятие категорий): {json_response}.")
-            if not json_response.get("error"):
-                return types.RaiseResponse(True, 3600, subcategories, json_response)
-            else:
-                return types.RaiseResponse(False, 10, [], json_response)
+        headers = {
+            "accept": "*/*",
+            "content-type": "application/x-www-form-urlencoded; charset=UTF-8",
+            "x-requested-with": "XMLHttpRequest"
+        }
+        payload = {
+            "game_id": category_id,
+            "node_id": subcats[0].id,
+            "node_ids[]": [i.id for i in subcats]
+        }
+
+        response = self.method("post", "lots/raise", headers, payload, raise_not_200=True)
+        json_response = response.json()
+        logger.debug(f"Ответ FunPay (поднятие категорий): {json_response}.")
+        if not json_response.get("error"):
+            return True
+        elif json_response.get("error") and json_response.get("msg") and "Подождите" in json_response.get("msg"):
+            wait_time = utils.parse_wait_time(json_response.get("msg"))
+            raise exceptions.RaiseError(response, category, json_response.get("MSG"), wait_time)
+        else:
+            raise exceptions.RaiseError(response, category, None, None)
 
     def get_user(self, user_id: int) -> types.UserProfile:
         """
         Парсит страницу пользователя.
 
         :param user_id: ID пользователя.
         :type user_id: :obj:`int`
 
         :return: объект профиля пользователя.
         :rtype: :class:`FunPayAPI.types.UserProfile`
         """
-        if not self.is_initiated():
+        if not self.is_initiated:
             raise exceptions.AccountNotInitiatedError()
 
-        headers = {
-            "accept": "*/*"
-        }
-
-        response = self.method("get", f"https://funpay.com/users/{user_id}/", headers, {}, raise_not_200=True)
+        response = self.method("get", f"users/{user_id}/", {"accept": "*/*"}, {}, raise_not_200=True)
         html_response = response.content.decode()
         parser = BeautifulSoup(html_response, "html.parser")
 
         username = parser.find("div", {"class": "user-link-name"})
         if not username:
             raise exceptions.UnauthorizedError(response)
 
@@ -657,20 +760,18 @@
 
         :param chat_id: ID чата.
         :type chat_id: :obj:`int`
 
         :return: объект чата.
         :rtype: :class:`FunPayAPI.types.Chat`
         """
-        if not self.is_initiated():
+        if not self.is_initiated:
             raise exceptions.AccountNotInitiatedError()
-        headers = {
-            "accept": "*/*"
-        }
-        response = self.method("get", f"https://funpay.com/chat/?node={chat_id}", headers, {}, raise_not_200=True)
+
+        response = self.method("get", f"chat/?node={chat_id}", {"accept": "*/*"}, {}, raise_not_200=True)
         html_response = response.content.decode()
         parser = BeautifulSoup(html_response, "html.parser")
         if (name := parser.find("div", {"class": "chat-header"}).find("div", {"class": "media-user-name"}).find("a").text) == "Чат":
             raise Exception("chat not found")  # todo
 
         if not (chat_panel := parser.find("div", {"class": "param-item chat-panel"})):
             text, link = None, None
@@ -687,20 +788,20 @@
 
         :param order_id: ID заказа.
         :type order_id: :obj:`str`
 
         :return: объекст заказа.
         :rtype: :class:`FunPayAPI.types.Order`
         """
-        if not self.is_initiated():
+        if not self.is_initiated:
             raise exceptions.AccountNotInitiatedError()
         headers = {
             "accept": "*/*"
         }
-        response = self.method("get", f"https://funpay.com/orders/{order_id}/", headers, {}, raise_not_200=True)
+        response = self.method("get", f"orders/{order_id}/", headers, {}, raise_not_200=True)
         html_response = response.content.decode()
         parser = BeautifulSoup(html_response, "html.parser")
         username = parser.find("div", {"class": "user-link-name"})
         if not username:
             raise exceptions.UnauthorizedError(response)
 
         if (span := parser.find("span", {"class": "text-warning"})) and span.text == "Возврат":
@@ -763,15 +864,18 @@
 
         order = types.Order(order_id, status, subcategory, short_description, full_description, sum_,
                             buyer_id, buyer_username, seller_id, seller_username, html_response, review)
         return order
 
     def get_sales(self, start_from: str | None = None, include_paid: bool = True, include_closed: bool = True,
                   include_refunded: bool = True, exclude_ids: list[str] | None = None,
-                  **filters) -> tuple[str | None, list[types.OrderShortcut]]:
+                  id: Optional[int] = None, buyer: Optional[str] = None,
+                  state: Optional[Literal["closed", "paid", "refunded"]] = None, game: Optional[int] = None,
+                  section: Optional[str] = None, server: Optional[int] = None,
+                  side: Optional[int] = None, **more_filters) -> tuple[str | None, list[types.OrderShortcut]]:
         """
         Получает и парсит список заказов со страницы https://funpay.com/orders/trade
 
         :param start_from: ID заказа, с которого начать список (ID заказа должен быть без '#'!).
         :type start_from: :obj:`str`
 
         :param include_paid: включить ли в список заказы, ожидающие выполнения?
@@ -782,41 +886,52 @@
 
         :param include_refunded: включить ли в список заказы, за которые запрошен возврат средств?
         :type include_refunded: :obj:`bool`, опционально
 
         :param exclude_ids: исключить заказы с ID из списка (ID заказа должен быть без '#'!).
         :type exclude_ids: :obj:`list` of :obj:`str`, опционально
 
-        :param filters: фильтры FunPay.\n
-            * id (:obj:`int`): ID заказа.\n
-            * buyer (:obj:`str`): никнейм покупателя.\n
-            * state (:obj:`str`): состояние заказа:\n
-
-                * paid - оплачен и ожидает выполнения.\n
-                * closed - выполнен.\n
-                * refunded - запрошен возврат средств.\n
+        :param id: ID заказа.
+        :type id: :obj:`int`, опционально
 
-            * game (:obj:`int`): ID игры.\n
-            * section (:obj:`str`): ID категории в формате <тип лота>-<ID категории>.\n
+        :param buyer: никнейм покупателя.
+        :type buyer: :obj:`str`, опционально
 
-                * lot - стандартный лот (например: lot-256)\n
-                * chip - игровая валюта (например: chip-4471)\n
+        :param state: статус заказа.
+        :type: :obj:`str` `paid`, `closed` or `refunded`, опционально
 
-            * server (:obj:`int`): ID сервера.\n
-            * side (:obj:`int`): ID стороны (платформы).
+        :param game: ID игры.
+        :type game: :obj:`int`, опционально
+
+        :param section: ID категории в формате `<тип лота>-<ID категории>`.\n
+            Типы лотов:\n
+            * `lot` - стандартный лот (например: `lot-256`)\n
+            * `chip` - игровая валюта (например: `chip-4471`)\n
+        :type section: :obj:`str`, опционально
+
+        :param server: ID сервера.
+        :type server: :obj:`int`, опционально
+
+        :param side: ID стороны (платформы).
+        :type side: :obj:`int`, опционально.
+
+        :param more_filters: доп. фильтры.
 
         :return: (ID след. заказа (для start_from), список заказов)
         :rtype: :obj:`tuple` (:obj:`str` or :obj:`None`, :obj:`list` of :class:`FunPayAPI.types.OrderShortcut`)
         """
-        if not self.is_initiated():
+        if not self.is_initiated:
             raise exceptions.AccountNotInitiatedError()
 
         exclude_ids = exclude_ids or []
-        link = "https://funpay.com/orders/trade?"
+        filters = {"id": id, "buyer": buyer, "state": state, "game": game, "section": section, "server": server,
+                   "side": side}
+        filters = {name: filters[name] for name in filters if filters[name]}
 
+        link = "https://funpay.com/orders/trade?"
         for name in filters:
             link += f"{name}={filters[name]}&"
         link = link[:-1]
 
         if start_from:
             filters["continue"] = start_from
 
@@ -825,18 +940,15 @@
 
         parser = BeautifulSoup(html_response, "html.parser")
         check_user = parser.find("div", {"class": "content-account content-account-login"})
         if check_user:
             raise exceptions.UnauthorizedError(response)
 
         next_order_id = parser.find("input", {"type": "hidden", "name": "continue"})
-        if not next_order_id:
-            next_order_id = None
-        else:
-            next_order_id = next_order_id.get("value")
+        next_order_id = next_order_id.get("value") if next_order_id else None
 
         order_divs = parser.find_all("a", {"class": "tc-item"})
         if not order_divs:
             return None, []
 
         sells = []
         for div in order_divs:
@@ -934,15 +1046,15 @@
 
         :param update: обновлять ли предварительно список чатов с помощью доп. запроса?
         :type update: :obj:`bool`, опционально
 
         :return: словарь с сохраненными чатами.
         :rtype: :obj:`dict` {:obj:`int`: :class:`FunPayAPi.types.ChatShortcut`}
         """
-        if not self.is_initiated():
+        if not self.is_initiated:
             raise exceptions.AccountNotInitiatedError()
         if update:
             chats = self.request_chats()
             self.add_chats(chats)
         return self.__saved_chats
 
     def get_chat_by_name(self, name: str, make_request: bool = False) -> types.ChatShortcut | None:
@@ -954,144 +1066,115 @@
 
         :param make_request: обновить ли сохраненные чаты, если чат не был найден?
         :type make_request: :obj:`bool`, опционально
 
         :return: объект чата или :obj:`None`, если чат не был найден.
         :rtype: :class:`FunPayAPI.types.ChatShortcut` or :obj:`None`
         """
-        if not self.is_initiated():
+        if not self.is_initiated:
             raise exceptions.AccountNotInitiatedError()
 
         for i in self.__saved_chats:
             if self.__saved_chats[i].name == name:
                 return self.__saved_chats[i]
 
         if make_request:
             self.add_chats(self.request_chats())
             return self.get_chat_by_name(name)
         else:
             return None
 
     def get_chat_by_id(self, chat_id: int, make_request: bool = False) -> types.ChatShortcut | None:
         """
-        Возвращает чат по его ID (если он сохранен).
+        Возвращает личный чат по его ID (если он сохранен).
 
         :param chat_id: ID чата.
         :type chat_id: :obj:`int`
 
         :param make_request: обновить ли сохраненные чаты, если чат не был найден?
         :type make_request: :obj:`bool`, опционально
 
         :return: объект чата или :obj:`None`, если чат не был найден.
         :rtype: :class:`FunPayAPI.types.ChatShortcut` or :obj:`None`
         """
-        if not self.is_initiated():
+        if not self.is_initiated:
             raise exceptions.AccountNotInitiatedError()
 
         if not make_request or chat_id in self.__saved_chats:
             return self.__saved_chats.get(chat_id)
 
         self.add_chats(self.request_chats())
         return self.get_chat_by_id(chat_id)
 
-    def get_lot_fields(self, lot_id: int, subcategory_id: int) -> types.LotFields:
+    def get_lot_fields(self, lot_id: int) -> types.LotFields:
         """
         Получает все поля лота.
 
         :param lot_id: ID лота.
         :type lot_id: :obj:`int`
 
-        :param subcategory_id: подкатегория лота.
-        :type subcategory_id: :obj:`int`
-
         :return: объект с полями лота.
         :rtype: :class:`FunPayAPI.types.LotFields`
         """
-        if not self.is_initiated():
+        if not self.is_initiated:
             raise exceptions.AccountNotInitiatedError()
         headers = {
             "accept": "*/*",
             "content-type": "application/json",
             "x-requested-with": "XMLHttpRequest",
         }
-        query = f"?tag={utils.random_tag()}&offer={lot_id}&node={subcategory_id}"
-        response = self.method("get", f"https://funpay.com/lots/offerEdit{query}", headers, {}, raise_not_200=True)
+        response = self.method("get", f"lots/offerEdit?offer={lot_id}", headers, {}, raise_not_200=True)
 
         json_response = response.json()
-        parser = BeautifulSoup(json_response["html"], "html.parser")
-
-        input_fields = parser.find_all("input")
-        text_fields = parser.find_all("textarea")
-        selection_fields = parser.find_all("select")
-        checkboxes = parser.find_all("input", {"type": "checkbox"}, checked=True)
-        result = {}
-
-        for field in input_fields:
-            name = field["name"]
-            if name in ["active", "deactivate_after_sale"]:
-                continue
-            else:
-                result[name] = field.get("value") or ""
-
-        for field in text_fields:
-            name = field["name"]
-            result[name] = field.text or ""
-
-        for field in selection_fields:
-            name = field["name"]
-            result[name] = field.find("option", selected=True)["value"]
-
-        for field in checkboxes:
-            name = field["name"]
-            if name == "active":
-                result[name] = "on"
-            elif name == "deactivate_after_sale":
-                result["deactivate_after_sale[]"] = "on"
+        bs = BeautifulSoup(json_response["html"], "html.parser")
 
-        if "deactivate_after_sale[]" not in result:
-            result["deactivate_after_sale"] = ""
-
-        return types.LotFields(lot_id, subcategory_id, result)
+        result = {"active": "", "deactivate_after_sale": ""}
+        result.update({field["name"]: field.get("value") or "" for field in bs.find_all("input")
+                       if field["name"] not in ["active", "deactivate_after_sale"]})
+        result.update({field["name"]: field.text or "" for field in bs.find_all("textarea")})
+        result.update({field["name"]: field.find("option", selected=True)["value"] for field in bs.find_all("select")})
+        result.update({field["name"]: "on" for field in bs.find_all("input", {"type": "checkbox"}, checked=True)})
+        return types.LotFields(lot_id, result)
 
     def save_lot(self, lot_fields: types.LotFields):
         """
         Сохраняет лот на FunPay.
 
         :param lot_fields: объект с полями лота.
         :type lot_fields: :class:`FunPayAPI.types.LotFields`
         """
-        if not self.is_initiated():
+        if not self.is_initiated:
             raise exceptions.AccountNotInitiatedError()
         headers = {
             "accept": "*/*",
             "content-type": "application/x-www-form-urlencoded; charset=UTF-8",
             "x-requested-with": "XMLHttpRequest",
         }
-        fields = lot_fields.renew_fields().get_fields()
+        fields = lot_fields.renew_fields().fields
         fields["location"] = "trade"
 
-        response = self.method("post", "https://funpay.com/lots/offerSave", headers, fields, raise_not_200=True)
+        response = self.method("post", "lots/offerSave", headers, fields, raise_not_200=True)
         json_response = response.json()
         if json_response.get("error"):
-            raise exceptions.LotSavingError(response, json_response.get("error"), lot_fields.lot_id,
-                                            lot_fields.subcategory_id)
+            raise exceptions.LotSavingError(response, json_response.get("error"), lot_fields.lot_id)
 
     def get_category(self, category_id: int) -> types.Category | None:
         """
         Возвращает объект категории (игры).
 
         :param category_id: ID категории (игры).
         :type category_id: :obj:`int`
 
         :return: объект категории (игры) или :obj:`None`, если категория не была найдена.
         :rtype: :class:`FunPayAPI.types.Category` or :obj:`None`
         """
         return self.__sorted_categories.get(category_id)
 
-    def get_categories(self) -> list[types.Category]:
+    @property
+    def categories(self) -> list[types.Category]:
         """
         Возвращает все категории (игры) FunPay (парсятся при первом выполнении метода :meth:`FunPayAPI.account.Account.get`).
 
         :return: все категории (игры) FunPay.
         :rtype: :obj:`list` of :class:`FunPayAPI.types.Category`
         """
         return self.__categories
@@ -1118,33 +1201,35 @@
         :type subcategory_id: :obj:`int`
 
         :return: объект подкатегории или :obj:`None`, если подкатегория не была найдена.
         :rtype: :class:`FunPayAPI.types.SubCategory` or :obj:`None`
         """
         return self.__sorted_subcategories[subcategory_type].get(subcategory_id)
 
-    def get_subcategories(self) -> list[types.SubCategory]:
+    @property
+    def subcategories(self) -> list[types.SubCategory]:
         """
         Возвращает все подкатегории FunPay (парсятся при первом выполнении метода Account.get).
 
         :return: все подкатегории FunPay.
         :rtype: :obj:`list` of :class:`FunPayAPI.types.SubCategory`
         """
         return self.__subcategories
 
-    def get_sorted_subcategories(self) -> dict[types.SubCategoryTypes, dict[int | str, types.SubCategory]]:
+    def get_sorted_subcategories(self) -> dict[types.SubCategoryTypes, dict[int, types.SubCategory]]:
         """
         Возвращает все подкатегории FunPay в виде словаря {тип подкатегории: {ID: подкатегория}}
         (парсятся при первом выполнении метода Account.get).
 
         :return: все подкатегории FunPay в виде словаря {тип подкатегории: {ID: подкатегория}}
-        :rtype: :obj:`dict` {:class:`FunPayAPI.common.enums.SubCategoryTypes`: :obj:`dict` {:obj:`int` or :obj:`str`: :class:`FunPayAPI.types.SubCategory`}}
+        :rtype: :obj:`dict` {:class:`FunPayAPI.common.enums.SubCategoryTypes`: :obj:`dict` {:obj:`int` :class:`FunPayAPI.types.SubCategory`}}
         """
         return self.__sorted_subcategories
 
+    @property
     def is_initiated(self) -> bool:
         """
         Инициализирован ли класс :class:`FunPayAPI.account.Account` с помощью метода :meth:`FunPayAPI.account.Account.get`?
 
         :return: :obj:`True`, если да, :obj:`False`, если нет.
         :rtype: :obj:`bool`
         """
@@ -1166,16 +1251,16 @@
         if not games_divs:
             return
 
         for i in games_divs:
             game_id = int(i.find("div", {"class": "game-title"}).get("data-id"))
             game_title = i.find("a").text
             game_obj = types.Category(game_id, game_title)
-            subcategories_divs = i.find_all("li")
 
+            subcategories_divs = i.find_all("li")
             for j in subcategories_divs:
                 subcategory_name = j.find("a").text
                 link = j.find("a").get("href")
                 subcategory_type = types.SubCategoryTypes.CURRENCY if "chips" in link else types.SubCategoryTypes.COMMON
                 subcategory_id = int(link.split("/")[-2])
 
                 subcategory_obj = types.SubCategory(subcategory_id, subcategory_name, subcategory_type, game_obj)
@@ -1183,41 +1268,39 @@
                 self.__subcategories.append(subcategory_obj)
                 self.__sorted_subcategories[subcategory_type][subcategory_id] = subcategory_obj
 
             self.__categories.append(game_obj)
             self.__sorted_categories[game_id] = game_obj
 
     def __parse_messages(self, json_messages: dict, chat_id: int | str,
-                         interlocutor_id: int, interlocutor_username: str | None,
+                         interlocutor_id: Optional[int] = None, interlocutor_username: Optional[str] = None,
                          from_id: int = 0) -> list[types.Message]:
         messages = []
-
-        ids = {
-            self.id: self.username,
-            0: "FunPay",
-            interlocutor_id: interlocutor_username
-        }
+        ids = {self.id: self.username, 0: "FunPay"}
+        if interlocutor_id is not None:
+            ids[interlocutor_id] = interlocutor_username
 
         for i in json_messages:
             if i["id"] < from_id:
                 continue
             author_id = i["author"]
             parser = BeautifulSoup(i["html"], "html.parser")
             # Если ник написавшего неизвестен, но он есть в HTML-коде сообщения
-            if not ids.get(author_id) and (author_div := parser.find("div", {"class": "media-user-name"})):
+            if ids.get(author_id) is None and (author_div := parser.find("div", {"class": "media-user-name"})):
                 author = author_div.find("a").text.strip()
                 ids[author_id] = author
-                if author_id == interlocutor_id and not interlocutor_username:
+                if isinstance(chat_id, int) and author_id == interlocutor_id and not interlocutor_username:
                     interlocutor_username = author
                     ids[interlocutor_id] = interlocutor_username
 
-            if image_link := parser.find("a", {"class": "chat-img-link"}):
+            if isinstance(chat_id, int) and (image_link := parser.find("a", {"class": "chat-img-link"})):
                 image_link = image_link.get("href")
                 message_text = None
             else:
+                image_link = None
                 if author_id == 0:
                     message_text = parser.find("div", {"class": "alert alert-with-icon alert-info"}).text.strip()
                 else:
                     message_text = parser.find("div", {"class": "message-text"}).text
 
             message_obj = types.Message(i["id"], message_text, chat_id, interlocutor_username,
                                         None, author_id, i["html"], image_link, determine_msg_type=False)
@@ -1230,9 +1313,8 @@
         # todo
         debug_text = ""
         for i in messages:
             i.author = ids.get(i.author_id)
             i.chat_name = interlocutor_username
             debug_text += f"{i.author} | {i.author_id} | {str(i)[:20]} /\\"
         logger.debug(debug_text)
-
         return messages
```

### Comparing `FunPayAPI-1.0.6/FunPayAPI/common/enums.py` & `FunPayAPI-1.0.7/FunPayAPI/common/enums.py`

 * *Files 6% similar despite different names*

```diff
@@ -114,17 +114,21 @@
 
 class Wallet(Enum):
     """
     В данном классе перечислены все кошельки для вывода средств с баланса FunPay.
     """
     QIWI = 0
     """Qiwi кошелек."""
-    BINANCE = 2
+    BINANCE = 1
     """Binance Pay."""
-    TRC = 3
+    TRC = 2
     """USDT TRC20."""
-    CARD = 4
-    """Банковская карта."""
-    WEBMONEY = 5
+    CARD_RUB = 3
+    """Рублевая банковская карта."""
+    CARD_USD = 4
+    """Долларовая банковская карта."""
+    CARD_EUR = 5
+    """Евро банковская карта."""
+    WEBMONEY = 6
     """WebMoney WMZ."""
-    YOUMONEY = 6
+    YOUMONEY = 7
     """ЮMoney."""
```

### Comparing `FunPayAPI-1.0.6/FunPayAPI/common/exceptions.py` & `FunPayAPI-1.0.7/FunPayAPI/common/exceptions.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 В данном модуле описаны все кастомные исключения, используемые в пакете FunPayAPI.
 """
 import requests
+from .. import types
 
 
 class AccountNotInitiatedError(Exception):
     """
     Исключение, которое возбуждается, если предпринята попытка вызвать метод класса :class:`FunPayAPI.account.Account`
     без предварительного получения данных аккаунта с помощью метода :meth:`FunPayAPI.account.Account.get`.
     """
@@ -55,14 +56,43 @@
     def __init__(self, response):
         super(UnauthorizedError, self).__init__(response)
 
     def short_str(self):
         return "Не авторизирован (возможно, введен неверный golden_key?)."
 
 
+class WithdrawError(RequestFailedError):
+    """
+    Исключение, которое возбуждается, если произошла ошибка при попытке вывести средства с аккаунта.
+    """
+    def __init__(self, response, error_message: str | None):
+        super(WithdrawError, self).__init__(response)
+        self.error_message = error_message
+        if not self.error_message:
+            self.log_response = True
+
+    def short_str(self):
+        return f"Произошла ошибка при выводе средств с аккаунта{f': {self.error_message}' if self.error_message else '.'}"
+
+
+class RaiseError(RequestFailedError):
+    """
+    Исключение, которое возбуждается, если произошла ошибка при попытке поднять лоты.
+    """
+    def __init__(self, response, category: types.Category, error_message: str | None, wait_time: int | None):
+        super(RaiseError, self).__init__(response)
+        self.category = category
+        self.error_message = error_message
+        self.wait_time = wait_time
+
+    def short_str(self):
+        return f"Не удалось поднять лоты категории \"{self.category.name}\"" \
+               f"{f': {self.error_message}' if self.error_message else '.'}"
+
+
 class ImageUploadError(RequestFailedError):
     """
     Исключение, которое возбуждается, если произошла ошибка при выгрузке изображения.
     """
     def __init__(self, response: requests.Response, error_message: str | None):
         super(ImageUploadError, self).__init__(response)
         self.error_message = error_message
@@ -106,19 +136,18 @@
                f"{f': {self.error_message}' if self.error_message else '.'}"
 
 
 class LotSavingError(RequestFailedError):
     """
     Исключение, которое возбуждается, если при сохранении лота произошла ошибка.
     """
-    def __init__(self, response: requests.Response, error_message: str | None, lot_id: int, subcategory_id: int | str):
+    def __init__(self, response: requests.Response, error_message: str | None, lot_id: int):
         super(LotSavingError, self).__init__(response)
         self.error_message = error_message
         self.lot_id = lot_id
-        self.subcategory_id = subcategory_id
         if not self.error_message:
             self.log_response = True
 
     def short_str(self):
         return f"Не удалось сохранить лот {self.lot_id}" \
                f"{f': {self.error_message}' if self.error_message else '.'}"
```

### Comparing `FunPayAPI-1.0.6/FunPayAPI/common/utils.py` & `FunPayAPI-1.0.7/FunPayAPI/common/utils.py`

 * *Files identical despite different names*

### Comparing `FunPayAPI-1.0.6/FunPayAPI/types.py` & `FunPayAPI-1.0.7/FunPayAPI/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -481,25 +481,20 @@
 class LotFields:
     """
     Класс, описывающий поля лота со страницы редактирования лота.
 
     :param lot_id: ID лота.
     :type lot_id: :obj:`int`
 
-    :param subcategory_id: ID категории (игры), к которой относится лот.
-    :type subcategory_id: :obj:`int`
-
     :param fields: словарь с полями.
     :type fields: :obj:`dict`
     """
-    def __init__(self, lot_id: int, subcategory_id: int, fields: dict):
+    def __init__(self, lot_id: int, fields: dict):
         self.lot_id: int = lot_id
         """ID лота."""
-        self.subcategory_id: int = subcategory_id
-        """ID подкатегории, к которой относится лот."""
         self.__fields: dict = fields
         """Поля лота."""
 
         self.title_ru: str = self.__fields.get("fields[summary][ru]")
         """Русское краткое описание (название) лота."""
         self.title_en: str = self.__fields.get("fields[summary][en]")
         """Английское краткое описание (название) лота."""
@@ -512,15 +507,16 @@
         self.price: float = float(i) if (i := self.__fields.get("price")) else None
         """Цена за 1шт."""
         self.active: bool = "active" in self.__fields
         """Активен ли лот."""
         self.deactivate_after_sale: bool = "deactivate_after_sale[]" in self.__fields
         """Деактивировать ли лот после продажи."""
 
-    def get_fields(self) -> dict[str, str]:
+    @property
+    def fields(self) -> dict[str, str]:
         """
         Возвращает все поля лота в виде словаря.
 
         :return: все поля лота в виде словаря.
         :rtype: :obj:`dict` {:obj:`str`: :obj:`str`}
         """
         return self.__fields
@@ -528,16 +524,15 @@
     def edit_fields(self, fields: dict[str, str]):
         """
         Редактирует переданные поля лота.
 
         :param fields: поля лота, которые нужно заменить, и их значения.
         :type fields: obj:`dict` {:obj:`str`: :obj:`str`}
         """
-        for i in fields:
-            self.__fields[i] = fields[i]
+        self.__fields.update(fields)
 
     def set_fields(self, fields: dict):
         """
         Сбрасывает текущие поля лота и устанавливает переданные.
         !НЕ РЕДАКТИРУЕТ СВОЙСТВА ЭКЗЕМЛПЯРА!
 
         :param fields: поля лота.
@@ -555,34 +550,17 @@
         :rtype: :class:`FunPayAPI.types.LotFields`
         """
         self.__fields["fields[summary][ru]"] = self.title_ru
         self.__fields["fields[summary][en]"] = self.title_en
         self.__fields["fields[desc][ru]"] = self.description_ru
         self.__fields["fields[desc][en]"] = self.description_en
         self.__fields["price"] = str(self.price) if self.price is not None else ""
-        if self.amount is not None:
-            self.__fields["amount"] = str(self.amount)
-        else:
-            if "amount" in self.__fields:
-                self.__fields.pop("amount")
-
-        if self.active:
-            self.__fields["active"] = "on"
-        else:
-            if "active" in self.__fields:
-                self.__fields.pop("active")
-
-        if self.deactivate_after_sale:
-            if "deactivate_after_sale" in self.__fields:
-                self.__fields.pop("deactivate_after_sale")
-            self.__fields["deactivate_after_sale[]"] = "on"
-        else:
-            if "deactivate_after_sale[]" in self.__fields:
-                self.__fields.pop("deactivate_after_sale[]")
-            self.__fields["deactivate_after_sale"] = ""
+        self.__fields["deactivate_after_sale"] = "on" if self.deactivate_after_sale else ""
+        self.__fields["active"] = "on" if self.active else ""
+        self.__fields["amount"] = self.amount if self.amount is not None else ""
         return self
 
 
 class LotShortcut:
     """
     Данный класс представляет виджет лота.
 
@@ -813,32 +791,40 @@
         """ID заказа, к которому относится отзыв."""
         self.author: str | None = author
         """Автор отзыва."""
         self.author_id: int | None = author_id
         """ID автора отзыва."""
 
 
-class RaiseResponse:
+class Balance:
     """
-    Данный класс представляет ответ FunPay на запрос о поднятии лотов.
+    Данный класс представляет информацию о балансе аккаунта.
+
+    :param total_rub: общий рублёвый баланс.
+    :type total_rub: :obj:`float`
 
-    :param complete: удалось ли поднять лоты?
-    :type complete: :obj:`bool`
+    :param available_rub: доступный к выводу рублёвый баланс.
+    :type available_rub: :obj:`float`
 
-    :param wait: примерное время ожидания до следующего поднятия.
-    :type wait: :obj:`int`
+    :param total_usd: общий долларовый баланс.
+    :type total_usd: :obj:`float`
 
-    :param raised_subcategories: список объектов поднятых подкатегорий.
-    :type raised_subcategories: :obj:`list` of :class:`FunPayAPI.types.SubCategory`
+    :param available_usd: доступный к выводу долларовый баланс.
+    :type available_usd: :obj:`float`
 
-    :param funpay_response: полный ответ Funpay.
-    :type funpay_response: :obj:`dict`
+    :param total_eur: общий евро баланс.
+    :param available_eur: :obj:`float`
     """
-    def __init__(self, complete: bool, wait: int, raised_subcategories: list[SubCategory], funpay_response: dict):
-        self.complete: bool = complete
-        """Удалось ли поднять лоты."""
-        self.wait: int = wait
-        """Примерное время ожидания до след. поднятия."""
-        self.raised_subcategories: list[SubCategory] = raised_subcategories
-        """Список объектов поднятых подкатегорий."""
-        self.funpay_response: dict = funpay_response
-        """Полный ответ FunPay."""
+    def __init__(self, total_rub: float, available_rub: float, total_usd: float, available_usd: float,
+                 total_eur: float, available_eur: float):
+        self.total_rub: float = total_rub
+        """Общий рублёвый баланс."""
+        self.available_rub: float = available_rub
+        """Доступный к выводу рублёвый баланс."""
+        self.total_usd: float = total_usd
+        """Общий долларовый баланс."""
+        self.available_usd: float = available_usd
+        """Доступный к выводу долларовый баланс."""
+        self.total_eur: float = total_eur
+        """Общий евро баланс."""
+        self.available_eur: float = available_eur
+        """Доступный к выводу евро баланс."""
```

### Comparing `FunPayAPI-1.0.6/FunPayAPI/updater/events.py` & `FunPayAPI-1.0.7/FunPayAPI/updater/events.py`

 * *Files identical despite different names*

### Comparing `FunPayAPI-1.0.6/FunPayAPI/updater/runner.py` & `FunPayAPI-1.0.7/FunPayAPI/updater/runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         Из событий, связанных с заказами, будет возвращаться только
         :class:`FunPayAPI.updater.events.OrdersListChangedEvent`.
     :type disabled_order_requests: :obj:`bool`, опционально
     """
     def __init__(self, account: Account, disable_message_requests: bool = False,
                  disabled_order_requests: bool = False):
         # todo добавить события и исключение событий о новых покупках (не продажах!)
-        if not account.is_initiated():
+        if not account.is_initiated:
             raise exceptions.AccountNotInitiatedError()
         if account.runner:
             raise Exception("К аккаунту уже привязан Runner!")  # todo
 
         self.make_msg_requests: bool = False if disable_message_requests else True
         """Делать ли доп. запросы для получения всех новых сообщений изменившихся чатов?"""
         self.make_order_requests: bool = False if disabled_order_requests else True
@@ -151,15 +151,18 @@
         self.__last_msg_event_tag = obj.get("tag")
         parser = BeautifulSoup(obj["data"]["html"], "html.parser")
         chats = parser.find_all("a", {"class": "contact-item"})
 
         # Получаем все изменившиеся чаты
         for msg in chats:
             chat_id = int(msg["data-id"])
-            last_msg_text = msg.find("div", {"class": "contact-item-message"}).text
+            last_msg_text = msg.find("div", {"class": "contact-item-message"})
+            if not last_msg_text:
+                continue
+            last_msg_text = last_msg_text.text
             if self.last_messages.get(chat_id) == last_msg_text:
                 continue
             unread = True if "unread" in msg.get("class") else False
             chat_with = msg.find("div", {"class": "media-user-name"}).text
             chat_obj = types.ChatShortcut(chat_id, chat_with, last_msg_text, unread, str(msg))
             self.account.add_chats([chat_obj])
             self.last_messages[chat_id] = last_msg_text
```

### Comparing `FunPayAPI-1.0.6/FunPayAPI.egg-info/PKG-INFO` & `FunPayAPI-1.0.7/FunPayAPI.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FunPayAPI
-Version: 1.0.6
+Version: 1.0.7
 Summary: Прослойка между FunPayAPI и клиентом.
 Home-page: https://github.com/woopertail/FunPayAPI
 Author: Woopertail
 Author-email: woopertail@gmail.com
 License: GPL2
 Keywords: funpay bot api tools
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: FunPayAPI Version: 1.0.6 Summary:
+Metadata-Version: 2.1 Name: FunPayAPI Version: 1.0.7 Summary:
 ÐÑÐ¾ÑÐ»Ð¾Ð¹ÐºÐ° Ð¼ÐµÐ¶Ð´Ñ FunPayAPI Ð¸ ÐºÐ»Ð¸ÐµÐ½ÑÐ¾Ð¼. Home-page: https:/
 /github.com/woopertail/FunPayAPI Author: Woopertail Author-email:
 woopertail@gmail.com License: GPL2 Keywords: funpay bot api tools Platform:
 UNKNOWN Classifier: Development Status :: 5 - Production/Stable Classifier:
 Programming Language :: Python :: 3 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Description-Content-Type: text/markdown License-File: LICENSE [https://
```

### Comparing `FunPayAPI-1.0.6/LICENSE` & `FunPayAPI-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `FunPayAPI-1.0.6/PKG-INFO` & `FunPayAPI-1.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FunPayAPI
-Version: 1.0.6
+Version: 1.0.7
 Summary: Прослойка между FunPayAPI и клиентом.
 Home-page: https://github.com/woopertail/FunPayAPI
 Author: Woopertail
 Author-email: woopertail@gmail.com
 License: GPL2
 Keywords: funpay bot api tools
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: FunPayAPI Version: 1.0.6 Summary:
+Metadata-Version: 2.1 Name: FunPayAPI Version: 1.0.7 Summary:
 ÐÑÐ¾ÑÐ»Ð¾Ð¹ÐºÐ° Ð¼ÐµÐ¶Ð´Ñ FunPayAPI Ð¸ ÐºÐ»Ð¸ÐµÐ½ÑÐ¾Ð¼. Home-page: https:/
 /github.com/woopertail/FunPayAPI Author: Woopertail Author-email:
 woopertail@gmail.com License: GPL2 Keywords: funpay bot api tools Platform:
 UNKNOWN Classifier: Development Status :: 5 - Production/Stable Classifier:
 Programming Language :: Python :: 3 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Description-Content-Type: text/markdown License-File: LICENSE [https://
```

### Comparing `FunPayAPI-1.0.6/README.md` & `FunPayAPI-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `FunPayAPI-1.0.6/setup.py` & `FunPayAPI-1.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_desc = f.read()
 
 
 setup(name='FunPayAPI',
-      version="1.0.6",
+      version="1.0.7",
       description='Прослойка между FunPayAPI и клиентом.',
       long_description=long_desc,
       long_description_content_type="text/markdown",
       author='Woopertail',
       author_email='woopertail@gmail.com',
       url='https://github.com/woopertail/FunPayAPI',
       packages=find_packages("."),
```

