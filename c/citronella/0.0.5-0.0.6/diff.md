# Comparing `tmp/citronella-0.0.5.tar.gz` & `tmp/citronella-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citronella-0.0.5.tar", last modified: Thu Mar  2 02:52:47 2023, max compression
+gzip compressed data, was "citronella-0.0.6.tar", last modified: Mon May 15 17:01:54 2023, max compression
```

## Comparing `citronella-0.0.5.tar` & `citronella-0.0.6.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 noodle    (1000) wheel      (998)        0 2023-03-02 02:52:47.391478 citronella-0.0.5/
--rw-r--r--   0 noodle    (1000) wheel      (998)     8712 2023-03-02 02:52:47.391478 citronella-0.0.5/PKG-INFO
--rw-r--r--   0 noodle    (1000) wheel      (998)     7898 2023-03-02 02:50:25.000000 citronella-0.0.5/README.md
--rw-r--r--   0 noodle    (1000) wheel      (998)       38 2023-03-02 02:52:47.391478 citronella-0.0.5/setup.cfg
--rw-r--r--   0 noodle    (1000) wheel      (998)     1233 2023-02-28 18:06:49.000000 citronella-0.0.5/setup.py
-drwxr-xr-x   0 noodle    (1000) wheel      (998)        0 2023-03-02 02:52:47.391478 citronella-0.0.5/src/
-drwxr-xr-x   0 noodle    (1000) wheel      (998)        0 2023-03-02 02:52:47.391478 citronella-0.0.5/src/citronella/
--rw-r--r--   0 noodle    (1000) wheel      (998)     1241 2023-03-01 18:19:27.000000 citronella-0.0.5/src/citronella/__init__.py
--rw-r--r--   0 noodle    (1000) wheel      (998)     1426 2023-03-01 18:17:50.000000 citronella-0.0.5/src/citronella/logger.py
--rw-r--r--   0 noodle    (1000) wheel      (998)     1912 2023-03-01 18:17:41.000000 citronella-0.0.5/src/citronella/page_decorator.py
--rw-r--r--   0 noodle    (1000) wheel      (998)     1623 2023-03-01 18:18:04.000000 citronella-0.0.5/src/citronella/page_tab.py
--rw-r--r--   0 noodle    (1000) wheel      (998)     1119 2023-03-01 18:18:14.000000 citronella-0.0.5/src/citronella/placeholder_page.py
--rw-r--r--   0 noodle    (1000) wheel      (998)     1964 2023-03-01 18:18:27.000000 citronella-0.0.5/src/citronella/ui.py
--rw-r--r--   0 noodle    (1000) wheel      (998)     5292 2023-03-01 18:18:43.000000 citronella-0.0.5/src/citronella/web_page.py
--rw-r--r--   0 noodle    (1000) wheel      (998)     6325 2023-03-01 18:18:55.000000 citronella-0.0.5/src/citronella/web_ui.py
-drwxr-xr-x   0 noodle    (1000) wheel      (998)        0 2023-03-02 02:52:47.391478 citronella-0.0.5/src/citronella.egg-info/
--rw-r--r--   0 noodle    (1000) wheel      (998)     8712 2023-03-02 02:52:47.000000 citronella-0.0.5/src/citronella.egg-info/PKG-INFO
--rw-r--r--   0 noodle    (1000) wheel      (998)      456 2023-03-02 02:52:47.000000 citronella-0.0.5/src/citronella.egg-info/SOURCES.txt
--rw-r--r--   0 noodle    (1000) wheel      (998)        1 2023-03-02 02:52:47.000000 citronella-0.0.5/src/citronella.egg-info/dependency_links.txt
--rw-r--r--   0 noodle    (1000) wheel      (998)        9 2023-03-02 02:52:47.000000 citronella-0.0.5/src/citronella.egg-info/requires.txt
--rw-r--r--   0 noodle    (1000) wheel      (998)       11 2023-03-02 02:52:47.000000 citronella-0.0.5/src/citronella.egg-info/top_level.txt
-drwxr-xr-x   0 noodle    (1000) wheel      (998)        0 2023-03-02 02:52:47.391478 citronella-0.0.5/test/
--rw-r--r--   0 noodle    (1000) wheel      (998)     1900 2023-02-26 21:21:38.000000 citronella-0.0.5/test/test_navigation_menu.py
+drwxr-xr-x   0 noodle    (1000) wheel      (998)        0 2023-05-15 17:01:54.140217 citronella-0.0.6/
+-rw-r--r--   0 noodle    (1000) wheel      (998)     9586 2023-05-15 17:01:54.140217 citronella-0.0.6/PKG-INFO
+-rw-r--r--   0 noodle    (1000) wheel      (998)     8748 2023-05-15 16:54:12.000000 citronella-0.0.6/README.md
+-rw-r--r--   0 noodle    (1000) wheel      (998)       38 2023-05-15 17:01:54.140217 citronella-0.0.6/setup.cfg
+-rw-r--r--   0 noodle    (1000) wheel      (998)     1257 2023-03-11 12:44:04.000000 citronella-0.0.6/setup.py
+drwxr-xr-x   0 noodle    (1000) wheel      (998)        0 2023-05-15 17:01:54.140217 citronella-0.0.6/src/
+drwxr-xr-x   0 noodle    (1000) wheel      (998)        0 2023-05-15 17:01:54.140217 citronella-0.0.6/src/citronella/
+-rw-r--r--   0 noodle    (1000) wheel      (998)     1186 2023-05-15 16:59:51.000000 citronella-0.0.6/src/citronella/__init__.py
+-rw-r--r--   0 noodle    (1000) wheel      (998)     1535 2023-05-15 16:59:51.000000 citronella-0.0.6/src/citronella/deprecated.py
+-rw-r--r--   0 noodle    (1000) wheel      (998)     1426 2023-05-15 16:59:51.000000 citronella-0.0.6/src/citronella/logger.py
+-rw-r--r--   0 noodle    (1000) wheel      (998)     2210 2023-05-15 16:59:51.000000 citronella-0.0.6/src/citronella/page_decorator.py
+-rw-r--r--   0 noodle    (1000) wheel      (998)     1452 2023-05-15 16:59:51.000000 citronella-0.0.6/src/citronella/page_validator.py
+-rw-r--r--   0 noodle    (1000) wheel      (998)     1119 2023-05-15 16:59:51.000000 citronella-0.0.6/src/citronella/placeholder_page.py
+-rw-r--r--   0 noodle    (1000) wheel      (998)     1527 2023-05-15 16:59:51.000000 citronella-0.0.6/src/citronella/ui.py
+-rw-r--r--   0 noodle    (1000) wheel      (998)     5136 2023-05-15 16:59:51.000000 citronella-0.0.6/src/citronella/web_page.py
+-rw-r--r--   0 noodle    (1000) wheel      (998)     5419 2023-05-15 16:59:51.000000 citronella-0.0.6/src/citronella/web_ui.py
+drwxr-xr-x   0 noodle    (1000) wheel      (998)        0 2023-05-15 17:01:54.140217 citronella-0.0.6/src/citronella.egg-info/
+-rw-r--r--   0 noodle    (1000) wheel      (998)     9586 2023-05-15 17:01:54.000000 citronella-0.0.6/src/citronella.egg-info/PKG-INFO
+-rw-r--r--   0 noodle    (1000) wheel      (998)      491 2023-05-15 17:01:54.000000 citronella-0.0.6/src/citronella.egg-info/SOURCES.txt
+-rw-r--r--   0 noodle    (1000) wheel      (998)        1 2023-05-15 17:01:54.000000 citronella-0.0.6/src/citronella.egg-info/dependency_links.txt
+-rw-r--r--   0 noodle    (1000) wheel      (998)        9 2023-05-15 17:01:54.000000 citronella-0.0.6/src/citronella.egg-info/requires.txt
+-rw-r--r--   0 noodle    (1000) wheel      (998)       11 2023-05-15 17:01:54.000000 citronella-0.0.6/src/citronella.egg-info/top_level.txt
+drwxr-xr-x   0 noodle    (1000) wheel      (998)        0 2023-05-15 17:01:54.140217 citronella-0.0.6/test/
+-rw-r--r--   0 noodle    (1000) wheel      (998)     1900 2023-04-29 22:47:14.000000 citronella-0.0.6/test/test_navigation_menu.py
```

### Comparing `citronella-0.0.5/PKG-INFO` & `citronella-0.0.6/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: citronella
-Version: 0.0.5
+Version: 0.0.6
 Summary: Webdriver Extension with Page Object Wrapper
-Home-page: https://github.com/heyclore/citronella
+Home-page: https://github.com/heyclore/citronella/tree/main/python#readme
 Author: heyclore
 Author-email: cloore@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/heyclore/citronella/tree/main/python
 Keywords: test,unittest,pytest,webdriver,appium,selenium
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -27,107 +27,94 @@
 webdriver extension with a page object wrapper.
 
 ![alt terminal](https://github.com/heyclore/citronella/blob/main/python/screenshot/terminal.png?raw=true)
 ![alt pytest-html](https://github.com/heyclore/citronella/blob/main/python/screenshot/pytest_html.png?raw=true)
 ![alt github-action](https://github.com/heyclore/citronella/blob/main/python/screenshot/github_action.png?raw=true)
 
 ## Example Tests
-Even though this module is mainly designed for the page object model, it can also be used without it for quick prototyping or mockups, etc.
-```python
-from selenium import webdriver
-from selenium.webdriver.common.by import By
-from citronella import WebPage
-
-
-driver = webdriver.Chrome()
-
-web = WebPage(driver, webdriver_wait=20, logger=False)
-web.driver.get('https://pypi.org/')
-
-web.locate(By.ID, 'search').get_element().send_keys('citronella')
-web.locate(By.XPATH, '//button[@type="submit"]/i').get_element().click()
-
-elements = web.locate(By.XPATH, '//span[@class="package-snippet__name"]')
-if elements.ec_visibility_of_all_elements_located():
-    results = elements.get_elements()
-    text_lists = [x.text for x in results]
-```
-
-
 
 ### Selenium
 
 ```python
 import pytest
-from Pages.home.home_page import HomePage
+from Pages.contents_page import ContentsPage
 
 
 class TestNavigationMenu:
 
     def test_help_page(self, web):
         web.driver.get('https://pypi.org/')
-        web.page_object(HomePage)
+        web.page = ContentsPage
 
-        web.page.help_button.click()
+        web.page.home_page.help_button.click()
         assert 'Help' in web.driver.title
 
     def test_sponsors_page(self, web):
-        web.page.sponsors_button.click()
+        web.page.help_page.sponsors_button.click()
         assert 'Sponsors' in web.driver.title
 
     def test_login_page(self, web):
-        web.page.login_button.click()
+        web.page.sponsors_page.login_button.click()
         assert 'Log' in web.driver.title
 
     def test_register_page(self, web):
-        web.page.register_button.click()
+        web.page.login_page.register_button.click()
         assert 'Create' in web.driver.title
 ```
 
 ### Appium
 
 ```python
 import pytest
-from Pages.api_demos_page import ApiDemosPage
+from Pages.contents_page import ContentsPage
 
 
-class TestNavigationMenu:
+class TestInput:
+
+    def test_input(self, web):
+        web.page = ContentsPage
+        web.page.home_page.gallery_button.click()
+        web.page.gallery_page.text_input.send_keys('citronella')
+        web.page.gallery_page.add_button.click()
+        elements = web.page.gallery_page.text_lists.get_elements()
+        assert 'citronella' in [x.text for x in elements]
+```
+
+Even though this module is mainly designed for the page object model, it can also be used without it for quick prototyping or mockups, etc.
+```python
+from selenium import webdriver
+from selenium.webdriver.common.by import By
+from citronella import WebPage
 
-    def test_accessibility_page(self, web):
-        web.page_object(ApiDemosPage)
 
-        web.page.accessibility_button.click()
-        assert web.page.accessibility_node_provider_button.get_element().is_visible()
+driver = webdriver.Chrome()
 
-    def test_animation_page(self, web):
-        web.back
-        web.page.animation_button.click()
-        assert web.page.cloning_button.get_element().is_visible()
-
-    def test_app_page(self, web):
-        web.back
-        web.page.app_button.click()
-        assert web.page.activity_button.get_element().is_visible()
-
-    def test_os_page(self, web):
-        web.back
-        web.page.os_button.click()
-        assert web.page.morse_code_button.get_element().is_visible()
+web = WebPage(driver, webdriver_wait=20, logger=False)
+web.driver.get('https://pypi.org/')
+
+web.locate(By.ID, 'search').get_element().send_keys('citronella')
+web.locate(By.XPATH, '//button[@type="submit"]/i').get_element().click()
+
+elements = web.locate(By.XPATH, '//span[@class="package-snippet__name"]')
+if elements.ec_visibility_of_all_elements_located():
+    results = elements.get_elements()
+    text_lists = [x.text for x in results]
 ```
+
 ___
 ## Install Package
 
 ```bash
 pip install citronella
 ```
 
 ___
 ## Documentation
 
-There are only three modules imported in this package:
+There are only two modules import in this package:
 
 * The first module is for conftest.py.
 
 ### Selenium
 
 ```python
 import pytest
@@ -158,64 +145,131 @@
     options.platformName = 'Android'
     options.app = os.getcwd() + '/APK/ApiDemos-debug.apk.zip'
     driver = webdriver.Remote('http://127.0.0.1:4723/wd/hub', options=options)
     yield WebPage(driver)
     driver.quit()
 ```
 
-* The second and third modules are for the page object model.
-
-[Check out this link for more information on the Page Object Design.](https://github.com/heyclore/citronella/tree/main/python/example#readme)
+* The second module are for the page object model.
 
 ### Selenium
 
 ```python
 from selenium.webdriver.common.by import By
-from citronella import Ui, PlaceholderPage
-from Pages.component.HeaderMenu import HeaderMenu
+from citronella import ui
+from Pages.contents_page import ContentsPage
 
 
-class HomePage(HeaderMenu):
+class HomePage(ContentsPage().header()):
 
     def some_button(self):
-        return Ui(By.XPATH, '//a[@name="foo"]')
+        return ui(By.XPATH, '//a[@name="foo"]')
 
     def search_input(self):
-        return Ui(By.ID, 'search')
+        return ui(By.ID, 'search')
 
     def search_button(self):
-        from Pages.SearchPage import SearchPage
-        return Ui(By.NAME, 'search-button', SearchPage)
-
-    def link_to_somewhere_currently_dont_have_page_object(self):
-        return Ui(By.NAME, 'search-button', PlaceholderPage)
+        return ui(By.NAME, 'search-button')
 ```
 
 ### Appium
 
 ```python
 from appium.webdriver.common.appiumby import AppiumBy
-from citronella import Ui, PlaceholderPage
-from Pages.component.HeaderMenu import HeaderMenu
+from citronella import ui
+from Pages.contents_page import ContentsPage
 
 
-class HomePage(HeaderMenu):
+class HomePage(ContentsPage().header()):
 
     def some_button(self):
-        return Ui(AppiumBy.XPATH, '//a[@name="foo"]')
+        return ui(AppiumBy.XPATH, '//a[@name="foo"]')
 
     def search_input(self):
-        return Ui(AppiumBy.ACCESSIBILITY_ID, 'search')
+        return ui(AppiumBy.ACCESSIBILITY_ID, 'search')
 
     def search_button(self):
-        from Pages.SearchPage import SearchPage
-        return Ui(AppiumBy.ID, 'search-button', SearchPage)
+        return ui(AppiumBy.ID, 'search-button')
+```
+
+___
+## Page Object Design / Strategy
+
+There's a two ways to create a page object for `WebPage`:
+
+1. Straightforward approach: This method requires importing the page object for each test.
+```python
+from selenium import webdriver
+from selenium.webdriver.common.by import By
+from citronella import WebPage, ui
+
+
+class HomePage:
+    def auth_buton(self):
+        return ui(By.XPATH, '//a[@name="foo"]')
 
-    def link_to_somewhere_currently_dont_have_page_object(self):
-        return Ui(AppiumBy.ACCESSIBILITY_ID, 'search-button', PlaceholderPage)
+class LoginPage:
+    def email_input(self):
+        return ui(By.ID, 'email')
+
+    def password_input(self):
+        return ui(By.ID, 'password')
+
+    def login_buton(self):
+        return ui(By.ID, 'login')
+
+driver = webdriver.Chrome()
+web = WebPage(driver)
+web.driver.get('https://foobarbaz.com/')
+web.page = HomePage
+web.page.auth_button.click()
+web.page = LoginPage
+web.page.email_input.send_keys('foo')
+web.page.password_input.send_keys('bar')
+web.page.login_button.click()
+```
+
+2. Lazy loading approach: This method is slightly more complex but offers the benefit of lazy loading.
+see [ContentsPage example](https://github.com/heyclore/citronella/blob/main/python/example/selenium/Pages/contents_page.py)
+or this [Page object example](https://github.com/heyclore/citronella/tree/main/python/example/selenium/Pages)
+```python
+from selenium import webdriver
+from selenium.webdriver.common.by import By
+from citronella import WebPage, ui
+
+
+class ContentsPage:
+    def home_page(self):
+        return HomePage
+
+    def login_page(self):
+        return LoginPage
+
+class HomePage:
+    def auth_buton(self):
+        return ui(By.XPATH, '//a[@name="foo"]')
+
+class LoginPage:
+    def email_input(self):
+        return ui(By.ID, 'email')
+
+    def password_input(self):
+        return ui(By.ID, 'password')
+
+    def login_buton(self):
+        return ui(By.ID, 'login')
+
+driver = webdriver.Chrome()
+web = WebPage(driver)
+web.driver.get('https://foobarbaz.com/')
+web.page = ContentsPage
+web.page.home_page.auth_button.click()
+web.page.login_page.email_input.send_keys('foo')
+web.page.login_page.password_input.send_keys('bar')
+web.page.login_page.login_button.click()
 ```
 
 ___
 ## Usage
 
 ### citronella.WebPage
 
@@ -225,44 +279,41 @@
 ###### Kwargs (optional):
 - webdriver_wait `number(seconds)`, default value is `10`
 - logger `bool`, default value is `True`
 
 ###### Method Lists:
 | Method Name        | Args*       | Kwargs**         | Note |
 | ------------------ |:-----------:|:----------------:|:----:|
-| driver             | None        | None             | return selenium `webdriver` object |
-| locate             | by, value   | None             | similar as`driver.get_element` args |
-| page_object        | Page Object | get_start `bool` | Page Object must contain `ACTIVITY` variable with URL(selenium)/State(appium) if using Kwargs** | 
-| page               | None        | None             |      |
-| back               | None        | None             |      |
-| webdriver_wait     | number(sec) | None             |      |
-| ready_state        | number(sec) | None             | execute javascript `document.readyState` manually, default timeout is `0` |
-| get_window_size    | None        | None             |      |
-| sleep              | number(sec) | None             |      |
+| driver             | -           | -                | return selenium `webdriver` object |
+| locate             | by, value   | -                | similar as`driver.get_element` args |
+| page               | page object | -                | setter |
+| page               | -           | -                | getter |
+| webdriver_wait     | number(sec) | -                |      |
+| ready_state        | number(sec) | -                | execute javascript `document.readyState` manually, default timeout is `30` |
+| sleep              | number(sec) | -                |      |
 
 ### citronella.ui / citronella.WebUi
 
 ###### Args:
 - by
 - value
-- page_object (optional)
 
 ###### Method Lists:
 | Method Name   | Args*  | Kwargs**           | Note |
 | ------------- |:------:|:------------------:|:----:|
-| send_keys     | text   | clear `bool`, return_key `bool` | default value is `False` by default |
-| click         | None   | switch_page `bool` | see [test_auth.py](example/selenium/Test/pytest_html_image/test_auth.py) example |
-| get_element   | None   | None               |      |
-| get_elements  | None   | None               |      |
-| ec_element_to_be_clickable | None | None | wrapper of `EC` / `excpected_condition` |
-| ec_presence_of_element_located | None | None | wrapper of `EC` / `excpected_condition` |
-| ec_presence_of_all_elements_located | None | None | wrapper of `EC` / `excpected_condition` |
-| ec_visibility_of_element_located | None | None | wrapper of `EC` / `excpected_condition` |
-| ec_visibility_of_all_elements_located | None | None | wrapper of `EC` / `excpected_condition` |
-| ec_visibility_of_any_elements_located | None | None | wrapper of `EC` / `excpected_condition` |
-| ec_invisibility_of_element_located | None | None | wrapper of `EC` / `excpected_condition` |
-| ec_element_located_to_be_selected | None | None | wrapper of `EC` / `excpected_condition` |
+| send_keys     | text   | clear `bool`, return_key `bool` |     |
+| click         | -      | -                  |      |
+| get_element   | -      | -                  |      |
+| get_elements  | -      | -                  |      |
+| ec_element_to_be_clickable | -    | -    | wrapper of `EC` / `excpected_condition` |
+| ec_presence_of_element_located | -    | -    | wrapper of `EC` / `excpected_condition` |
+| ec_presence_of_all_elements_located | -    | -    | wrapper of `EC` / `excpected_condition` |
+| ec_visibility_of_element_located | -    | -    | wrapper of `EC` / `excpected_condition` |
+| ec_visibility_of_all_elements_located | -    | -    | wrapper of `EC` / `excpected_condition` |
+| ec_visibility_of_any_elements_located | -    | -    | wrapper of `EC` / `excpected_condition` |
+| ec_invisibility_of_element_located | -    | -    | wrapper of `EC` / `excpected_condition` |
+| ec_element_located_to_be_selected | -    | -    | wrapper of `EC` / `excpected_condition` |
 
 
 ## Testing powered by
 <a target="_blank" href="https://www.browserstack.com/"><img width="200" src="https://www.browserstack.com/images/layout/browserstack-logo-600x315.png"></a><br>
 [BrowserStack Open-Source Program](https://www.browserstack.com/open-source)
```

### Comparing `citronella-0.0.5/README.md` & `citronella-0.0.6/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -6,107 +6,94 @@
 webdriver extension with a page object wrapper.
 
 ![alt terminal](https://github.com/heyclore/citronella/blob/main/python/screenshot/terminal.png?raw=true)
 ![alt pytest-html](https://github.com/heyclore/citronella/blob/main/python/screenshot/pytest_html.png?raw=true)
 ![alt github-action](https://github.com/heyclore/citronella/blob/main/python/screenshot/github_action.png?raw=true)
 
 ## Example Tests
-Even though this module is mainly designed for the page object model, it can also be used without it for quick prototyping or mockups, etc.
-```python
-from selenium import webdriver
-from selenium.webdriver.common.by import By
-from citronella import WebPage
-
-
-driver = webdriver.Chrome()
-
-web = WebPage(driver, webdriver_wait=20, logger=False)
-web.driver.get('https://pypi.org/')
-
-web.locate(By.ID, 'search').get_element().send_keys('citronella')
-web.locate(By.XPATH, '//button[@type="submit"]/i').get_element().click()
-
-elements = web.locate(By.XPATH, '//span[@class="package-snippet__name"]')
-if elements.ec_visibility_of_all_elements_located():
-    results = elements.get_elements()
-    text_lists = [x.text for x in results]
-```
-
-
 
 ### Selenium
 
 ```python
 import pytest
-from Pages.home.home_page import HomePage
+from Pages.contents_page import ContentsPage
 
 
 class TestNavigationMenu:
 
     def test_help_page(self, web):
         web.driver.get('https://pypi.org/')
-        web.page_object(HomePage)
+        web.page = ContentsPage
 
-        web.page.help_button.click()
+        web.page.home_page.help_button.click()
         assert 'Help' in web.driver.title
 
     def test_sponsors_page(self, web):
-        web.page.sponsors_button.click()
+        web.page.help_page.sponsors_button.click()
         assert 'Sponsors' in web.driver.title
 
     def test_login_page(self, web):
-        web.page.login_button.click()
+        web.page.sponsors_page.login_button.click()
         assert 'Log' in web.driver.title
 
     def test_register_page(self, web):
-        web.page.register_button.click()
+        web.page.login_page.register_button.click()
         assert 'Create' in web.driver.title
 ```
 
 ### Appium
 
 ```python
 import pytest
-from Pages.api_demos_page import ApiDemosPage
+from Pages.contents_page import ContentsPage
 
 
-class TestNavigationMenu:
+class TestInput:
+
+    def test_input(self, web):
+        web.page = ContentsPage
+        web.page.home_page.gallery_button.click()
+        web.page.gallery_page.text_input.send_keys('citronella')
+        web.page.gallery_page.add_button.click()
+        elements = web.page.gallery_page.text_lists.get_elements()
+        assert 'citronella' in [x.text for x in elements]
+```
+
+Even though this module is mainly designed for the page object model, it can also be used without it for quick prototyping or mockups, etc.
+```python
+from selenium import webdriver
+from selenium.webdriver.common.by import By
+from citronella import WebPage
 
-    def test_accessibility_page(self, web):
-        web.page_object(ApiDemosPage)
 
-        web.page.accessibility_button.click()
-        assert web.page.accessibility_node_provider_button.get_element().is_visible()
+driver = webdriver.Chrome()
 
-    def test_animation_page(self, web):
-        web.back
-        web.page.animation_button.click()
-        assert web.page.cloning_button.get_element().is_visible()
-
-    def test_app_page(self, web):
-        web.back
-        web.page.app_button.click()
-        assert web.page.activity_button.get_element().is_visible()
-
-    def test_os_page(self, web):
-        web.back
-        web.page.os_button.click()
-        assert web.page.morse_code_button.get_element().is_visible()
+web = WebPage(driver, webdriver_wait=20, logger=False)
+web.driver.get('https://pypi.org/')
+
+web.locate(By.ID, 'search').get_element().send_keys('citronella')
+web.locate(By.XPATH, '//button[@type="submit"]/i').get_element().click()
+
+elements = web.locate(By.XPATH, '//span[@class="package-snippet__name"]')
+if elements.ec_visibility_of_all_elements_located():
+    results = elements.get_elements()
+    text_lists = [x.text for x in results]
 ```
+
 ___
 ## Install Package
 
 ```bash
 pip install citronella
 ```
 
 ___
 ## Documentation
 
-There are only three modules imported in this package:
+There are only two modules import in this package:
 
 * The first module is for conftest.py.
 
 ### Selenium
 
 ```python
 import pytest
@@ -137,64 +124,131 @@
     options.platformName = 'Android'
     options.app = os.getcwd() + '/APK/ApiDemos-debug.apk.zip'
     driver = webdriver.Remote('http://127.0.0.1:4723/wd/hub', options=options)
     yield WebPage(driver)
     driver.quit()
 ```
 
-* The second and third modules are for the page object model.
-
-[Check out this link for more information on the Page Object Design.](https://github.com/heyclore/citronella/tree/main/python/example#readme)
+* The second module are for the page object model.
 
 ### Selenium
 
 ```python
 from selenium.webdriver.common.by import By
-from citronella import Ui, PlaceholderPage
-from Pages.component.HeaderMenu import HeaderMenu
+from citronella import ui
+from Pages.contents_page import ContentsPage
 
 
-class HomePage(HeaderMenu):
+class HomePage(ContentsPage().header()):
 
     def some_button(self):
-        return Ui(By.XPATH, '//a[@name="foo"]')
+        return ui(By.XPATH, '//a[@name="foo"]')
 
     def search_input(self):
-        return Ui(By.ID, 'search')
+        return ui(By.ID, 'search')
 
     def search_button(self):
-        from Pages.SearchPage import SearchPage
-        return Ui(By.NAME, 'search-button', SearchPage)
-
-    def link_to_somewhere_currently_dont_have_page_object(self):
-        return Ui(By.NAME, 'search-button', PlaceholderPage)
+        return ui(By.NAME, 'search-button')
 ```
 
 ### Appium
 
 ```python
 from appium.webdriver.common.appiumby import AppiumBy
-from citronella import Ui, PlaceholderPage
-from Pages.component.HeaderMenu import HeaderMenu
+from citronella import ui
+from Pages.contents_page import ContentsPage
 
 
-class HomePage(HeaderMenu):
+class HomePage(ContentsPage().header()):
 
     def some_button(self):
-        return Ui(AppiumBy.XPATH, '//a[@name="foo"]')
+        return ui(AppiumBy.XPATH, '//a[@name="foo"]')
 
     def search_input(self):
-        return Ui(AppiumBy.ACCESSIBILITY_ID, 'search')
+        return ui(AppiumBy.ACCESSIBILITY_ID, 'search')
 
     def search_button(self):
-        from Pages.SearchPage import SearchPage
-        return Ui(AppiumBy.ID, 'search-button', SearchPage)
+        return ui(AppiumBy.ID, 'search-button')
+```
+
+___
+## Page Object Design / Strategy
+
+There's a two ways to create a page object for `WebPage`:
+
+1. Straightforward approach: This method requires importing the page object for each test.
+```python
+from selenium import webdriver
+from selenium.webdriver.common.by import By
+from citronella import WebPage, ui
+
+
+class HomePage:
+    def auth_buton(self):
+        return ui(By.XPATH, '//a[@name="foo"]')
 
-    def link_to_somewhere_currently_dont_have_page_object(self):
-        return Ui(AppiumBy.ACCESSIBILITY_ID, 'search-button', PlaceholderPage)
+class LoginPage:
+    def email_input(self):
+        return ui(By.ID, 'email')
+
+    def password_input(self):
+        return ui(By.ID, 'password')
+
+    def login_buton(self):
+        return ui(By.ID, 'login')
+
+driver = webdriver.Chrome()
+web = WebPage(driver)
+web.driver.get('https://foobarbaz.com/')
+web.page = HomePage
+web.page.auth_button.click()
+web.page = LoginPage
+web.page.email_input.send_keys('foo')
+web.page.password_input.send_keys('bar')
+web.page.login_button.click()
+```
+
+2. Lazy loading approach: This method is slightly more complex but offers the benefit of lazy loading.
+see [ContentsPage example](https://github.com/heyclore/citronella/blob/main/python/example/selenium/Pages/contents_page.py)
+or this [Page object example](https://github.com/heyclore/citronella/tree/main/python/example/selenium/Pages)
+```python
+from selenium import webdriver
+from selenium.webdriver.common.by import By
+from citronella import WebPage, ui
+
+
+class ContentsPage:
+    def home_page(self):
+        return HomePage
+
+    def login_page(self):
+        return LoginPage
+
+class HomePage:
+    def auth_buton(self):
+        return ui(By.XPATH, '//a[@name="foo"]')
+
+class LoginPage:
+    def email_input(self):
+        return ui(By.ID, 'email')
+
+    def password_input(self):
+        return ui(By.ID, 'password')
+
+    def login_buton(self):
+        return ui(By.ID, 'login')
+
+driver = webdriver.Chrome()
+web = WebPage(driver)
+web.driver.get('https://foobarbaz.com/')
+web.page = ContentsPage
+web.page.home_page.auth_button.click()
+web.page.login_page.email_input.send_keys('foo')
+web.page.login_page.password_input.send_keys('bar')
+web.page.login_page.login_button.click()
 ```
 
 ___
 ## Usage
 
 ### citronella.WebPage
 
@@ -204,44 +258,41 @@
 ###### Kwargs (optional):
 - webdriver_wait `number(seconds)`, default value is `10`
 - logger `bool`, default value is `True`
 
 ###### Method Lists:
 | Method Name        | Args*       | Kwargs**         | Note |
 | ------------------ |:-----------:|:----------------:|:----:|
-| driver             | None        | None             | return selenium `webdriver` object |
-| locate             | by, value   | None             | similar as`driver.get_element` args |
-| page_object        | Page Object | get_start `bool` | Page Object must contain `ACTIVITY` variable with URL(selenium)/State(appium) if using Kwargs** | 
-| page               | None        | None             |      |
-| back               | None        | None             |      |
-| webdriver_wait     | number(sec) | None             |      |
-| ready_state        | number(sec) | None             | execute javascript `document.readyState` manually, default timeout is `0` |
-| get_window_size    | None        | None             |      |
-| sleep              | number(sec) | None             |      |
+| driver             | -           | -                | return selenium `webdriver` object |
+| locate             | by, value   | -                | similar as`driver.get_element` args |
+| page               | page object | -                | setter |
+| page               | -           | -                | getter |
+| webdriver_wait     | number(sec) | -                |      |
+| ready_state        | number(sec) | -                | execute javascript `document.readyState` manually, default timeout is `30` |
+| sleep              | number(sec) | -                |      |
 
 ### citronella.ui / citronella.WebUi
 
 ###### Args:
 - by
 - value
-- page_object (optional)
 
 ###### Method Lists:
 | Method Name   | Args*  | Kwargs**           | Note |
 | ------------- |:------:|:------------------:|:----:|
-| send_keys     | text   | clear `bool`, return_key `bool` | default value is `False` by default |
-| click         | None   | switch_page `bool` | see [test_auth.py](example/selenium/Test/pytest_html_image/test_auth.py) example |
-| get_element   | None   | None               |      |
-| get_elements  | None   | None               |      |
-| ec_element_to_be_clickable | None | None | wrapper of `EC` / `excpected_condition` |
-| ec_presence_of_element_located | None | None | wrapper of `EC` / `excpected_condition` |
-| ec_presence_of_all_elements_located | None | None | wrapper of `EC` / `excpected_condition` |
-| ec_visibility_of_element_located | None | None | wrapper of `EC` / `excpected_condition` |
-| ec_visibility_of_all_elements_located | None | None | wrapper of `EC` / `excpected_condition` |
-| ec_visibility_of_any_elements_located | None | None | wrapper of `EC` / `excpected_condition` |
-| ec_invisibility_of_element_located | None | None | wrapper of `EC` / `excpected_condition` |
-| ec_element_located_to_be_selected | None | None | wrapper of `EC` / `excpected_condition` |
+| send_keys     | text   | clear `bool`, return_key `bool` |     |
+| click         | -      | -                  |      |
+| get_element   | -      | -                  |      |
+| get_elements  | -      | -                  |      |
+| ec_element_to_be_clickable | -    | -    | wrapper of `EC` / `excpected_condition` |
+| ec_presence_of_element_located | -    | -    | wrapper of `EC` / `excpected_condition` |
+| ec_presence_of_all_elements_located | -    | -    | wrapper of `EC` / `excpected_condition` |
+| ec_visibility_of_element_located | -    | -    | wrapper of `EC` / `excpected_condition` |
+| ec_visibility_of_all_elements_located | -    | -    | wrapper of `EC` / `excpected_condition` |
+| ec_visibility_of_any_elements_located | -    | -    | wrapper of `EC` / `excpected_condition` |
+| ec_invisibility_of_element_located | -    | -    | wrapper of `EC` / `excpected_condition` |
+| ec_element_located_to_be_selected | -    | -    | wrapper of `EC` / `excpected_condition` |
 
 
 ## Testing powered by
 <a target="_blank" href="https://www.browserstack.com/"><img width="200" src="https://www.browserstack.com/images/layout/browserstack-logo-600x315.png"></a><br>
 [BrowserStack Open-Source Program](https://www.browserstack.com/open-source)
```

### Comparing `citronella-0.0.5/setup.py` & `citronella-0.0.6/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 
 setup(
     name="citronella",
-    version="0.0.5",
+    version="0.0.6",
     license="MIT",
     description="Webdriver Extension with Page Object Wrapper",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/heyclore/citronella",
+    url="https://github.com/heyclore/citronella/tree/main/python#readme",
     author="heyclore",
     author_email="cloore@gmail.com",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Testing",
         "License :: OSI Approved :: MIT License",
```

### Comparing `citronella-0.0.5/src/citronella/__init__.py` & `citronella-0.0.6/src/citronella/placeholder_page.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,13 +17,8 @@
 #FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 #OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 #SOFTWARE.
 
 
-from .ui import ui
-from .web_page import WebPage
-from .placeholder_page import PlaceholderPage
-#MARK TO REMOVE {
-from .ui import Ui
-#MARK TO REMOVE }
+class PlaceholderPage: pass
```

### Comparing `citronella-0.0.5/src/citronella/logger.py` & `citronella-0.0.6/src/citronella/logger.py`

 * *Files identical despite different names*

### Comparing `citronella-0.0.5/src/citronella/page_decorator.py` & `citronella-0.0.6/src/citronella/page_decorator.py`

 * *Files 22% similar despite different names*

```diff
@@ -22,25 +22,31 @@
 
 
 from .web_ui import WebUi
 
 
 class PageDecorator:
     """This is a page decorator class."""
-    def __init__(self, driver, webdriver_wait, pages, logger):
-        self.cls = pages.current_page()
+    def __init__(self, driver, webdriver_wait, contents_page, logger):
         self.driver = driver
-        self.pages = pages
-        self.logger = logger
         self.webdriver_wait = webdriver_wait
+        self.contents_page = contents_page
+        self.logger = logger
 
     def __getattr__(self, attr):
         """look up the attr / method name inside page object."""
-        cls_attr = self.cls.__getattribute__(attr)
-        def wrap(*args, **kwargs):
-            """This is a wrapper function."""
-            f = cls_attr(*args, **kwargs)
-            return WebUi(self.driver, self.webdriver_wait, self.pages,
-                         self.logger, f['by'], f['value'], f['page'], attr,
-                         self.cls.__class__.__name__)
+        try:
+            ui = self.contents_page().__getattribute__(attr)()
+        except TypeError as e:
+            if 'takes 0 positional arguments but 1 was given' in str(e):
+                raise Exception(f'please add "self" to "{attr}" method '
+                                f'from {self.contents_page.__name__}')
+            raise Exception(e)
+        except Exception as e:
+            raise Exception(e)
+
+        if isinstance(ui, dict):
+            return WebUi(self.driver, self.webdriver_wait, self.logger,
+                         ui['by'], ui['value'], attr,
+                         self.contents_page.__name__)
 
-        return wrap()
+        return PageDecorator(self.driver, self.webdriver_wait, ui, self.logger)
```

### Comparing `citronella-0.0.5/src/citronella/page_tab.py` & `citronella-0.0.6/src/citronella/ui.py`

 * *Files 21% similar despite different names*

```diff
@@ -17,27 +17,30 @@
 #FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 #OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 #SOFTWARE.
 
 
-class PageTab:
-    """This is a page page tab class."""
-    _pages = []
-
-    @property
-    def current_page(self):
-        """return the last page object stored."""
-        return self._pages[-1]
-
-    def append(self, new_page):
-        """store the page object in _pages."""
-        self._pages.append(new_page)
-        if len(self._pages) > 5:
-            self._pages.pop(0)
-
-    def pop(self):
-        """delete the last item of the _pages lists."""
-        if len(self._pages) == 0:
-            return
-        self._pages.pop()
+from .deprecated import logwarning
+
+
+def ui(by, value, page=None):
+    """
+    forward the data to page decorator and wrap into WebUi class.
+
+    Args:
+        by
+        ui
+
+    Usage:
+        ui(By.NAME, 'q')
+    """
+    ##
+    if page:
+        logwarning('"page" kwargs for ui module is deprecated and will '
+        'remove for the next version.')
+    ##
+    return {
+            'by': by,
+            'value': value,
+            }
```

### Comparing `citronella-0.0.5/src/citronella/placeholder_page.py` & `citronella-0.0.6/src/citronella/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -17,8 +17,10 @@
 #FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 #OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 #SOFTWARE.
 
 
-class PlaceholderPage: pass
+from .ui import ui
+from .web_page import WebPage
+from .placeholder_page import PlaceholderPage
```

### Comparing `citronella-0.0.5/src/citronella/web_page.py` & `citronella-0.0.6/src/citronella/web_page.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,138 +19,131 @@
 #LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 #OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 #SOFTWARE.
 
 
 from types import SimpleNamespace
 from time import sleep
+from logging import warning
 from .page_decorator import PageDecorator
-from .page_tab import PageTab
 from .web_ui import WebUi
+from .page_validator import page_validator
+from .deprecated import logwarning
 
 
 class WebPage:
     """
     an object class that use across the tests.
+    contents_page are need to set if using page object strategy, it does not
+    requied if only using this to access 'web.locate'.
     webdriver_wait is set '10' seconds by default
     logger is set 'True' by default
 
     Args:
         driver
     Kwargs (optional):
+        contents_page
         webdriver_wait
         logger
 
     Usage:
         driver = webdriver.Chrome()
         web = WebPage(driver)
+        or
+        web = WebPage(driver) without contents_page to access "web.locate" only
     """
     def __init__(self, driver, webdriver_wait=10, logger=True):
         self._driver = driver
         self._webdriver_wait = webdriver_wait
-        self._pages = PageTab()
+        self._contents_page = None
         self._logger = logger
-        self._app = driver.current_package if 'appium' in str(
-                driver.__class__) else None
 
     @property
     def driver(self):
         """return the original selenium / appium driver."""
         return self._driver
 
-    @property
-    def page(self):
-        """return last page object model."""
-        return PageDecorator(self.driver, self._webdriver_wait, self._pages,
-                             self._logger)
-
+    ##
     def page_object(self, new_page, get_start=False):
         """
-        initialize page object module object, get_start kwargs is optional and
-        it set to FALSE by default, it can be use if the page object have
-        an ACTIVITY constant variable.
-        in selenium:
-        it's equal as self.driver.get(url)
-        in appium:
-        it's equal as self.driver.start_activity(package_name, activity_name)
+        initialize page object module object.
 
         Args:
             page_object_model
 
-        Kwargs:
-            get_start=True
-
         Usage:
-            self.browser.page_object(Homepage)
-            or
-            self.browser.page_object(Homepage, get_start=True)
-        """
-        self._pages.append(new_page)
-        if get_start:
-            if 'ACTIVITY' not in dir(new_page):
-                raise ValueError(
-                        f'ACTIVITY is not exist in {new_page.__qualname__}')
-            if self._app:
-                return self.driver.start_activity(self._app, new_page.ACTIVITY)
-            self.driver.get(new_page.ACTIVITY)
+            web.page_object(ContentsPage)
+        """
+        self._contents_page = new_page
+        logwarning('\n\t "page_object" method is deprecated and will remove for the next version'
+                   '\n\t use "web.page = HomePage" instead \n\t or \n\t "web.page = ContentsPage"'
+                   )
+    ##
+
+    @property
+    def page(self):
+        """return a page decorator object of ContentsPage."""
+        if not self._contents_page:
+            warning('\n\tpage object hasn\'t been set yet.'
+                    '\n\t"web = WebPage(driver, contents_page=ContentsPage)" '
+                    'before "using web.page.foo.click()" etc.')
+        return PageDecorator(self.driver, self._webdriver_wait, self._contents_page,
+                             self._logger)
+
+    @page.setter
+    def page(self, new_page):
+        self._contents_page = page_validator(new_page)
 
     def locate(self, by, value):
         """
         an alternative way for testing without page object and return WebUi
         class, but can't use page and back method and causing an error.
         good for quick prototype / write a tests.
 
         Args:
             by
             value
 
         Usage:
-            web.ui(By.NAME, 'q').ec_presence_of_element_located()
-            web.ui(By.NAME, 'q').get_element().text()
-            web.ui(By.NAME, 'q').get_element().click()
-        """
-        return WebUi(self._driver, self._webdriver_wait, self._pages,
-                     self._logger, by, value, None, self.locate.__name__,
-                     self.__class__.__name__)
+            web.locate(By.NAME, 'q').ec_presence_of_element_located()
+            web.locate(By.NAME, 'q').get_element().text()
+            web.locate(By.NAME, 'q').get_element().click()
+        """
+        return WebUi(self._driver, self._webdriver_wait, self._logger, by,
+                     value, self.locate.__name__, self.__class__.__name__)
 
+    ##
     @property
     def back(self):
-        """return to previous page and delete the last page object."""
+        """return to previous page."""
         self.driver.back()
-        self._pages.pop()
+        logwarning('"back" method is deprecated and will remove for the next '
+                   'version.\n\t use "web.driver.back()" instead.')
 
     @property
     def get_window_size(self):
         """
         get current windows size.
 
         Usage:
-            height = self.browser.get_window_size.height
-            width = self.browser.get_window_size.width
+            height = web.get_window_size.height
+            width = web.get_window_size.width
         """
+        logwarning('"get_window_size" method is deprecated and will remove for the next '
+                   'version.\n\t use "web.driver.get_window_size()" instead.')
         return SimpleNamespace(**self.driver.get_window_size())
+    ##
 
-    def ready_state(self, wait):
-        """execute javascript for page to fully load, disabled for appium"""
-        if not self._app:
-            for x in range(wait):
-                if self.driver.execute_script(
-                        'return document.readyState') != 'complete':
-                    sleep(1)
+    def ready_state(self, timeout=30):
+        """execute javascript for page to fully load"""
+        for x in range(timeout):
+            if self.driver.execute_script(
+                    'return document.readyState') != 'complete':
+                sleep(1)
 
     def webdriver_wait(self, wait):
         """override webdriver wait."""
         self._webdriver_wait = wait
 
     def sleep(self, time):
         """use time.sleep module to manually wait."""
         sleep(time)
-
-    #MARK TO REMOVE {
-    @property
-    def ready_state_toggle(self):
-        """switch ready_state bool"""
-        #self._ready_state = not self._ready_state
-        from logging import warning
-        warning("ready_state_toggle module is deprecated and will be removed in the next version.")
-        warning("will remove this method for next version")
-    #MARK TO REMOVE }
```

### Comparing `citronella-0.0.5/src/citronella/web_ui.py` & `citronella-0.0.6/src/citronella/web_ui.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,26 +26,25 @@
 from selenium.webdriver.common.keys import Keys
 from selenium.webdriver.support.expected_conditions import \
         presence_of_element_located, presence_of_all_elements_located, \
         visibility_of_element_located, visibility_of_all_elements_located, \
         visibility_of_any_elements_located, invisibility_of_element_located, \
         element_located_to_be_selected, element_to_be_clickable
 from .logger import logger
+from .deprecated import logwarning
 
 
 class WebUi:
     """a wrapped object of a web element."""
-    def __init__(self, driver, webdriver_wait, pages, logger, by, value,
-                 new_page, function_name, class_name):
+    def __init__(self, driver, webdriver_wait, logger, by, value,
+                 function_name, class_name):
         self._driver = driver
         self._wait = webdriver_wait
-        self._pages = pages
         self._logger = logger
         self._locator = (by, value)
-        self._new_page = new_page
         self._function_name = function_name
         self._class_name = class_name
 
     def _webdriver_wait(self, ec):
         """return a web element or elements."""
         WebDriverWait(self._driver, self._wait)
         return WebDriverWait(self._driver, self._wait).until(ec)
@@ -109,55 +108,35 @@
         """return list of web element, equal as find_elements."""
         return self._webdriver_wait(presence_of_all_elements_located(
             self._locator))
 
     @logger
     def click(self, switch_page=True):
         """click to web element."""
+        ##
+        if not switch_page:
+            logwarning('"switch_page" kwargs is deprecated and will remove for the next version')
+            return
+        ##
         try:
             self._webdriver_wait(element_to_be_clickable(self._locator)).click()
         except Exception as e:
             sleep(2)
             self._webdriver_wait(element_to_be_clickable(self._locator)).click()
 
-        if self._new_page and switch_page:
-            self._pages.append(self._new_page)
-
     @logger
-    def send_keys(self, text, clear=False, return_key=False):
+    def send_keys(self, text, clear=False, return_key=False, switch_page=True):
         """custom webdriver send_keys with optional clear field."""
+        ##
+        if not switch_page:
+            logwarning('"switch_page" kwargs is deprecated and will remove for the next version')
+            return
+        ##
         element = self._webdriver_wait(presence_of_element_located(self._locator))
 
         if clear:
             element.clear()
 
         element.send_keys(text)
 
         if return_key:
             element.send_keys(Keys.RETURN)
-
-            if self._new_page:
-                self._pages.append(self._new_page)
-
-#MARK TO REMOVE {
-    def get_attribute(self, attribute):
-        from logging import warning
-        warning("get_attribute module is deprecated and will be removed in the next version.")
-        warning('use "web.page.foobar.get_element.get_attribute(attribute)" instead')
-        return self._webdriver_wait(presence_of_element_located(
-            self._locator)).get_attribute(attribute)
-
-    @logger
-    def is_located(self):
-        from logging import warning
-        warning("is_located module is deprecated and will be removed in the next version.")
-        warning('use "web.page.foobar.ec_presence_of_element_located" instead')
-        return True if self._webdriver_wait(
-                presence_of_all_elements_located(self._locator)) else False
-
-    @logger
-    def text(self):
-        from logging import warning
-        warning("text module is deprecated and will be removed in the next version.")
-        warning('use "web.page.foobar.get_element.text" instead')
-        return self.get_element().text
-#MARK TO REMOVE }
```

### Comparing `citronella-0.0.5/src/citronella.egg-info/PKG-INFO` & `citronella-0.0.6/src/citronella.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: citronella
-Version: 0.0.5
+Version: 0.0.6
 Summary: Webdriver Extension with Page Object Wrapper
-Home-page: https://github.com/heyclore/citronella
+Home-page: https://github.com/heyclore/citronella/tree/main/python#readme
 Author: heyclore
 Author-email: cloore@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/heyclore/citronella/tree/main/python
 Keywords: test,unittest,pytest,webdriver,appium,selenium
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -27,107 +27,94 @@
 webdriver extension with a page object wrapper.
 
 ![alt terminal](https://github.com/heyclore/citronella/blob/main/python/screenshot/terminal.png?raw=true)
 ![alt pytest-html](https://github.com/heyclore/citronella/blob/main/python/screenshot/pytest_html.png?raw=true)
 ![alt github-action](https://github.com/heyclore/citronella/blob/main/python/screenshot/github_action.png?raw=true)
 
 ## Example Tests
-Even though this module is mainly designed for the page object model, it can also be used without it for quick prototyping or mockups, etc.
-```python
-from selenium import webdriver
-from selenium.webdriver.common.by import By
-from citronella import WebPage
-
-
-driver = webdriver.Chrome()
-
-web = WebPage(driver, webdriver_wait=20, logger=False)
-web.driver.get('https://pypi.org/')
-
-web.locate(By.ID, 'search').get_element().send_keys('citronella')
-web.locate(By.XPATH, '//button[@type="submit"]/i').get_element().click()
-
-elements = web.locate(By.XPATH, '//span[@class="package-snippet__name"]')
-if elements.ec_visibility_of_all_elements_located():
-    results = elements.get_elements()
-    text_lists = [x.text for x in results]
-```
-
-
 
 ### Selenium
 
 ```python
 import pytest
-from Pages.home.home_page import HomePage
+from Pages.contents_page import ContentsPage
 
 
 class TestNavigationMenu:
 
     def test_help_page(self, web):
         web.driver.get('https://pypi.org/')
-        web.page_object(HomePage)
+        web.page = ContentsPage
 
-        web.page.help_button.click()
+        web.page.home_page.help_button.click()
         assert 'Help' in web.driver.title
 
     def test_sponsors_page(self, web):
-        web.page.sponsors_button.click()
+        web.page.help_page.sponsors_button.click()
         assert 'Sponsors' in web.driver.title
 
     def test_login_page(self, web):
-        web.page.login_button.click()
+        web.page.sponsors_page.login_button.click()
         assert 'Log' in web.driver.title
 
     def test_register_page(self, web):
-        web.page.register_button.click()
+        web.page.login_page.register_button.click()
         assert 'Create' in web.driver.title
 ```
 
 ### Appium
 
 ```python
 import pytest
-from Pages.api_demos_page import ApiDemosPage
+from Pages.contents_page import ContentsPage
 
 
-class TestNavigationMenu:
+class TestInput:
+
+    def test_input(self, web):
+        web.page = ContentsPage
+        web.page.home_page.gallery_button.click()
+        web.page.gallery_page.text_input.send_keys('citronella')
+        web.page.gallery_page.add_button.click()
+        elements = web.page.gallery_page.text_lists.get_elements()
+        assert 'citronella' in [x.text for x in elements]
+```
+
+Even though this module is mainly designed for the page object model, it can also be used without it for quick prototyping or mockups, etc.
+```python
+from selenium import webdriver
+from selenium.webdriver.common.by import By
+from citronella import WebPage
 
-    def test_accessibility_page(self, web):
-        web.page_object(ApiDemosPage)
 
-        web.page.accessibility_button.click()
-        assert web.page.accessibility_node_provider_button.get_element().is_visible()
+driver = webdriver.Chrome()
 
-    def test_animation_page(self, web):
-        web.back
-        web.page.animation_button.click()
-        assert web.page.cloning_button.get_element().is_visible()
-
-    def test_app_page(self, web):
-        web.back
-        web.page.app_button.click()
-        assert web.page.activity_button.get_element().is_visible()
-
-    def test_os_page(self, web):
-        web.back
-        web.page.os_button.click()
-        assert web.page.morse_code_button.get_element().is_visible()
+web = WebPage(driver, webdriver_wait=20, logger=False)
+web.driver.get('https://pypi.org/')
+
+web.locate(By.ID, 'search').get_element().send_keys('citronella')
+web.locate(By.XPATH, '//button[@type="submit"]/i').get_element().click()
+
+elements = web.locate(By.XPATH, '//span[@class="package-snippet__name"]')
+if elements.ec_visibility_of_all_elements_located():
+    results = elements.get_elements()
+    text_lists = [x.text for x in results]
 ```
+
 ___
 ## Install Package
 
 ```bash
 pip install citronella
 ```
 
 ___
 ## Documentation
 
-There are only three modules imported in this package:
+There are only two modules import in this package:
 
 * The first module is for conftest.py.
 
 ### Selenium
 
 ```python
 import pytest
@@ -158,64 +145,131 @@
     options.platformName = 'Android'
     options.app = os.getcwd() + '/APK/ApiDemos-debug.apk.zip'
     driver = webdriver.Remote('http://127.0.0.1:4723/wd/hub', options=options)
     yield WebPage(driver)
     driver.quit()
 ```
 
-* The second and third modules are for the page object model.
-
-[Check out this link for more information on the Page Object Design.](https://github.com/heyclore/citronella/tree/main/python/example#readme)
+* The second module are for the page object model.
 
 ### Selenium
 
 ```python
 from selenium.webdriver.common.by import By
-from citronella import Ui, PlaceholderPage
-from Pages.component.HeaderMenu import HeaderMenu
+from citronella import ui
+from Pages.contents_page import ContentsPage
 
 
-class HomePage(HeaderMenu):
+class HomePage(ContentsPage().header()):
 
     def some_button(self):
-        return Ui(By.XPATH, '//a[@name="foo"]')
+        return ui(By.XPATH, '//a[@name="foo"]')
 
     def search_input(self):
-        return Ui(By.ID, 'search')
+        return ui(By.ID, 'search')
 
     def search_button(self):
-        from Pages.SearchPage import SearchPage
-        return Ui(By.NAME, 'search-button', SearchPage)
-
-    def link_to_somewhere_currently_dont_have_page_object(self):
-        return Ui(By.NAME, 'search-button', PlaceholderPage)
+        return ui(By.NAME, 'search-button')
 ```
 
 ### Appium
 
 ```python
 from appium.webdriver.common.appiumby import AppiumBy
-from citronella import Ui, PlaceholderPage
-from Pages.component.HeaderMenu import HeaderMenu
+from citronella import ui
+from Pages.contents_page import ContentsPage
 
 
-class HomePage(HeaderMenu):
+class HomePage(ContentsPage().header()):
 
     def some_button(self):
-        return Ui(AppiumBy.XPATH, '//a[@name="foo"]')
+        return ui(AppiumBy.XPATH, '//a[@name="foo"]')
 
     def search_input(self):
-        return Ui(AppiumBy.ACCESSIBILITY_ID, 'search')
+        return ui(AppiumBy.ACCESSIBILITY_ID, 'search')
 
     def search_button(self):
-        from Pages.SearchPage import SearchPage
-        return Ui(AppiumBy.ID, 'search-button', SearchPage)
+        return ui(AppiumBy.ID, 'search-button')
+```
+
+___
+## Page Object Design / Strategy
+
+There's a two ways to create a page object for `WebPage`:
+
+1. Straightforward approach: This method requires importing the page object for each test.
+```python
+from selenium import webdriver
+from selenium.webdriver.common.by import By
+from citronella import WebPage, ui
+
+
+class HomePage:
+    def auth_buton(self):
+        return ui(By.XPATH, '//a[@name="foo"]')
 
-    def link_to_somewhere_currently_dont_have_page_object(self):
-        return Ui(AppiumBy.ACCESSIBILITY_ID, 'search-button', PlaceholderPage)
+class LoginPage:
+    def email_input(self):
+        return ui(By.ID, 'email')
+
+    def password_input(self):
+        return ui(By.ID, 'password')
+
+    def login_buton(self):
+        return ui(By.ID, 'login')
+
+driver = webdriver.Chrome()
+web = WebPage(driver)
+web.driver.get('https://foobarbaz.com/')
+web.page = HomePage
+web.page.auth_button.click()
+web.page = LoginPage
+web.page.email_input.send_keys('foo')
+web.page.password_input.send_keys('bar')
+web.page.login_button.click()
+```
+
+2. Lazy loading approach: This method is slightly more complex but offers the benefit of lazy loading.
+see [ContentsPage example](https://github.com/heyclore/citronella/blob/main/python/example/selenium/Pages/contents_page.py)
+or this [Page object example](https://github.com/heyclore/citronella/tree/main/python/example/selenium/Pages)
+```python
+from selenium import webdriver
+from selenium.webdriver.common.by import By
+from citronella import WebPage, ui
+
+
+class ContentsPage:
+    def home_page(self):
+        return HomePage
+
+    def login_page(self):
+        return LoginPage
+
+class HomePage:
+    def auth_buton(self):
+        return ui(By.XPATH, '//a[@name="foo"]')
+
+class LoginPage:
+    def email_input(self):
+        return ui(By.ID, 'email')
+
+    def password_input(self):
+        return ui(By.ID, 'password')
+
+    def login_buton(self):
+        return ui(By.ID, 'login')
+
+driver = webdriver.Chrome()
+web = WebPage(driver)
+web.driver.get('https://foobarbaz.com/')
+web.page = ContentsPage
+web.page.home_page.auth_button.click()
+web.page.login_page.email_input.send_keys('foo')
+web.page.login_page.password_input.send_keys('bar')
+web.page.login_page.login_button.click()
 ```
 
 ___
 ## Usage
 
 ### citronella.WebPage
 
@@ -225,44 +279,41 @@
 ###### Kwargs (optional):
 - webdriver_wait `number(seconds)`, default value is `10`
 - logger `bool`, default value is `True`
 
 ###### Method Lists:
 | Method Name        | Args*       | Kwargs**         | Note |
 | ------------------ |:-----------:|:----------------:|:----:|
-| driver             | None        | None             | return selenium `webdriver` object |
-| locate             | by, value   | None             | similar as`driver.get_element` args |
-| page_object        | Page Object | get_start `bool` | Page Object must contain `ACTIVITY` variable with URL(selenium)/State(appium) if using Kwargs** | 
-| page               | None        | None             |      |
-| back               | None        | None             |      |
-| webdriver_wait     | number(sec) | None             |      |
-| ready_state        | number(sec) | None             | execute javascript `document.readyState` manually, default timeout is `0` |
-| get_window_size    | None        | None             |      |
-| sleep              | number(sec) | None             |      |
+| driver             | -           | -                | return selenium `webdriver` object |
+| locate             | by, value   | -                | similar as`driver.get_element` args |
+| page               | page object | -                | setter |
+| page               | -           | -                | getter |
+| webdriver_wait     | number(sec) | -                |      |
+| ready_state        | number(sec) | -                | execute javascript `document.readyState` manually, default timeout is `30` |
+| sleep              | number(sec) | -                |      |
 
 ### citronella.ui / citronella.WebUi
 
 ###### Args:
 - by
 - value
-- page_object (optional)
 
 ###### Method Lists:
 | Method Name   | Args*  | Kwargs**           | Note |
 | ------------- |:------:|:------------------:|:----:|
-| send_keys     | text   | clear `bool`, return_key `bool` | default value is `False` by default |
-| click         | None   | switch_page `bool` | see [test_auth.py](example/selenium/Test/pytest_html_image/test_auth.py) example |
-| get_element   | None   | None               |      |
-| get_elements  | None   | None               |      |
-| ec_element_to_be_clickable | None | None | wrapper of `EC` / `excpected_condition` |
-| ec_presence_of_element_located | None | None | wrapper of `EC` / `excpected_condition` |
-| ec_presence_of_all_elements_located | None | None | wrapper of `EC` / `excpected_condition` |
-| ec_visibility_of_element_located | None | None | wrapper of `EC` / `excpected_condition` |
-| ec_visibility_of_all_elements_located | None | None | wrapper of `EC` / `excpected_condition` |
-| ec_visibility_of_any_elements_located | None | None | wrapper of `EC` / `excpected_condition` |
-| ec_invisibility_of_element_located | None | None | wrapper of `EC` / `excpected_condition` |
-| ec_element_located_to_be_selected | None | None | wrapper of `EC` / `excpected_condition` |
+| send_keys     | text   | clear `bool`, return_key `bool` |     |
+| click         | -      | -                  |      |
+| get_element   | -      | -                  |      |
+| get_elements  | -      | -                  |      |
+| ec_element_to_be_clickable | -    | -    | wrapper of `EC` / `excpected_condition` |
+| ec_presence_of_element_located | -    | -    | wrapper of `EC` / `excpected_condition` |
+| ec_presence_of_all_elements_located | -    | -    | wrapper of `EC` / `excpected_condition` |
+| ec_visibility_of_element_located | -    | -    | wrapper of `EC` / `excpected_condition` |
+| ec_visibility_of_all_elements_located | -    | -    | wrapper of `EC` / `excpected_condition` |
+| ec_visibility_of_any_elements_located | -    | -    | wrapper of `EC` / `excpected_condition` |
+| ec_invisibility_of_element_located | -    | -    | wrapper of `EC` / `excpected_condition` |
+| ec_element_located_to_be_selected | -    | -    | wrapper of `EC` / `excpected_condition` |
 
 
 ## Testing powered by
 <a target="_blank" href="https://www.browserstack.com/"><img width="200" src="https://www.browserstack.com/images/layout/browserstack-logo-600x315.png"></a><br>
 [BrowserStack Open-Source Program](https://www.browserstack.com/open-source)
```

### Comparing `citronella-0.0.5/test/test_navigation_menu.py` & `citronella-0.0.6/test/test_navigation_menu.py`

 * *Files identical despite different names*

