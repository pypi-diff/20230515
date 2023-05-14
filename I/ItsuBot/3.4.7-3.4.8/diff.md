# Comparing `tmp/ItsuBot-3.4.7.tar.gz` & `tmp/ItsuBot-3.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ItsuBot-3.4.7.tar", last modified: Sun May 14 22:41:30 2023, max compression
+gzip compressed data, was "dist\ItsuBot-3.4.8.tar", last modified: Sun May 14 23:39:38 2023, max compression
```

## Comparing `ItsuBot-3.4.7.tar` & `ItsuBot-3.4.8.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 22:41:30.000000 ItsuBot-3.4.7/
-drwxrwxrwx   0        0        0        0 2023-05-14 22:41:30.000000 ItsuBot-3.4.7/ItsuBot/
--rw-rw-rw-   0        0        0    64902 2023-05-14 22:40:49.000000 ItsuBot-3.4.7/ItsuBot/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-14 22:41:30.000000 ItsuBot-3.4.7/ItsuBot.egg-info/
--rw-rw-rw-   0        0        0      358 2023-05-14 22:41:29.000000 ItsuBot-3.4.7/ItsuBot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      152 2023-05-14 22:41:30.000000 ItsuBot-3.4.7/ItsuBot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 22:41:29.000000 ItsuBot-3.4.7/ItsuBot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-14 22:41:29.000000 ItsuBot-3.4.7/ItsuBot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      358 2023-05-14 22:41:30.000000 ItsuBot-3.4.7/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-14 22:41:30.000000 ItsuBot-3.4.7/setup.cfg
--rw-rw-rw-   0        0        0      384 2023-05-14 22:41:10.000000 ItsuBot-3.4.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 23:39:38.000000 ItsuBot-3.4.8/
+drwxrwxrwx   0        0        0        0 2023-05-14 23:39:38.000000 ItsuBot-3.4.8/ItsuBot/
+-rw-rw-rw-   0        0        0    64899 2023-05-14 23:03:04.000000 ItsuBot-3.4.8/ItsuBot/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-14 23:39:38.000000 ItsuBot-3.4.8/ItsuBot.egg-info/
+-rw-rw-rw-   0        0        0      358 2023-05-14 23:39:38.000000 ItsuBot-3.4.8/ItsuBot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      152 2023-05-14 23:39:38.000000 ItsuBot-3.4.8/ItsuBot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 23:39:38.000000 ItsuBot-3.4.8/ItsuBot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-14 23:39:38.000000 ItsuBot-3.4.8/ItsuBot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      358 2023-05-14 23:39:38.000000 ItsuBot-3.4.8/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-14 23:39:38.000000 ItsuBot-3.4.8/setup.cfg
+-rw-rw-rw-   0        0        0      384 2023-05-14 23:39:18.000000 ItsuBot-3.4.8/setup.py
```

### Comparing `ItsuBot-3.4.7/ItsuBot/__init__.py` & `ItsuBot-3.4.8/ItsuBot/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1178,15 +1178,15 @@
     async def cid(self, ctx: fortnitepy.ext.commands.Context, character_id: str) -> None:
         await self.party.me.set_outfit(asset=character_id,variants=self.party.me.create_variants(profile_banner='ProfileBanner'))
         await ctx.send(f'Skin set to {character_id}.')
         os.system('clear')
 
     @is_admin()
     @commands.command()
-    async def repl(self, ctx: fortnitepy.ext.commands.Context) -> None:
+    async def r(self, ctx: fortnitepy.ext.commands.Context) -> None:
         await ctx.send(f'{self.url}')
 
     @commands.command()
     async def eid(self, ctx: fortnitepy.ext.commands.Context, emote_id: str) -> None:
         await self.party.me.clear_emote()
         await self.party.me.set_emote(asset=emote_id)
         await ctx.send(f'Emote set to {emote_id}!')
```

#### html2text {}

```diff
@@ -447,15 +447,15 @@
 (asset='CID_VIP_Athena_Commando_M_GalileoGondola_SG') await ctx.send('Skin set
 to Star Wars Hologram!') @commands.command() async def cid(self, ctx:
 fortnitepy.ext.commands.Context, character_id: str) -> None: await
 self.party.me.set_outfit
 (asset=character_id,variants=self.party.me.create_variants
 (profile_banner='ProfileBanner')) await ctx.send(f'Skin set to
 {character_id}.') os.system('clear') @is_admin() @commands.command() async def
-repl(self, ctx: fortnitepy.ext.commands.Context) -> None: await ctx.send(f'
+r(self, ctx: fortnitepy.ext.commands.Context) -> None: await ctx.send(f'
 {self.url}') @commands.command() async def eid(self, ctx:
 fortnitepy.ext.commands.Context, emote_id: str) -> None: await
 self.party.me.clear_emote() await self.party.me.set_emote(asset=emote_id) await
 ctx.send(f'Emote set to {emote_id}!') os.system('clear') @commands.command()
 async def stop(self, ctx: fortnitepy.ext.commands.Context) -> None: await
 self.party.me.clear_emote() await ctx.send('Stopped emoting.') os.system
 ('clear') @commands.command() async def point(self, ctx:
```

