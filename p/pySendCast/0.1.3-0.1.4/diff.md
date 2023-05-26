# Comparing `tmp/pySendCast-0.1.3.tar.gz` & `tmp/pySendCast-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pySendCast-0.1.3.tar", last modified: Tue Sep 22 08:56:09 2020, max compression
+gzip compressed data, was "pySendCast-0.1.4.tar", last modified: Fri May 26 10:57:00 2023, max compression
```

## Comparing `pySendCast-0.1.3.tar` & `pySendCast-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2020-09-22 08:56:09.445408 pySendCast-0.1.3/
--rw-rw-rw-   0        0        0     5690 2020-09-22 08:56:09.444431 pySendCast-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     3711 2020-09-22 08:17:40.000000 pySendCast-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2020-09-22 08:56:09.419025 pySendCast-0.1.3/pySendCast/
--rw-rw-rw-   0        0        0       36 2019-09-08 11:33:11.000000 pySendCast-0.1.3/pySendCast/__init__.py
--rw-rw-rw-   0        0        0      408 2020-01-15 13:21:33.000000 pySendCast-0.1.3/pySendCast/__main__.py
--rw-rw-rw-   0        0        0     4077 2020-01-15 13:01:03.000000 pySendCast-0.1.3/pySendCast/bcast.py
--rw-rw-rw-   0        0        0     1760 2019-09-08 11:33:11.000000 pySendCast-0.1.3/pySendCast/recv.py
--rw-rw-rw-   0        0        0     1555 2020-09-22 08:15:00.000000 pySendCast-0.1.3/pySendCast/send.py
-drwxrwxrwx   0        0        0        0 2020-09-22 08:56:09.443453 pySendCast-0.1.3/pySendCast.egg-info/
--rw-rw-rw-   0        0        0     5690 2020-09-22 08:56:09.000000 pySendCast-0.1.3/pySendCast.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      295 2020-09-22 08:56:09.000000 pySendCast-0.1.3/pySendCast.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-09-22 08:56:09.000000 pySendCast-0.1.3/pySendCast.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2020-09-22 08:56:09.000000 pySendCast-0.1.3/pySendCast.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       11 2020-09-22 08:56:09.000000 pySendCast-0.1.3/pySendCast.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2020-09-22 08:56:09.445408 pySendCast-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1129 2020-09-22 08:19:08.000000 pySendCast-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 10:57:00.483610 pySendCast-0.1.4/
+-rw-rw-rw-   0        0        0     1057 2019-09-08 11:33:11.000000 pySendCast-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0     4758 2023-05-26 10:57:00.482610 pySendCast-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3955 2023-05-26 10:56:01.000000 pySendCast-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-26 10:57:00.475611 pySendCast-0.1.4/pySendCast/
+-rw-rw-rw-   0        0        0       36 2019-09-08 11:33:11.000000 pySendCast-0.1.4/pySendCast/__init__.py
+-rw-rw-rw-   0        0        0      408 2020-01-15 13:21:33.000000 pySendCast-0.1.4/pySendCast/__main__.py
+-rw-rw-rw-   0        0        0     4446 2023-05-26 10:49:51.000000 pySendCast-0.1.4/pySendCast/bcast.py
+-rw-rw-rw-   0        0        0     1868 2023-05-26 10:51:38.000000 pySendCast-0.1.4/pySendCast/recv.py
+-rw-rw-rw-   0        0        0     1767 2023-05-26 10:51:32.000000 pySendCast-0.1.4/pySendCast/send.py
+drwxrwxrwx   0        0        0        0 2023-05-26 10:57:00.480610 pySendCast-0.1.4/pySendCast.egg-info/
+-rw-rw-rw-   0        0        0     4758 2023-05-26 10:57:00.000000 pySendCast-0.1.4/pySendCast.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      303 2023-05-26 10:57:00.000000 pySendCast-0.1.4/pySendCast.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 10:57:00.000000 pySendCast-0.1.4/pySendCast.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-05-26 10:57:00.000000 pySendCast-0.1.4/pySendCast.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       11 2023-05-26 10:57:00.000000 pySendCast-0.1.4/pySendCast.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-26 10:57:00.483610 pySendCast-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1129 2023-05-26 07:34:54.000000 pySendCast-0.1.4/setup.py
```

### Comparing `pySendCast-0.1.3/README.md` & `pySendCast-0.1.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 # pySendCast
 A pure Python cross-platform program to send and receive data over local area network(LAN) with on-the-fly gzip streaming and broadcasting
 
+### Important note
+On firewall environments like Windows, set TCP port 18902 allowed. This port is used to transfer gzip stream. On Windows, it should be also checked that the network you are sending files over is set to be a private network.
+
 ### How to install
 ```
 pip install pySendCast
 ```
 
 ### How to use
 ```
```

### Comparing `pySendCast-0.1.3/pySendCast/bcast.py` & `pySendCast-0.1.4/pySendCast/bcast.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,51 +1,53 @@
 from time import sleep
 from logging import info, debug, warn, critical, error
-from socket import socket
+from socket import socket, timeout
 import struct
 import sys
 
 BCAST_PORT = 31023 # 31022 for sync_play
 BCAST_MAGIC = 'ch.ideas_bcast.py'
 
 class BroadCastSocket(socket):
   def __init__(self, port=None, magic=None):
     from socket import AF_INET, SOCK_DGRAM
     super().__init__(AF_INET, SOCK_DGRAM)#, IPPROTO_UDP
     super().setblocking(True)
-    #super().setblocking(False)
-    #super().settimeout(0)
+    super().settimeout(1)
     self.bcast_port = port or BCAST_PORT
     self.magic = (BCAST_MAGIC + (('_'+magic) if magic else '')).encode()
   
   def set_iface(self, iface):
     from sys import platform
     if platform == 'win32': return
     from socket import SOL_SOCKET, SO_BINDTODEVICE
     super().setsockopt(SOL_SOCKET, SO_BINDTODEVICE, iface.encode())
 
   def wait(self, num=0):
     pass
 
+# Receiving side is Server
 class BroadCastServSocket(BroadCastSocket):
   def __init__(self, port=None, magic=None):
     super().__init__(port, magic)
     from socket import AF_INET, SOL_SOCKET, SO_BROADCAST
     super().bind(('', 0))
     super().setsockopt(SOL_SOCKET, SO_BROADCAST, 1)
-    super().settimeout(0)
     from sys import platform
     if platform == 'win32':
-      from socket import inet_aton, getaddrinfo, gethostname
-      addrs = getaddrinfo(gethostname(), 0, family=AF_INET)
-      #ip = max(addrs, key=lambda v:int.from_bytes(inet_aton(v[-1][0]), 'big'))[-1][0]
-      #self.bcast_addr = ip[:ip.rindex('.')+1]+'255'
-      self.bcast_addrs = [v[:v.rindex('.')+1]+'255' for v in list(map(lambda v:v[-1][0], addrs))]
+      from socket import gethostbyname_ex, gethostname
+      self.bcast_addrs = [ip[:ip.rindex('.')+1]+'255' for ip in gethostbyname_ex(gethostname())[2] if not ip.startswith('127.')]
+    #  from socket import inet_aton, getaddrinfo, gethostname
+    #  addrs = getaddrinfo(gethostname(), 0, family=AF_INET)
+    #  #ip = max(addrs, key=lambda v:int.from_bytes(inet_aton(v[-1][0]), 'big'))[-1][0]
+    #  self.bcast_addrs = [v[:v.rindex('.')+1]+'255' for v in list(map(lambda v:v[-1][0], addrs))]
+    #  #self.bcast_addr = '255.255.255.255'
     else:
       self.bcast_addrs = ['<broadcast>']
+    #print('broadcasting to', self.bcast_addrs)
 
   def send(self, data):
     #info('server sending : %s', data)
     try:
       #super().sendto(data, (self.bcast_addr, self.bcast_port))
       for addr in self.bcast_addrs:
         #print('server sending : %s to %s:%s', data, addr, self.bcast_port)
@@ -55,32 +57,39 @@
 
   def announce(self):
     self.send(self.magic)
 
   def announce_loop(self):
     try:
       while True:
-        self.announce()
+        try:
+          self.announce()
+        except timeout:
+          pass
         sleep(1)
     except KeyboardInterrupt:
       print('finishing announce loop')
 
+# Sending side is Client
 class BroadCastCliSocket(BroadCastSocket):
   def __init__(self, port=None, magic=None):
     super().__init__(port, magic)
     from socket import SOL_SOCKET, SO_REUSEADDR
     super().setsockopt(SOL_SOCKET, SO_REUSEADDR, 1)
     self.serv_addr = []
     super().bind(('', self.bcast_port))
 
   def discovery(self):
-    data, addr = super().recvfrom(len(self.magic)+2)
-    #print('discovered message :', data)
-    #print('discovered from :', addr)
-    return None if data[:len(self.magic)] != self.magic else addr
+    try:
+      data, addr = super().recvfrom(len(self.magic)+2)
+      #print('discovered message :', data)
+      #print('discovered from :', addr)
+      return None if data[:len(self.magic)] != self.magic else addr
+    except timeout:
+      return None
     #if not addr in self.serv_addr:
     #  self.serv_addr.append(addr)
     #  print('added to server address :', addr)
   
   def send(self, data):
     if self.serv_addr is None: return
     super().sendto(data, self.serv_addr)
@@ -113,15 +122,17 @@
 
 def test(is_serv):
   sock = (BroadCastServSocket if is_serv else BroadCastCliSocket)()
   try:
     if is_serv:
       sock.announce_loop()
     else:
-      print('discovered :', sock.discovery())
+      while not sock.discovery():
+        pass
   except KeyboardInterrupt:
+    print('test is canceled')
     sock.close()
 
 if __name__ == '__main__':
   from sys import argv
   is_serv = len(argv)>1 and argv[1]=='s'
   test(is_serv)#, '' if len(argv)<3 else argv[2]) #argv[2] if len(argv)>2 and argv[2] else '')
```

### Comparing `pySendCast-0.1.3/pySendCast/recv.py` & `pySendCast-0.1.4/pySendCast/recv.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,18 +22,19 @@
       print('generated PIN :', pin)
     else: pin = argv[1]
   else: pin = ''
   with socket.socket() as s:
     s.bind(('', 18902))
     s.setblocking(True)
     s.settimeout(1)
-    s.listen(1)
+    s.listen()
     try:
       while True:
         with BroadCastServSocket(magic='sendfile'+pin) as sa:
+          print('announcing')
           sa.announce()
         try:
           c, a = s.accept()
           print(a[0]) # ip address
           from .send import isurl
           with tarfile.open(fileobj=c.makefile('rb', buffering=0), mode='r|gz') as t:
             timeit.gc.disable()
@@ -46,16 +47,18 @@
                 continue
               print('extracting %s (%d bytes)'%(ti.name,ti.size))
               t0=timeit.default_timer()
               t.extract(ti)
               t0=timeit.default_timer()-t0
               print('extracting %s done (%d bytes, %f seconds, %f MB/s)'%(ti.name,ti.size, t0, ti.size/t0/10**6))
             timeit.gc.enable()
-            break
+            break # complete -> break loop
         except socket.timeout:
           continue
     except KeyboardInterrupt:
       s.close()
+      print('user canceled receiving')
+      return 1
 
 if __name__ == '__main__':
   from sys import argv
   main(argv)
```

### Comparing `pySendCast-0.1.3/pySendCast/send.py` & `pySendCast-0.1.4/pySendCast/send.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,47 +9,53 @@
   from string import digits
   return ''.join(choices(digits, k=length))
 
 def isurl(s):
   return s.startswith(('http://','https://'))
 
 def main(argv):
-  srv_addr = None
+  srv_addr, pin = None, ''
   if len(argv) > 1:
     if argv[1] in ('-up', '--userpin') and len(argv)>4:
       pin=argv[2]
       print('user PIN :', pin)
       argv = [argv[0]] + argv[3:]
     elif argv[1] in ('-p', '--pin'):
       pin=mkpin()
       print('generated PIN :', pin)
       argv = [argv[0]] + argv[2:]
     elif argv[1] in ('-r', '--recv', '--receiver'):
-      pin=''
       srv_addr = (argv[2],)
-    else: pin=''
-  else: pin=''
-  with BroadCastCliSocket(magic='sendfile'+pin) as s:
-    try:
+
+  try:
+    with BroadCastCliSocket(magic='sendfile'+pin) as s:
       while srv_addr is None:
-        srv_addr = s.discovery()
-      print(srv_addr[0])
-    except KeyboardInterrupt:
-      s.close()
-  print('sending to :', (srv_addr[0], 18902))
-  with socket.create_connection((srv_addr[0], 18902)) as s:
-    with tarfile.open(fileobj=s.makefile('wb', buffering=0), mode='w|gz') as t:
-      for a in argv[1:]:
-        isMessage = isurl(a)
-        if not isMessage:
-          files = list(glob.iglob(a))
-          isMessage |= 0 == len(files)
-        if isMessage:
-          t.addfile(tarfile.TarInfo(a))
-        else:
-          for f in files:
-            print('sending %s' %f)
-            t.add(f, arcname=basename(f))
+        try:
+          srv_addr = s.discovery()
+        except socket.timeout:
+          pass
+    print('sending to :', (srv_addr[0], 18902))
+    while True:
+      try:
+        with socket.create_connection((srv_addr[0], 18902), timeout=1) as s:
+          with tarfile.open(fileobj=s.makefile('wb', buffering=0), mode='w|gz') as t:
+            for a in argv[1:]:
+              isMessage = isurl(a)
+              if not isMessage:
+                files = list(glob.iglob(a))
+                isMessage |= 0 == len(files)
+              if isMessage:
+                t.addfile(tarfile.TarInfo(a))
+              else:
+                for f in files:
+                  print('sending %s' %f)
+                  t.add(f, arcname=basename(f))
+            return 0
+      except socket.timeout:
+        pass
+  except KeyboardInterrupt:
+    print('user canceled sending')
+    return 1
   
 if __name__ == '__main__':
   from sys import argv
   main(argv)
```

### Comparing `pySendCast-0.1.3/setup.py` & `pySendCast-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 long_description = open('README.md').read()
 if type(long_description) is bytes:
   long_description = long_description.decode()
 
 setup(
     name='pySendCast',
-    version='0.1.3',
+    version='0.1.4',
     author='Ch.Idea',
     author_email='sbw228@gmail.com',
     description='A pure Python cross-platform program to send and receive data over local area network(LAN) with on-the-fly gzip streaming and broadcasting',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/chidea/pySendCast',
     packages=find_packages(),
```

