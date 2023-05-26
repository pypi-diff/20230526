# Comparing `tmp/sopel-twitter-1.0.1.tar.gz` & `tmp/sopel-twitter-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sopel-twitter-1.0.1.tar", last modified: Sun Apr 16 22:04:31 2023, max compression
+gzip compressed data, was "sopel-twitter-1.1.0.tar", last modified: Fri May 26 05:20:25 2023, max compression
```

## Comparing `sopel-twitter-1.0.1.tar` & `sopel-twitter-1.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 dgw       (1000) dgw       (1000)        0 2023-04-16 22:04:31.338235 sopel-twitter-1.0.1/
--rw-r--r--   0 dgw       (1000) dgw       (1000)     1022 2022-03-02 18:17:04.000000 sopel-twitter-1.0.1/COPYING
--rw-r--r--   0 dgw       (1000) dgw       (1000)      161 2023-04-15 06:53:37.000000 sopel-twitter-1.0.1/MANIFEST.in
--rw-r--r--   0 dgw       (1000) dgw       (1000)     2492 2023-04-16 22:03:50.000000 sopel-twitter-1.0.1/NEWS
--rw-r--r--   0 dgw       (1000) dgw       (1000)     5693 2023-04-16 22:04:31.339315 sopel-twitter-1.0.1/PKG-INFO
--rw-r--r--   0 dgw       (1000) dgw       (1000)     1298 2023-04-15 06:53:37.000000 sopel-twitter-1.0.1/README.md
--rw-r--r--   0 dgw       (1000) dgw       (1000)        0 2023-04-15 06:53:37.000000 sopel-twitter-1.0.1/dev-requirements.txt
--rw-r--r--   0 dgw       (1000) dgw       (1000)      699 2023-04-16 22:04:31.346241 sopel-twitter-1.0.1/setup.cfg
--rwxr-xr-x   0 dgw       (1000) dgw       (1000)      889 2023-04-15 06:53:37.000000 sopel-twitter-1.0.1/setup.py
-drwxr-xr-x   0 dgw       (1000) dgw       (1000)        0 2023-04-16 22:04:31.209991 sopel-twitter-1.0.1/sopel_twitter/
--rw-r--r--   0 dgw       (1000) dgw       (1000)     8588 2023-04-16 22:00:49.000000 sopel-twitter-1.0.1/sopel_twitter/__init__.py
-drwxr-xr-x   0 dgw       (1000) dgw       (1000)        0 2023-04-16 22:04:31.317003 sopel-twitter-1.0.1/sopel_twitter.egg-info/
--rw-r--r--   0 dgw       (1000) dgw       (1000)     5693 2023-04-16 22:04:30.000000 sopel-twitter-1.0.1/sopel_twitter.egg-info/PKG-INFO
--rw-r--r--   0 dgw       (1000) dgw       (1000)      400 2023-04-16 22:04:30.000000 sopel-twitter-1.0.1/sopel_twitter.egg-info/SOURCES.txt
--rw-r--r--   0 dgw       (1000) dgw       (1000)        1 2023-04-16 22:04:30.000000 sopel-twitter-1.0.1/sopel_twitter.egg-info/dependency_links.txt
--rw-r--r--   0 dgw       (1000) dgw       (1000)       41 2023-04-16 22:04:30.000000 sopel-twitter-1.0.1/sopel_twitter.egg-info/entry_points.txt
--rw-r--r--   0 dgw       (1000) dgw       (1000)        1 2023-04-15 21:13:31.000000 sopel-twitter-1.0.1/sopel_twitter.egg-info/not-zip-safe
--rw-r--r--   0 dgw       (1000) dgw       (1000)       36 2023-04-16 22:04:30.000000 sopel-twitter-1.0.1/sopel_twitter.egg-info/requires.txt
--rw-r--r--   0 dgw       (1000) dgw       (1000)       20 2023-04-16 22:04:30.000000 sopel-twitter-1.0.1/sopel_twitter.egg-info/top_level.txt
-drwxr-xr-x   0 dgw       (1000) dgw       (1000)        0 2023-04-16 22:04:31.337082 sopel-twitter-1.0.1/tests/
--rw-r--r--   0 dgw       (1000) dgw       (1000)       15 2023-04-15 06:53:37.000000 sopel-twitter-1.0.1/tests/__init__.py
--rw-r--r--   0 dgw       (1000) dgw       (1000)      296 2023-04-15 06:53:37.000000 sopel-twitter-1.0.1/tests/test_twitter.py
+drwxr-xr-x   0 dgw       (1000) dgw       (1000)        0 2023-05-26 05:20:25.428260 sopel-twitter-1.1.0/
+-rw-r--r--   0 dgw       (1000) dgw       (1000)     1022 2022-03-02 18:17:04.000000 sopel-twitter-1.1.0/COPYING
+-rw-r--r--   0 dgw       (1000) dgw       (1000)      161 2023-04-29 21:04:00.000000 sopel-twitter-1.1.0/MANIFEST.in
+-rw-r--r--   0 dgw       (1000) dgw       (1000)     2634 2023-05-18 04:45:03.000000 sopel-twitter-1.1.0/NEWS
+-rw-r--r--   0 dgw       (1000) dgw       (1000)     4506 2023-05-26 05:20:25.428760 sopel-twitter-1.1.0/PKG-INFO
+-rw-r--r--   0 dgw       (1000) dgw       (1000)     1298 2023-04-29 21:04:00.000000 sopel-twitter-1.1.0/README.md
+-rw-r--r--   0 dgw       (1000) dgw       (1000)        0 2023-04-29 21:04:00.000000 sopel-twitter-1.1.0/dev-requirements.txt
+-rw-r--r--   0 dgw       (1000) dgw       (1000)      694 2023-05-26 05:20:25.431258 sopel-twitter-1.1.0/setup.cfg
+-rwxr-xr-x   0 dgw       (1000) dgw       (1000)      889 2023-04-29 21:04:00.000000 sopel-twitter-1.1.0/setup.py
+drwxr-xr-x   0 dgw       (1000) dgw       (1000)        0 2023-05-26 05:20:25.376254 sopel-twitter-1.1.0/sopel_twitter/
+-rw-r--r--   0 dgw       (1000) dgw       (1000)     8920 2023-05-26 05:18:02.000000 sopel-twitter-1.1.0/sopel_twitter/__init__.py
+drwxr-xr-x   0 dgw       (1000) dgw       (1000)        0 2023-05-26 05:20:25.411759 sopel-twitter-1.1.0/sopel_twitter.egg-info/
+-rw-r--r--   0 dgw       (1000) dgw       (1000)     4506 2023-05-26 05:20:24.000000 sopel-twitter-1.1.0/sopel_twitter.egg-info/PKG-INFO
+-rw-r--r--   0 dgw       (1000) dgw       (1000)      400 2023-05-26 05:20:24.000000 sopel-twitter-1.1.0/sopel_twitter.egg-info/SOURCES.txt
+-rw-r--r--   0 dgw       (1000) dgw       (1000)        1 2023-05-26 05:20:24.000000 sopel-twitter-1.1.0/sopel_twitter.egg-info/dependency_links.txt
+-rw-r--r--   0 dgw       (1000) dgw       (1000)       40 2023-05-26 05:20:24.000000 sopel-twitter-1.1.0/sopel_twitter.egg-info/entry_points.txt
+-rw-r--r--   0 dgw       (1000) dgw       (1000)        1 2023-04-15 21:13:31.000000 sopel-twitter-1.1.0/sopel_twitter.egg-info/not-zip-safe
+-rw-r--r--   0 dgw       (1000) dgw       (1000)       31 2023-05-26 05:20:24.000000 sopel-twitter-1.1.0/sopel_twitter.egg-info/requires.txt
+-rw-r--r--   0 dgw       (1000) dgw       (1000)       20 2023-05-26 05:20:24.000000 sopel-twitter-1.1.0/sopel_twitter.egg-info/top_level.txt
+drwxr-xr-x   0 dgw       (1000) dgw       (1000)        0 2023-05-26 05:20:25.427262 sopel-twitter-1.1.0/tests/
+-rw-r--r--   0 dgw       (1000) dgw       (1000)       15 2023-04-29 21:04:00.000000 sopel-twitter-1.1.0/tests/__init__.py
+-rw-r--r--   0 dgw       (1000) dgw       (1000)      296 2023-04-29 21:04:00.000000 sopel-twitter-1.1.0/tests/test_twitter.py
```

### Comparing `sopel-twitter-1.0.1/COPYING` & `sopel-twitter-1.1.0/COPYING`

 * *Files identical despite different names*

### Comparing `sopel-twitter-1.0.1/NEWS` & `sopel-twitter-1.1.0/NEWS`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+Changes between 1.0.1 and 1.1.0
+===============================
+
+Changed:
+* Updated to `tweety-ns` 0.7, including revamped exceptions (#46)
+
+
 Changes between 1.0.0 and 1.0.1
 ===============================
 
 Fixed:
 * Don't cache Tweety object; it stops working after some hours (#43)
```

### Comparing `sopel-twitter-1.0.1/README.md` & `sopel-twitter-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `sopel-twitter-1.0.1/setup.cfg` & `sopel-twitter-1.1.0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sopel-twitter
-version = 1.0.1
+version = 1.1.0
 description = A Twitter plugin for Sopel
 author = dgw
 author_email = dgw@technobabbl.es
 url = https://github.com/sopel-irc/sopel-twitter
 license = Eiffel Forum License, version 2
 classifiers = 
 	Intended Audience :: Developers
@@ -15,15 +15,15 @@
 
 [options]
 packages = find:
 zip_safe = false
 include_package_data = true
 install_requires = 
 	sopel>=7.1,<9
-	tweety-ns>=0.6.1,<0.7
+	tweety-ns~=0.7.1
 
 [options.entry_points]
 sopel.plugins = 
 	twitter = sopel_twitter
 
 [egg_info]
 tag_build =
```

### Comparing `sopel-twitter-1.0.1/setup.py` & `sopel-twitter-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `sopel-twitter-1.0.1/sopel_twitter/__init__.py` & `sopel-twitter-1.1.0/sopel_twitter/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -176,19 +176,23 @@
 
     output_user(bot, trigger, trigger.group(3))
 
 
 def output_status(bot, trigger, id_):
     try:
         tweet = Twitter().tweet_detail(id_)
+    except tweety_errors.AuthenticationRequired:
+        bot.say("That content requires authentication; sorry!")
+        return
     except tweety_errors.InvalidTweetIdentifier:
-        bot.say("Couldn't fetch that tweet. Most likely, it's either private or deleted.")
+        bot.say("Couldn't fetch that tweet. It's probably private, 18+ flagged, or deleted.")
         return
     except (
         tweety_errors.GuestTokenNotFound,
+        tweety_errors.InvalidCredentials,
         tweety_errors.ProxyParseError,
         tweety_errors.UnknownError,
     ):
         bot.say("Can't access Twitter data. Please try again later.")
         return
 
     template = "[Twitter] {tweet} | {RTs} RTs | {hearts} ♥s | Posted: {posted}"
@@ -208,47 +212,51 @@
                                 RTs=tweet.retweet_counts,
                                 hearts=tweet.likes,
                                 posted=format_time(bot, trigger, tweet.created_on)))
 
 
 def output_user(bot, trigger, sn):
     try:
-        user = Twitter(sn).get_user_info()
+        user = Twitter().get_user_info(sn)
     except tweety_errors.UserNotFound:
         bot.say("User not found.")
         return
     except tweety_errors.UserProtected:
         bot.say("User profile is protected.")
         return
+    except tweety_errors.AuthenticationRequired:
+        bot.say("That content requires authentication; sorry!")
+        return
     except (
         tweety_errors.GuestTokenNotFound,
+        tweety_errors.InvalidCredentials,
         tweety_errors.ProxyParseError,
         tweety_errors.UnknownError,
     ):
         bot.say("Can't access Twitter data. Please try again later.")
         return
 
     url = None
     try:
         url = user.entities['url']['urls'][0]['expanded_url']
     except (KeyError, IndexError):
         pass
 
-    bio = user.get('description', None)
+    bio = getattr(user, 'description', None)
     if bio:
-        for link in user['entities']['description']['urls']:  # bloody t.co everywhere
+        for link in user.entities['description']['urls']:  # bloody t.co everywhere
             bio = bio.replace(link['url'], link['expanded_url'])
         bio = tools.web.decode(bio)
 
-    message = ('[Twitter] {user[name]} (@{user[screen_name]}){verified}{protected}{location}{url}'
-               ' | {user[friends_count]:,} friends, {user[followers_count]:,} followers'
-               ' | {user[statuses_count]:,} tweets, {user[favourites_count]:,} ♥s'
+    message = ('[Twitter] {user.name} (@{user.screen_name}){verified}{protected}{location}{url}'
+               ' | {user.friends_count:,} friends, {user.followers_count:,} followers'
+               ' | {user.statuses_count:,} tweets, {user.favourites_count:,} ♥s'
                ' | Joined: {joined}{bio}').format(
                user=user,
-               verified=(' ✔️' if user['verified'] else ''),
-               protected=(' 🔒' if user['protected'] else ''),
-               location=(' | ' + user['location'] if user.get('location', None) else ''),
+               verified=(' ✔️' if user.verified else ''),
+               protected=(' 🔒' if user.protected else ''),
+               location=(' | ' + user.location if getattr(user, 'location', None) else ''),
                url=(' | ' + url if url else ''),
-               joined=format_time(bot, trigger, user['created_at']),
+               joined=format_time(bot, trigger, user.created_at),
                bio=(' | ' + bio if bio else ''))
 
     bot.say(message, truncation=' […]')
```

