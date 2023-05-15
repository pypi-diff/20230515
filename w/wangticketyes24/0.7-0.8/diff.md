# Comparing `tmp/wangticketyes24-0.7-py3-none-any.whl.zip` & `tmp/wangticketyes24-0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 27708 bytes, number of entries: 12
--rw-r--r--  2.0 unx      114 b- defN 23-Apr-01 09:29 wangticketyes24/__init__.py
--rw-r--r--  2.0 unx    26478 b- defN 23-Apr-01 05:48 wangticketyes24/selenium_yes24.py
+Zip file size: 27816 bytes, number of entries: 12
+-rw-r--r--  2.0 unx      114 b- defN 23-May-15 13:50 wangticketyes24/__init__.py
+-rw-r--r--  2.0 unx    26992 b- defN 23-May-15 13:49 wangticketyes24/selenium_yes24.py
 -rw-r--r--  2.0 unx    42099 b- defN 23-Apr-01 09:29 wangticketyes24/yes24.py
 -rw-r--r--  2.0 unx       94 b- defN 18-Dec-12 13:54 yes24ticket/__init__.py
 -rw-r--r--  2.0 unx     7490 b- defN 18-Dec-12 14:11 yes24ticket/selenium_yes24.py
 -rw-r--r--  2.0 unx    15460 b- defN 18-Dec-12 14:12 yes24ticket/yes24test.py
--rw-r--r--  2.0 unx       61 b- defN 23-Apr-01 09:30 wangticketyes24-0.7.dist-info/DESCRIPTION.rst
--rw-r--r--  2.0 unx      690 b- defN 23-Apr-01 09:30 wangticketyes24-0.7.dist-info/metadata.json
--rw-r--r--  2.0 unx       16 b- defN 23-Apr-01 09:30 wangticketyes24-0.7.dist-info/top_level.txt
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-01 09:30 wangticketyes24-0.7.dist-info/WHEEL
--rw-r--r--  2.0 unx      575 b- defN 23-Apr-01 09:30 wangticketyes24-0.7.dist-info/METADATA
--rw-r--r--  2.0 unx     1034 b- defN 23-Apr-01 09:30 wangticketyes24-0.7.dist-info/RECORD
-12 files, 94203 bytes uncompressed, 25974 bytes compressed:  72.4%
+-rw-r--r--  2.0 unx       61 b- defN 23-May-15 13:52 wangticketyes24-0.8.dist-info/DESCRIPTION.rst
+-rw-r--r--  2.0 unx      690 b- defN 23-May-15 13:52 wangticketyes24-0.8.dist-info/metadata.json
+-rw-r--r--  2.0 unx       16 b- defN 23-May-15 13:52 wangticketyes24-0.8.dist-info/top_level.txt
+-rw-r--r--  2.0 unx       92 b- defN 23-May-15 13:52 wangticketyes24-0.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx      575 b- defN 23-May-15 13:52 wangticketyes24-0.8.dist-info/METADATA
+-rw-r--r--  2.0 unx     1034 b- defN 23-May-15 13:52 wangticketyes24-0.8.dist-info/RECORD
+12 files, 94717 bytes uncompressed, 26082 bytes compressed:  72.5%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: yes24ticket/selenium_yes24.py
 Comment: 
 
 Filename: yes24ticket/yes24test.py
 Comment: 
 
-Filename: wangticketyes24-0.7.dist-info/DESCRIPTION.rst
+Filename: wangticketyes24-0.8.dist-info/DESCRIPTION.rst
 Comment: 
 
-Filename: wangticketyes24-0.7.dist-info/metadata.json
+Filename: wangticketyes24-0.8.dist-info/metadata.json
 Comment: 
 
-Filename: wangticketyes24-0.7.dist-info/top_level.txt
+Filename: wangticketyes24-0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: wangticketyes24-0.7.dist-info/WHEEL
+Filename: wangticketyes24-0.8.dist-info/WHEEL
 Comment: 
 
-Filename: wangticketyes24-0.7.dist-info/METADATA
+Filename: wangticketyes24-0.8.dist-info/METADATA
 Comment: 
 
-Filename: wangticketyes24-0.7.dist-info/RECORD
+Filename: wangticketyes24-0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## wangticketyes24/__init__.py

```diff
@@ -1,5 +1,5 @@
 name = "wangticketyes24"
-__version__ = "0.7"
+__version__ = "0.8"
 
 from .yes24 import Yes24
 from .selenium_yes24 import Selenium_yes24
```

## wangticketyes24/selenium_yes24.py

```diff
@@ -309,15 +309,15 @@
 		e = retry_find_element_by_xpath(self.driver, "//a[contains(@onclick,'fdc_DeliveryEnd')]")
 		self.driver.execute_script("arguments[0].click();", e)
 
 	def prepare_lastpage(self, payment_method=1, showcaptcha=True):
 		### Generating CAPTCHA if not exists
 		if self.driver.execute_script("return reCAPTCHAUse;") != 'Y' and showcaptcha:
 			print("Generating captcha system")
-			self.driver.execute_script("reCAPTCHAUse = 'Y';")
+			self.driver.execute_script("reCAPTCHAUse = 'NC';")
 			captchaHtml = """<li class="d_line">
                                       <em class="blu">자동주문방지</em>
                                       <div class="con">
                                         
                                         <img src="" id="captchaImg" width="180px">
                                         <div style="position:absolute;left:190px;top:15px;"> 
                                             <a href="javascript:initCaptcha();"><img src="http://tkfile.yes24.com/img/common/ic_refresh.png" alt="새로고침" width="12px">새로고침</a>
@@ -326,15 +326,15 @@
                                         </div>
                                       </div>
                                     </li>
 			"""
 
 			e = self.driver.find_element_by_xpath("//ul[@class='mb']")
 			self.driver.execute_script("arguments[0].innerHTML = arguments[0].innerHTML + arguments[1];", e, captchaHtml)
-			self.driver.execute_script("reCAPTCHAUse = 'Y';")
+			self.driver.execute_script("reCAPTCHAUse = 'NC';")
 			self.driver.execute_script("initCaptcha();")
 
 		# 2 credit card / 222 kakao bank / 22 bank
 		if payment_method == 1:
 			e = retry_find_element_by_xpath(self.driver, "//input[@idgroup='2']")
 			self.driver.execute_script("arguments[0].click();", e)
 		elif payment_method == 2:
@@ -355,15 +355,15 @@
 		#e = self.driver.find_element_by_id("chkinfoAgree")
 		#self.driver.execute_script("arguments[0].click();", e)
 
 	def handleCaptcha(self, captcha_self=False):
 		if captcha_self:
 			return
 
-		if self.driver.execute_script("return reCAPTCHAUse;") != 'Y':
+		if self.driver.execute_script("return reCAPTCHAUse;") != 'NC':
 			print("captcha is not needed")
 			return
 
 		## captchaKey ready??
 		while True:
 			captchaKey = self.driver.find_element_by_id("captchaKey").get_attribute("value")
 			print("captchaKey:", captchaKey)
@@ -425,19 +425,21 @@
 	def handleDialog(self):
 		ALERT1 = "자동주문방지 문자를 잘못 입력하셨습니다."
 		ALERT2 = "티켓 주문처리중 오류가 발생하였습니다."
 		#"예매 완료까지 허용된 제한 시간이 만료 되어 예매를 완료 할 수 없습니다. 다시 예매 하여 주십시오!"
 		#"오류 내용 : 좌석선점오류[62][235]"
 		#"제휴처 좌석선점에 오류가 발생하였습니다.[45][335]"
 		#티켓 주문처리중 오류가 발생하였습니다.[372]<br>예매중인 공연은 고객님 1인당 2매 까지만 예매/예약이 가능 한 공연 입니다. 기존 예매/예약분을 합하여 허용 기준을 초과 합니다
+		#티켓 주문처리중 오류가 발생하였습니다.[861]<br>팬클럽 인증 정보가 없습니다. 팬클럽 인증 확인 후 예매하여 주시기 바랍니다.
 		#""
 		ALERT3 = "자동주문방지 문자를 입력해주세요."
 		ALERT4 = "결제를 취소하셨습니다."
 		ALERT5 = "가상계좌 발급중 오류가 발생하였습니다."
 		ALERT6 = "허용 기준을 초과 합니다"
+		ALERT7 = "팬클럽 인증 정보가 없습니다."
 
 		content = self.driver.find_element_by_xpath("//div[@id='dialogAlert']")
 		contentHTML = content.get_attribute('innerHTML')
 		print("alert is displayed.", contentHTML)
 
 		btn_xpath = "//button[@aria-disabled='false']"
 		e = self.driver.find_element_by_xpath(btn_xpath)
@@ -446,14 +448,16 @@
 
 		if ALERT1 in contentHTML:
 			return 1
 		elif ALERT5 in contentHTML:
 			return 3
 		elif ALERT6 in contentHTML:
 			return 4
+		elif ALERT7 in contentHTML:
+			return 5
 		elif ALERT2 in contentHTML or ALERT4 in contentHTML:
 			return 2
 		else:
 			return -1
 
 	def enterOrderPage(self, bookno):
 		## handling popup
@@ -652,14 +656,21 @@
 						elif ret == 4:
 							msg = "[{}] 예매가능매수 초과".format(self.userid)
 							print(msg)
 							self.notifyTelegram(message=msg)
 							print("Should find new seats after 10seconds")
 							time.sleep(10)
 							return False
+						elif ret == 5:
+							msg = "[{}] 팬클럽 미인증 계정".format(self.userid)
+							print(msg)
+							self.notifyTelegram(message=msg)
+							print("Should find new seats after 10seconds")
+							time.sleep(10)
+							return False
 					elif len(inicis)>0 and inicis[0].is_displayed():
 						print("credit card checkout displayed")
 						self.notifySeatInfo()
 						self.payHyundaiCard()
 						continue
 					elif len(success)>0 and success[0].is_displayed():
 						print("SuccessBoard is ready")
```

## Comparing `wangticketyes24-0.7.dist-info/metadata.json` & `wangticketyes24-0.8.dist-info/metadata.json`

 * *Files 1% similar despite different names*

### Pretty-printed

 * *Similarity: 0.9545454545454546%*

 * *Differences: {"'version'": "'0.8'"}*

```diff
@@ -33,9 +33,9 @@
                 "beautifulsoup4",
                 "requests",
                 "selenium"
             ]
         }
     ],
     "summary": "wangticket for y",
-    "version": "0.7"
+    "version": "0.8"
 }
```

## Comparing `wangticketyes24-0.7.dist-info/METADATA` & `wangticketyes24-0.8.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.0
 Name: wangticketyes24
-Version: 0.7
+Version: 0.8
 Summary: wangticket for y
 Home-page: https://gitlab.com/wangticket/yes24-ticket
 Author: Wangticket
 Author-email: wangticket77@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `wangticketyes24-0.7.dist-info/RECORD` & `wangticketyes24-0.8.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-wangticketyes24/__init__.py,sha256=lGh34rQuMWhUWnyQ84C3DzbqPSRr-FJQCMKcqTHRPL0,114
-wangticketyes24/selenium_yes24.py,sha256=phd97fQLcY28UQ4aFnUN7RrOMCzwqZmU0H9cbdZRRN4,26478
+wangticketyes24/__init__.py,sha256=2-aIW9w48KQgr5RocuUKNVMGjOTtaiiwHDjXuBsGK2M,114
+wangticketyes24/selenium_yes24.py,sha256=Sq6mxeZGBqHfj1HkErCjeN7Xy50qkmWhSxfHs7tTNMw,26992
 wangticketyes24/yes24.py,sha256=X-RrImHk-hHnO7wE5U28Jx2ow3bwqDbiY3YO0kMmHEY,42099
-wangticketyes24-0.7.dist-info/DESCRIPTION.rst,sha256=iA1-u5zGsM2eQRcqv1-vqBiJevH0U-KhtkZxpjzmfx4,61
-wangticketyes24-0.7.dist-info/METADATA,sha256=kgIRe_3Tyn676U8zjZ9QN9O2o4KdlrG5kybfEVNTohU,575
-wangticketyes24-0.7.dist-info/RECORD,,
-wangticketyes24-0.7.dist-info/WHEEL,sha256=8Lm45v9gcYRm70DrgFGVe4WsUtUMi1_0Tso1hqPGMjA,92
-wangticketyes24-0.7.dist-info/metadata.json,sha256=iiHnWdBNuAYFvEOVJiGhQdeHoxFA-uRQy1rd3XDCaTs,690
-wangticketyes24-0.7.dist-info/top_level.txt,sha256=gHGxU_Wfy3Ly7zkKLxm67DoXktNcwN0ImDzlhzNaiW4,16
+wangticketyes24-0.8.dist-info/DESCRIPTION.rst,sha256=iA1-u5zGsM2eQRcqv1-vqBiJevH0U-KhtkZxpjzmfx4,61
+wangticketyes24-0.8.dist-info/METADATA,sha256=nwiuk092CUeJvW-kknIqCI7nktE1w4PkN40KBvZm5QM,575
+wangticketyes24-0.8.dist-info/RECORD,,
+wangticketyes24-0.8.dist-info/WHEEL,sha256=8Lm45v9gcYRm70DrgFGVe4WsUtUMi1_0Tso1hqPGMjA,92
+wangticketyes24-0.8.dist-info/metadata.json,sha256=U3tl3vd1LgbYvH30QVzRv4AEY34Wprf5HqgFWo9y15U,690
+wangticketyes24-0.8.dist-info/top_level.txt,sha256=gHGxU_Wfy3Ly7zkKLxm67DoXktNcwN0ImDzlhzNaiW4,16
 yes24ticket/__init__.py,sha256=amffzfln3WNiLWWyUul39xXObS4TmQRza8OBgfN24M8,94
 yes24ticket/selenium_yes24.py,sha256=z6ataHl-e3AVhQTZFSYPdn1OfSOklBTizd2mLA57DAM,7490
 yes24ticket/yes24test.py,sha256=6my-oQh4NITv3IkaT_W_v61Z5iPDqNmDU6b3Qx9N5l8,15460
```

