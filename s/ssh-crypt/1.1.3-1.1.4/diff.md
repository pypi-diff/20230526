# Comparing `tmp/ssh-crypt-1.1.3.tar.gz` & `tmp/ssh-crypt-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssh-crypt-1.1.3.tar", last modified: Tue Dec 13 18:30:29 2022, max compression
+gzip compressed data, was "ssh-crypt-1.1.4.tar", last modified: Fri May 26 04:52:31 2023, max compression
```

## Comparing `ssh-crypt-1.1.3.tar` & `ssh-crypt-1.1.4.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxrwxr-x   0 sets      (1000) sets      (1000)        0 2022-12-13 18:30:29.409749 ssh-crypt-1.1.3/
--rw-rw-r--   0 sets      (1000) sets      (1000)       45 2022-12-13 18:26:38.000000 ssh-crypt-1.1.3/MANIFEST.in
--rw-rw-r--   0 sets      (1000) sets      (1000)     8365 2022-12-13 18:30:29.405749 ssh-crypt-1.1.3/PKG-INFO
--rw-rw-r--   0 sets      (1000) sets      (1000)     6177 2022-12-13 18:26:38.000000 ssh-crypt-1.1.3/README.md
--rw-rw-r--   0 sets      (1000) sets      (1000)     1460 2022-12-13 18:26:38.000000 ssh-crypt-1.1.3/license.txt
--rw-rw-r--   0 sets      (1000) sets      (1000)       36 2021-04-01 15:55:05.000000 ssh-crypt-1.1.3/requirements.txt
--rw-rw-r--   0 sets      (1000) sets      (1000)       38 2022-12-13 18:30:29.409749 ssh-crypt-1.1.3/setup.cfg
--rw-rw-r--   0 sets      (1000) sets      (1000)      929 2022-12-13 18:26:38.000000 ssh-crypt-1.1.3/setup.py
-drwxrwxr-x   0 sets      (1000) sets      (1000)        0 2022-12-13 18:30:29.405749 ssh-crypt-1.1.3/ssh_crypt/
--rw-rw-r--   0 sets      (1000) sets      (1000)       53 2021-04-01 15:55:05.000000 ssh-crypt-1.1.3/ssh_crypt/__init__.py
--rw-rw-r--   0 sets      (1000) sets      (1000)     9661 2022-12-13 18:26:38.000000 ssh-crypt-1.1.3/ssh_crypt/ssh_crypt.py
-drwxrwxr-x   0 sets      (1000) sets      (1000)        0 2022-12-13 18:30:29.405749 ssh-crypt-1.1.3/ssh_crypt.egg-info/
--rw-rw-r--   0 sets      (1000) sets      (1000)     8365 2022-12-13 18:30:29.000000 ssh-crypt-1.1.3/ssh_crypt.egg-info/PKG-INFO
--rw-rw-r--   0 sets      (1000) sets      (1000)      336 2022-12-13 18:30:29.000000 ssh-crypt-1.1.3/ssh_crypt.egg-info/SOURCES.txt
--rw-rw-r--   0 sets      (1000) sets      (1000)        1 2022-12-13 18:30:29.000000 ssh-crypt-1.1.3/ssh_crypt.egg-info/dependency_links.txt
--rw-rw-r--   0 sets      (1000) sets      (1000)       46 2022-12-13 18:30:29.000000 ssh-crypt-1.1.3/ssh_crypt.egg-info/entry_points.txt
--rw-rw-r--   0 sets      (1000) sets      (1000)        1 2022-12-13 18:28:36.000000 ssh-crypt-1.1.3/ssh_crypt.egg-info/not-zip-safe
--rw-rw-r--   0 sets      (1000) sets      (1000)       36 2022-12-13 18:30:29.000000 ssh-crypt-1.1.3/ssh_crypt.egg-info/requires.txt
--rw-rw-r--   0 sets      (1000) sets      (1000)       10 2022-12-13 18:30:29.000000 ssh-crypt-1.1.3/ssh_crypt.egg-info/top_level.txt
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-26 04:52:31.083265 ssh-crypt-1.1.4/
+-rw-r--r--   0 user       (501) staff       (20)       45 2022-12-09 09:10:04.000000 ssh-crypt-1.1.4/MANIFEST.in
+-rw-r--r--   0 user       (501) staff       (20)     7253 2023-05-26 04:52:31.083075 ssh-crypt-1.1.4/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)     6969 2023-05-25 14:53:13.000000 ssh-crypt-1.1.4/README.md
+-rw-r--r--   0 user       (501) staff       (20)     1460 2022-12-09 09:10:04.000000 ssh-crypt-1.1.4/license.txt
+-rw-r--r--   0 user       (501) staff       (20)       36 2021-03-30 07:40:28.000000 ssh-crypt-1.1.4/requirements.txt
+-rw-r--r--   0 user       (501) staff       (20)       38 2023-05-26 04:52:31.083316 ssh-crypt-1.1.4/setup.cfg
+-rw-r--r--   0 user       (501) staff       (20)      929 2023-05-26 04:52:08.000000 ssh-crypt-1.1.4/setup.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-26 04:52:31.081348 ssh-crypt-1.1.4/ssh_crypt/
+-rw-r--r--   0 user       (501) staff       (20)       53 2021-03-30 12:27:03.000000 ssh-crypt-1.1.4/ssh_crypt/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     9661 2022-12-13 12:12:07.000000 ssh-crypt-1.1.4/ssh_crypt/ssh_crypt.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-26 04:52:31.082537 ssh-crypt-1.1.4/ssh_crypt.egg-info/
+-rw-r--r--   0 user       (501) staff       (20)     7253 2023-05-26 04:52:31.000000 ssh-crypt-1.1.4/ssh_crypt.egg-info/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      358 2023-05-26 04:52:31.000000 ssh-crypt-1.1.4/ssh_crypt.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2023-05-26 04:52:31.000000 ssh-crypt-1.1.4/ssh_crypt.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (501) staff       (20)       45 2023-05-26 04:52:31.000000 ssh-crypt-1.1.4/ssh_crypt.egg-info/entry_points.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2023-05-26 04:52:30.000000 ssh-crypt-1.1.4/ssh_crypt.egg-info/not-zip-safe
+-rw-r--r--   0 user       (501) staff       (20)       36 2023-05-26 04:52:31.000000 ssh-crypt-1.1.4/ssh_crypt.egg-info/requires.txt
+-rw-r--r--   0 user       (501) staff       (20)       10 2023-05-26 04:52:31.000000 ssh-crypt-1.1.4/ssh_crypt.egg-info/top_level.txt
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-26 04:52:31.082675 ssh-crypt-1.1.4/tests/
+-rw-r--r--   0 user       (501) staff       (20)     8973 2021-07-29 06:27:04.000000 ssh-crypt-1.1.4/tests/test_encrypt.py
```

### Comparing `ssh-crypt-1.1.3/PKG-INFO` & `ssh-crypt-1.1.4/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,246 +1,250 @@
 Metadata-Version: 2.1
 Name: ssh-crypt
-Version: 1.1.3
+Version: 1.1.4
 Summary: ssh-crypt is a tool to encrypt/decrypt data using your ssh key from ssh-agent
-Home-page: UNKNOWN
 Author: Maxim Nikitenko
 Author-email: iam@sets88.com
 License: BSD
-Description: # Why you may need it
-        
-        Sometimes you want to keep your password inside your shell scripts
-        but it's not very safe to have raw passwords in it
-        
-        This module can help you to solve this problem by keeping your passwords encrypted.
-        
-        The idea is you have your ssh key which protected with master password(or a special device containing a key)
-        and there is an ssh-agent which can keep your ssh key(or use you key device), so you can use you key as an
-        encryption key, until you have your key in ssh-agent you can decrypt your passwords
-        inside your shell scripts, but after your ssh key been removed from your ssh-agent you(or somebody else) can't
-        use it to encrypt/decrypt passwords or other sensitive data, here how you can use it:
-        You add your ssh key to ssh-agent:
-        
-            /usr/bin/ssh-add -t 1d -k ~/.ssh/id_rsa
-        
-        You enter master password and now you have ssh key in your ssh-agent,
-        Now you can use it to encrypt passwords or other sensitive data:
-        
-            ssh-crypt -e -s 'testpassword'
-        
-        You get string which contains your encrypted password, copy it, you can use it further,
-        lets write a shell script:
-        
-            !/bin/bash
-        
-            PASS='{V|B;*R$Ep:HtO~*;QAd?yR#b?V9~a34?!!sxqQT%{!x)bNby^5'
-        
-            mysql -h localhost -u testuser -p$(ssh-crypt -d -s $PASS)
-        
-        now you don't have raw password inside your shell script anymore, while this encrypted password
-        can be decrypted only if your ssh key still in your ssh-agent
-        
-        
-        Also you can use it just to encrypt/decrypt files like here:
-        
-            ssh-crypt -e -i /tmp/rawfile -o /tmp/encrypted_file
-            ssh-crypt -d -i /tmp/encrypted_file -o /tmp/rawfile
-        
-        
-        # How it works
-        
-        When you encrypt your password it generates random bytes, which signed by you ssh key
-        from your ssh-agent, then it creates sha3_256 from this signature and uses it as a key
-        to encrypt your data with AES and creating base85 of it if binary mode is not enabled
-        
-        ![How encryption works](/data/encryption.png)
-        
-        When you decrypt your password it takes nonce bytes from the string you pass, signs it with your ssh key,
-        creates sha3_256 from it and uses it as a AES key to decrypt the rest of data
-        
-        ![How decryption works](/data/decryption.png)
-        
-        
-        # How to install it
-        
-            pip install ssh-crypt
-        
-        # How to use it in python scripts
-        
-        ```python
-        from ssh_crypt import E
-        
-        super_secret_password = str(E('{V|B;*R$Ep:HtO~*;QAd?yR#b?V9~a34?!!sxqQT%{!x)bNby^5'))
-        ```
-        
-        # Using yubiko keys to keep your ssh key
-        
-        ## Install yubico-piv-tool
-        
-        Download it from https://developers.yubico.com/yubico-piv-tool/Releases/ or from (brew, apt, yum, or pacman)
-        
-        ## SSH Key
-        
-        Generate new key
-        
-            ssh-keygen -b 2048 -t rsa -m PEM
-        
-        or alter current key to PEM format
-        
-            ssh-keygen -p -m PEM
-        
-        unfortunately 4096 and longer RSA keys are not supported by PIV specification
-        
-        ## Import key to yubikey
-        
-        Slot 9a only can be used to store rsa key
-        
-            yubico-piv-tool --touch-policy=cached -s 9a -a import-key --pin-policy=once -i id_rsa
-        
-        ## Add card to ssh-agent
-        
-        Remove old card if exists (as if it was previously added next command will not work even if "ssh-add -D" executed)
-        
-            ssh-add -e /usr/local/lib/libykcs11.dylib
-        
-        Add new card
-        
-            ssh-add -s /usr/local/lib/libykcs11.dylib
-        
-        Enter Yubikey PIN when it's asked for passphrase for PKCS#11
-        All set up now but you have to confirm decryption by touching yubico button
-        if it't not convinient for you to touch button all the time you can disable this behaviour by removeing
-        "--touch-policy=cached" param during key import
-        
-        
-        # Use it with apps which demands config files which have to contain some token or password
-        
-        Just create a shell script with which you can access your application here is an example:
-        
-        ```bash
-        #! /bin/bash
-        
-        TOKEN='{V|B;*R$Ep:HtO~*;QAd?yR#b?V9~a34?!!sxqQT%{!x)bNby^5'
-        
-        CONFIG="apiVersion: v1
-        clusters:
-        - cluster:
-            certificate-authority-data: ***somesertdata**
-            server: https://kuber-api-host:6443
-          name: app
-        contexts:
-        - context:
-            cluster: app
-            namespace: some-namespace
-            user: max
-          name: app
-        current-context: app
-        kind: Config
-        preferences: {}
-        users:
-        - name: max
-          user:
-            token:
-             $(ssh-crypt -d -s $TOKEN)
-        "
-        
-        kubectl --kubeconfig <(echo "$CONFIG") $*
-        ```
-        
-        # Using SSH-Agent Forwarding
-        
-        There is an option to use scripts with encrypted passwords in it on remote hosts, by connecting to it via ssh like this
-        
-            ssh -A user@somehost
-        
-        "-A" parameter enables SSH-Agent forwarding.
-        **Beware!** never use this technique if you don't fully trust remote host
-        as someone who has enough permissions on that host may use your ssh agent for bad purpose 
-        
-        
-        # Options
-        
-        -h, --help
-        
-        Prints brief usage information.
-        
-        -e, --encrypt
-        
-        Encrypt incomming data
-        
-        Examples:
-        
-            ssh-crypt -e -s 'testpassword'
-            echo 'testpassword' | ssh-crypt -e
-        
-        
-        -d, --decrypt
-        
-        Decrypt incomming data, encrypt mode will be enabled if not set
-        
-        Examples:
-        
-            ssh-crypt -d -s '{V|B;*R$Ep:HtO~*;QAd?yR#b?V9~a34?!!sxqQT%{!x)bNby^5'
-            echo '{V|B;*R$Ep:HtO~*;QAd?yR#b?V9~a34?!!sxqQT%{!x)bNby^5' | ssh-crypt -e
-        
-        
-        -i, --input
-        
-        Input file, STDIN will be used if not set
-        
-        Examples:
-        
-            ssh-crypt -e -i /tmp/testfile
-            ssh-crypt -d -i /tmp/testfile
-            ssh-crypt -e -b -i /tmp/testfile
-        
-        
-        -o, --output
-        
-        Output file, STDOUT will be used if not set
-        
-        Examples:
-        
-            ssh-crypt -e -s 'testpassword' -o /tmp/testfile
-            echo 'testpassword' | ssh-crypt -e -o /tmp/testfile
-        
-        
-        -s, --string
-        
-        Use passed string as an input data
-        
-        Examples:
-        
-            ssh-crypt -e -s 'testpassword'
-            ssh-crypt -d -s '{V|B;*R$Ep:HtO~*;QAd?yR#b?V9~a34?!!sxqQT%{!x)bNby^5'
-        
-        
-        -b, --binary
-        
-        Not use base85(used to make encrypted data look more like text file, to allow to copy it inside shell scripts) for payload
-        
-        Examples:
-        
-            ssh-crypt -e -s 'testpassword' -b -o /tmp/testfile
-            ssh-crypt -e -i /tmp/testfile -b
-        
-        
-        -k, --key
-        
-        Pick key from ssh-agent keys list by its fingerprint
-        
-            ssh-add -l -E md5
-            2048 MD5:12:34:56:78:90:ab:cd:ef:01:23:34:56:78:90:12:34 Public key for PIV Authentication (RSA)
-        
-        Examples:
-        
-            ssh-crypt -e -s 'testpassword' --key '12:34:56:78:90:ab:cd:ef:01:23:34:56:78:90:12:34'
-            ssh-crypt -d -s '{V|B;*R$Ep:HtO~*;QAd?yR#b?V9~a34?!!sxqQT%{!x)bNby^5' -k '12:34:56:78:90:ab:cd:ef:01:23:34:56:78:90:12:34'
-        
-        
-        # Bugs
-        
-        See github issues: https://github.com/Sets88/ssh-crypt/issues
-        
 Platform: any
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
+
+# Why you may need it
+
+Sometimes, you may need to store passwords within your shell scripts, but doing so in plain text is a major security risk.
+
+Fortunately, this module can help you keep your passwords encrypted and secure.
+
+Here's how it works: you protect your ssh key with a master password or a special device, and then use the ssh-agent
+to keep your ssh key (or use your key device). This allows you to use your key as an encryption key, and decrypt your
+passwords within your shell scripts while your key is in the ssh-agent. However, once your ssh key is removed
+from the ssh-agent, neither you nor anyone else can use it to encrypt or decrypt sensitive data.
+To use this module, simply add your ssh key to the ssh-agent:
+
+    /usr/bin/ssh-add -t 1d -k ~/.ssh/id_rsa
+
+After entering your master password, your ssh key is now stored in the ssh-agent. You can use it
+to encrypt passwords or other sensitive data securely:
+
+    ssh-crypt -e -s 'testpassword'
+
+Once you have encrypted your password, you will receive a string containing the encrypted data.
+You can copy this string and use it as needed. To automate this process, you can write a shell script:
+
+    !/bin/bash
+
+    PASS='{V|B;*R$Ep:HtO~*;QAd?yR#b?V9~a34?!!sxqQT%{!x)bNby^5'
+
+    mysql -h localhost -u testuser -p$(ssh-crypt -d -s $PASS)
+
+By using this module, you no longer need to store raw passwords within your shell scripts.
+Instead, you can use encrypted passwords that can only be decrypted if your ssh key is still stored in
+the ssh-agent. This ensures that your sensitive data remains secure and protected from unauthorized access.
+
+In addition to encrypting and decrypting passwords, this module can also be used to encrypt and
+decrypt files. This provides an extra layer of security for your sensitive data, ensuring
+that it remains protected from prying eyes.
+
+    ssh-crypt -e -i /tmp/rawfile -o /tmp/encrypted_file
+    ssh-crypt -d -i /tmp/encrypted_file -o /tmp/rawfile
+
+
+# How it works
+
+When you encrypt your password using this module, it generates random bytes that are signed by
+your ssh key from your ssh-agent. It then creates a sha3_256 hash from this signature and uses
+it as a key to encrypt your data with AES. If binary mode is not enabled, it also creates
+a base85 representation of the encrypted data. This process ensures that your sensitive data
+is encrypted using a strong key and is protected from unauthorized access.
+
+![How encryption works](/data/encryption.png)
+
+When you decrypt your password using this module, it takes the nonce bytes from the string
+you pass and signs it with your ssh key. It then creates a sha3_256 hash from this signature
+and uses it as an AES key to decrypt the rest of the data.
+
+![How decryption works](/data/decryption.png)
+
+
+# How to install it
+
+    pip install ssh-crypt
+
+# How to use it in python scripts
+
+```python
+from ssh_crypt import E
+
+super_secret_password = str(E('{V|B;*R$Ep:HtO~*;QAd?yR#b?V9~a34?!!sxqQT%{!x)bNby^5'))
+```
+
+# Using yubiko keys to keep your ssh key
+
+## Install yubico-piv-tool
+
+Download it from https://developers.yubico.com/yubico-piv-tool/Releases/ or from (brew, apt, yum, or pacman)
+
+## SSH Key
+
+Generate new key
+
+    ssh-keygen -b 2048 -t rsa -m PEM
+
+or alter current key to PEM format
+
+    ssh-keygen -p -m PEM
+
+unfortunately 4096 and longer RSA keys are not supported by PIV specification
+
+## Import key to yubikey
+
+Slot 9a only can be used to store rsa key
+
+    yubico-piv-tool --touch-policy=cached -s 9a -a import-key --pin-policy=once -i id_rsa
+
+## Add card to ssh-agent
+
+Remove old card if exists (as if it was previously added next command will not work even if "ssh-add -D" executed)
+
+    ssh-add -e /usr/local/lib/libykcs11.dylib
+
+Add new card
+
+    ssh-add -s /usr/local/lib/libykcs11.dylib
+
+Enter Yubikey PIN when it's asked for passphrase for PKCS#11
+All set up now but you have to confirm decryption by touching yubico button
+if it't not convinient for you to touch button all the time you can disable this behaviour by removeing
+"--touch-policy=cached" param during key import
+
+
+# Use it with apps which demands config files which have to contain some token or password
+
+Just create a shell script with which you can access your application here is an example:
+
+```bash
+#! /bin/bash
+
+TOKEN='{V|B;*R$Ep:HtO~*;QAd?yR#b?V9~a34?!!sxqQT%{!x)bNby^5'
+
+CONFIG="apiVersion: v1
+clusters:
+- cluster:
+    certificate-authority-data: ***somesertdata**
+    server: https://kuber-api-host:6443
+  name: app
+contexts:
+- context:
+    cluster: app
+    namespace: some-namespace
+    user: max
+  name: app
+current-context: app
+kind: Config
+preferences: {}
+users:
+- name: max
+  user:
+    token:
+     $(ssh-crypt -d -s $TOKEN)
+"
+
+kubectl --kubeconfig <(echo "$CONFIG") $*
+```
+
+# Using SSH-Agent Forwarding
+
+This module also allows you to use scripts with encrypted passwords on remote hosts by connecting to them via ssh.
+This can be done by using the ssh-agent to forward your ssh key to the remote host, allowing you to decrypt
+the passwords within your scripts on the remote host.
+
+    ssh -A user@somehost
+
+"-A" parameter enables SSH-Agent forwarding.
+**Beware!** never use this technique if you don't fully trust remote host
+as someone who has enough permissions on remote host may use your ssh agent for bad purpose
+
+
+# Options
+
+-h, --help
+
+Prints brief usage information.
+
+-e, --encrypt
+
+Encrypt incomming data
+
+Examples:
+
+    ssh-crypt -e -s 'testpassword'
+    echo 'testpassword' | ssh-crypt -e
+
+
+-d, --decrypt
+
+Decrypt incomming data, encrypt mode will be enabled if not set
+
+Examples:
+
+    ssh-crypt -d -s '{V|B;*R$Ep:HtO~*;QAd?yR#b?V9~a34?!!sxqQT%{!x)bNby^5'
+    echo '{V|B;*R$Ep:HtO~*;QAd?yR#b?V9~a34?!!sxqQT%{!x)bNby^5' | ssh-crypt -e
+
+
+-i, --input
+
+Input file, STDIN will be used if not set
+
+Examples:
+
+    ssh-crypt -e -i /tmp/testfile
+    ssh-crypt -d -i /tmp/testfile
+    ssh-crypt -e -b -i /tmp/testfile
+
+
+-o, --output
+
+Output file, STDOUT will be used if not set
+
+Examples:
+
+    ssh-crypt -e -s 'testpassword' -o /tmp/testfile
+    echo 'testpassword' | ssh-crypt -e -o /tmp/testfile
+
+
+-s, --string
+
+Use passed string as an input data
+
+Examples:
+
+    ssh-crypt -e -s 'testpassword'
+    ssh-crypt -d -s '{V|B;*R$Ep:HtO~*;QAd?yR#b?V9~a34?!!sxqQT%{!x)bNby^5'
+
+
+-b, --binary
+
+Not use base85(used to make encrypted data look more like text file, to allow to copy it inside shell scripts) for payload
+
+Examples:
+
+    ssh-crypt -e -s 'testpassword' -b -o /tmp/testfile
+    ssh-crypt -e -i /tmp/testfile -b
+
+
+-k, --key
+
+Pick key from ssh-agent keys list by its fingerprint
+
+    ssh-add -l -E md5
+    2048 MD5:12:34:56:78:90:ab:cd:ef:01:23:34:56:78:90:12:34 Public key for PIV Authentication (RSA)
+
+Examples:
+
+    ssh-crypt -e -s 'testpassword' --key '12:34:56:78:90:ab:cd:ef:01:23:34:56:78:90:12:34'
+    ssh-crypt -d -s '{V|B;*R$Ep:HtO~*;QAd?yR#b?V9~a34?!!sxqQT%{!x)bNby^5' -k '12:34:56:78:90:ab:cd:ef:01:23:34:56:78:90:12:34'
+
+
+# Bugs
+
+See github issues: https://github.com/Sets88/ssh-crypt/issues
```

### Comparing `ssh-crypt-1.1.3/README.md` & `ssh-crypt-1.1.4/ssh_crypt.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,57 +1,71 @@
+Metadata-Version: 2.1
+Name: ssh-crypt
+Version: 1.1.4
+Summary: ssh-crypt is a tool to encrypt/decrypt data using your ssh key from ssh-agent
+Author: Maxim Nikitenko
+Author-email: iam@sets88.com
+License: BSD
+Platform: any
+Requires-Python: >=3.5
+Description-Content-Type: text/markdown
+
 # Why you may need it
 
-Sometimes you want to keep your password inside your shell scripts
-but it's not very safe to have raw passwords in it
+Sometimes, you may need to store passwords within your shell scripts, but doing so in plain text is a major security risk.
 
-This module can help you to solve this problem by keeping your passwords encrypted.
+Fortunately, this module can help you keep your passwords encrypted and secure.
 
-The idea is you have your ssh key which protected with master password(or a special device containing a key)
-and there is an ssh-agent which can keep your ssh key(or use you key device), so you can use you key as an
-encryption key, until you have your key in ssh-agent you can decrypt your passwords
-inside your shell scripts, but after your ssh key been removed from your ssh-agent you(or somebody else) can't
-use it to encrypt/decrypt passwords or other sensitive data, here how you can use it:
-You add your ssh key to ssh-agent:
+Here's how it works: you protect your ssh key with a master password or a special device, and then use the ssh-agent
+to keep your ssh key (or use your key device). This allows you to use your key as an encryption key, and decrypt your
+passwords within your shell scripts while your key is in the ssh-agent. However, once your ssh key is removed
+from the ssh-agent, neither you nor anyone else can use it to encrypt or decrypt sensitive data.
+To use this module, simply add your ssh key to the ssh-agent:
 
     /usr/bin/ssh-add -t 1d -k ~/.ssh/id_rsa
 
-You enter master password and now you have ssh key in your ssh-agent,
-Now you can use it to encrypt passwords or other sensitive data:
+After entering your master password, your ssh key is now stored in the ssh-agent. You can use it
+to encrypt passwords or other sensitive data securely:
 
     ssh-crypt -e -s 'testpassword'
 
-You get string which contains your encrypted password, copy it, you can use it further,
-lets write a shell script:
+Once you have encrypted your password, you will receive a string containing the encrypted data.
+You can copy this string and use it as needed. To automate this process, you can write a shell script:
 
     !/bin/bash
 
     PASS='{V|B;*R$Ep:HtO~*;QAd?yR#b?V9~a34?!!sxqQT%{!x)bNby^5'
 
     mysql -h localhost -u testuser -p$(ssh-crypt -d -s $PASS)
 
-now you don't have raw password inside your shell script anymore, while this encrypted password
-can be decrypted only if your ssh key still in your ssh-agent
-
-
-Also you can use it just to encrypt/decrypt files like here:
+By using this module, you no longer need to store raw passwords within your shell scripts.
+Instead, you can use encrypted passwords that can only be decrypted if your ssh key is still stored in
+the ssh-agent. This ensures that your sensitive data remains secure and protected from unauthorized access.
+
+In addition to encrypting and decrypting passwords, this module can also be used to encrypt and
+decrypt files. This provides an extra layer of security for your sensitive data, ensuring
+that it remains protected from prying eyes.
 
     ssh-crypt -e -i /tmp/rawfile -o /tmp/encrypted_file
     ssh-crypt -d -i /tmp/encrypted_file -o /tmp/rawfile
 
 
 # How it works
 
-When you encrypt your password it generates random bytes, which signed by you ssh key
-from your ssh-agent, then it creates sha3_256 from this signature and uses it as a key
-to encrypt your data with AES and creating base85 of it if binary mode is not enabled
+When you encrypt your password using this module, it generates random bytes that are signed by
+your ssh key from your ssh-agent. It then creates a sha3_256 hash from this signature and uses
+it as a key to encrypt your data with AES. If binary mode is not enabled, it also creates
+a base85 representation of the encrypted data. This process ensures that your sensitive data
+is encrypted using a strong key and is protected from unauthorized access.
 
 ![How encryption works](/data/encryption.png)
 
-When you decrypt your password it takes nonce bytes from the string you pass, signs it with your ssh key,
-creates sha3_256 from it and uses it as a AES key to decrypt the rest of data
+When you decrypt your password using this module, it takes the nonce bytes from the string
+you pass and signs it with your ssh key. It then creates a sha3_256 hash from this signature
+and uses it as an AES key to decrypt the rest of the data.
 
 ![How decryption works](/data/decryption.png)
 
 
 # How to install it
 
     pip install ssh-crypt
@@ -136,21 +150,23 @@
 "
 
 kubectl --kubeconfig <(echo "$CONFIG") $*
 ```
 
 # Using SSH-Agent Forwarding
 
-There is an option to use scripts with encrypted passwords in it on remote hosts, by connecting to it via ssh like this
+This module also allows you to use scripts with encrypted passwords on remote hosts by connecting to them via ssh.
+This can be done by using the ssh-agent to forward your ssh key to the remote host, allowing you to decrypt
+the passwords within your scripts on the remote host.
 
     ssh -A user@somehost
 
 "-A" parameter enables SSH-Agent forwarding.
 **Beware!** never use this technique if you don't fully trust remote host
-as someone who has enough permissions on that host may use your ssh agent for bad purpose 
+as someone who has enough permissions on remote host may use your ssh agent for bad purpose
 
 
 # Options
 
 -h, --help
 
 Prints brief usage information.
```

### Comparing `ssh-crypt-1.1.3/license.txt` & `ssh-crypt-1.1.4/license.txt`

 * *Files identical despite different names*

### Comparing `ssh-crypt-1.1.3/setup.py` & `ssh-crypt-1.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
             return f.readlines()
     except FileNotFoundError:
         raise RuntimeError('No requirements info found.')
 
 
 setup(
     name='ssh-crypt',
-    version='1.1.3',
+    version='1.1.4',
     license='BSD',
     author='Maxim Nikitenko',
     author_email='iam@sets88.com',
     packages=find_packages(),
     description='ssh-crypt is a tool to encrypt/decrypt data using your ssh key from ssh-agent',\
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

### Comparing `ssh-crypt-1.1.3/ssh_crypt/ssh_crypt.py` & `ssh-crypt-1.1.4/ssh_crypt/ssh_crypt.py`

 * *Files identical despite different names*

### Comparing `ssh-crypt-1.1.3/ssh_crypt.egg-info/PKG-INFO` & `ssh-crypt-1.1.4/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,246 +1,239 @@
-Metadata-Version: 2.1
-Name: ssh-crypt
-Version: 1.1.3
-Summary: ssh-crypt is a tool to encrypt/decrypt data using your ssh key from ssh-agent
-Home-page: UNKNOWN
-Author: Maxim Nikitenko
-Author-email: iam@sets88.com
-License: BSD
-Description: # Why you may need it
-        
-        Sometimes you want to keep your password inside your shell scripts
-        but it's not very safe to have raw passwords in it
-        
-        This module can help you to solve this problem by keeping your passwords encrypted.
-        
-        The idea is you have your ssh key which protected with master password(or a special device containing a key)
-        and there is an ssh-agent which can keep your ssh key(or use you key device), so you can use you key as an
-        encryption key, until you have your key in ssh-agent you can decrypt your passwords
-        inside your shell scripts, but after your ssh key been removed from your ssh-agent you(or somebody else) can't
-        use it to encrypt/decrypt passwords or other sensitive data, here how you can use it:
-        You add your ssh key to ssh-agent:
-        
-            /usr/bin/ssh-add -t 1d -k ~/.ssh/id_rsa
-        
-        You enter master password and now you have ssh key in your ssh-agent,
-        Now you can use it to encrypt passwords or other sensitive data:
-        
-            ssh-crypt -e -s 'testpassword'
-        
-        You get string which contains your encrypted password, copy it, you can use it further,
-        lets write a shell script:
-        
-            !/bin/bash
-        
-            PASS='{V|B;*R$Ep:HtO~*;QAd?yR#b?V9~a34?!!sxqQT%{!x)bNby^5'
-        
-            mysql -h localhost -u testuser -p$(ssh-crypt -d -s $PASS)
-        
-        now you don't have raw password inside your shell script anymore, while this encrypted password
-        can be decrypted only if your ssh key still in your ssh-agent
-        
-        
-        Also you can use it just to encrypt/decrypt files like here:
-        
-            ssh-crypt -e -i /tmp/rawfile -o /tmp/encrypted_file
-            ssh-crypt -d -i /tmp/encrypted_file -o /tmp/rawfile
-        
-        
-        # How it works
-        
-        When you encrypt your password it generates random bytes, which signed by you ssh key
-        from your ssh-agent, then it creates sha3_256 from this signature and uses it as a key
-        to encrypt your data with AES and creating base85 of it if binary mode is not enabled
-        
-        ![How encryption works](/data/encryption.png)
-        
-        When you decrypt your password it takes nonce bytes from the string you pass, signs it with your ssh key,
-        creates sha3_256 from it and uses it as a AES key to decrypt the rest of data
-        
-        ![How decryption works](/data/decryption.png)
-        
-        
-        # How to install it
-        
-            pip install ssh-crypt
-        
-        # How to use it in python scripts
-        
-        ```python
-        from ssh_crypt import E
-        
-        super_secret_password = str(E('{V|B;*R$Ep:HtO~*;QAd?yR#b?V9~a34?!!sxqQT%{!x)bNby^5'))
-        ```
-        
-        # Using yubiko keys to keep your ssh key
-        
-        ## Install yubico-piv-tool
-        
-        Download it from https://developers.yubico.com/yubico-piv-tool/Releases/ or from (brew, apt, yum, or pacman)
-        
-        ## SSH Key
-        
-        Generate new key
-        
-            ssh-keygen -b 2048 -t rsa -m PEM
-        
-        or alter current key to PEM format
-        
-            ssh-keygen -p -m PEM
-        
-        unfortunately 4096 and longer RSA keys are not supported by PIV specification
-        
-        ## Import key to yubikey
-        
-        Slot 9a only can be used to store rsa key
-        
-            yubico-piv-tool --touch-policy=cached -s 9a -a import-key --pin-policy=once -i id_rsa
-        
-        ## Add card to ssh-agent
-        
-        Remove old card if exists (as if it was previously added next command will not work even if "ssh-add -D" executed)
-        
-            ssh-add -e /usr/local/lib/libykcs11.dylib
-        
-        Add new card
-        
-            ssh-add -s /usr/local/lib/libykcs11.dylib
-        
-        Enter Yubikey PIN when it's asked for passphrase for PKCS#11
-        All set up now but you have to confirm decryption by touching yubico button
-        if it't not convinient for you to touch button all the time you can disable this behaviour by removeing
-        "--touch-policy=cached" param during key import
-        
-        
-        # Use it with apps which demands config files which have to contain some token or password
-        
-        Just create a shell script with which you can access your application here is an example:
-        
-        ```bash
-        #! /bin/bash
-        
-        TOKEN='{V|B;*R$Ep:HtO~*;QAd?yR#b?V9~a34?!!sxqQT%{!x)bNby^5'
-        
-        CONFIG="apiVersion: v1
-        clusters:
-        - cluster:
-            certificate-authority-data: ***somesertdata**
-            server: https://kuber-api-host:6443
-          name: app
-        contexts:
-        - context:
-            cluster: app
-            namespace: some-namespace
-            user: max
-          name: app
-        current-context: app
-        kind: Config
-        preferences: {}
-        users:
-        - name: max
-          user:
-            token:
-             $(ssh-crypt -d -s $TOKEN)
-        "
-        
-        kubectl --kubeconfig <(echo "$CONFIG") $*
-        ```
-        
-        # Using SSH-Agent Forwarding
-        
-        There is an option to use scripts with encrypted passwords in it on remote hosts, by connecting to it via ssh like this
-        
-            ssh -A user@somehost
-        
-        "-A" parameter enables SSH-Agent forwarding.
-        **Beware!** never use this technique if you don't fully trust remote host
-        as someone who has enough permissions on that host may use your ssh agent for bad purpose 
-        
-        
-        # Options
-        
-        -h, --help
-        
-        Prints brief usage information.
-        
-        -e, --encrypt
-        
-        Encrypt incomming data
-        
-        Examples:
-        
-            ssh-crypt -e -s 'testpassword'
-            echo 'testpassword' | ssh-crypt -e
-        
-        
-        -d, --decrypt
-        
-        Decrypt incomming data, encrypt mode will be enabled if not set
-        
-        Examples:
-        
-            ssh-crypt -d -s '{V|B;*R$Ep:HtO~*;QAd?yR#b?V9~a34?!!sxqQT%{!x)bNby^5'
-            echo '{V|B;*R$Ep:HtO~*;QAd?yR#b?V9~a34?!!sxqQT%{!x)bNby^5' | ssh-crypt -e
-        
-        
-        -i, --input
-        
-        Input file, STDIN will be used if not set
-        
-        Examples:
-        
-            ssh-crypt -e -i /tmp/testfile
-            ssh-crypt -d -i /tmp/testfile
-            ssh-crypt -e -b -i /tmp/testfile
-        
-        
-        -o, --output
-        
-        Output file, STDOUT will be used if not set
-        
-        Examples:
-        
-            ssh-crypt -e -s 'testpassword' -o /tmp/testfile
-            echo 'testpassword' | ssh-crypt -e -o /tmp/testfile
-        
-        
-        -s, --string
-        
-        Use passed string as an input data
-        
-        Examples:
-        
-            ssh-crypt -e -s 'testpassword'
-            ssh-crypt -d -s '{V|B;*R$Ep:HtO~*;QAd?yR#b?V9~a34?!!sxqQT%{!x)bNby^5'
-        
-        
-        -b, --binary
-        
-        Not use base85(used to make encrypted data look more like text file, to allow to copy it inside shell scripts) for payload
-        
-        Examples:
-        
-            ssh-crypt -e -s 'testpassword' -b -o /tmp/testfile
-            ssh-crypt -e -i /tmp/testfile -b
-        
-        
-        -k, --key
-        
-        Pick key from ssh-agent keys list by its fingerprint
-        
-            ssh-add -l -E md5
-            2048 MD5:12:34:56:78:90:ab:cd:ef:01:23:34:56:78:90:12:34 Public key for PIV Authentication (RSA)
-        
-        Examples:
-        
-            ssh-crypt -e -s 'testpassword' --key '12:34:56:78:90:ab:cd:ef:01:23:34:56:78:90:12:34'
-            ssh-crypt -d -s '{V|B;*R$Ep:HtO~*;QAd?yR#b?V9~a34?!!sxqQT%{!x)bNby^5' -k '12:34:56:78:90:ab:cd:ef:01:23:34:56:78:90:12:34'
-        
-        
-        # Bugs
-        
-        See github issues: https://github.com/Sets88/ssh-crypt/issues
-        
-Platform: any
-Requires-Python: >=3.5
-Description-Content-Type: text/markdown
+# Why you may need it
+
+Sometimes, you may need to store passwords within your shell scripts, but doing so in plain text is a major security risk.
+
+Fortunately, this module can help you keep your passwords encrypted and secure.
+
+Here's how it works: you protect your ssh key with a master password or a special device, and then use the ssh-agent
+to keep your ssh key (or use your key device). This allows you to use your key as an encryption key, and decrypt your
+passwords within your shell scripts while your key is in the ssh-agent. However, once your ssh key is removed
+from the ssh-agent, neither you nor anyone else can use it to encrypt or decrypt sensitive data.
+To use this module, simply add your ssh key to the ssh-agent:
+
+    /usr/bin/ssh-add -t 1d -k ~/.ssh/id_rsa
+
+After entering your master password, your ssh key is now stored in the ssh-agent. You can use it
+to encrypt passwords or other sensitive data securely:
+
+    ssh-crypt -e -s 'testpassword'
+
+Once you have encrypted your password, you will receive a string containing the encrypted data.
+You can copy this string and use it as needed. To automate this process, you can write a shell script:
+
+    !/bin/bash
+
+    PASS='{V|B;*R$Ep:HtO~*;QAd?yR#b?V9~a34?!!sxqQT%{!x)bNby^5'
+
+    mysql -h localhost -u testuser -p$(ssh-crypt -d -s $PASS)
+
+By using this module, you no longer need to store raw passwords within your shell scripts.
+Instead, you can use encrypted passwords that can only be decrypted if your ssh key is still stored in
+the ssh-agent. This ensures that your sensitive data remains secure and protected from unauthorized access.
+
+In addition to encrypting and decrypting passwords, this module can also be used to encrypt and
+decrypt files. This provides an extra layer of security for your sensitive data, ensuring
+that it remains protected from prying eyes.
+
+    ssh-crypt -e -i /tmp/rawfile -o /tmp/encrypted_file
+    ssh-crypt -d -i /tmp/encrypted_file -o /tmp/rawfile
+
+
+# How it works
+
+When you encrypt your password using this module, it generates random bytes that are signed by
+your ssh key from your ssh-agent. It then creates a sha3_256 hash from this signature and uses
+it as a key to encrypt your data with AES. If binary mode is not enabled, it also creates
+a base85 representation of the encrypted data. This process ensures that your sensitive data
+is encrypted using a strong key and is protected from unauthorized access.
+
+![How encryption works](/data/encryption.png)
+
+When you decrypt your password using this module, it takes the nonce bytes from the string
+you pass and signs it with your ssh key. It then creates a sha3_256 hash from this signature
+and uses it as an AES key to decrypt the rest of the data.
+
+![How decryption works](/data/decryption.png)
+
+
+# How to install it
+
+    pip install ssh-crypt
+
+# How to use it in python scripts
+
+```python
+from ssh_crypt import E
+
+super_secret_password = str(E('{V|B;*R$Ep:HtO~*;QAd?yR#b?V9~a34?!!sxqQT%{!x)bNby^5'))
+```
+
+# Using yubiko keys to keep your ssh key
+
+## Install yubico-piv-tool
+
+Download it from https://developers.yubico.com/yubico-piv-tool/Releases/ or from (brew, apt, yum, or pacman)
+
+## SSH Key
+
+Generate new key
+
+    ssh-keygen -b 2048 -t rsa -m PEM
+
+or alter current key to PEM format
+
+    ssh-keygen -p -m PEM
+
+unfortunately 4096 and longer RSA keys are not supported by PIV specification
+
+## Import key to yubikey
+
+Slot 9a only can be used to store rsa key
+
+    yubico-piv-tool --touch-policy=cached -s 9a -a import-key --pin-policy=once -i id_rsa
+
+## Add card to ssh-agent
+
+Remove old card if exists (as if it was previously added next command will not work even if "ssh-add -D" executed)
+
+    ssh-add -e /usr/local/lib/libykcs11.dylib
+
+Add new card
+
+    ssh-add -s /usr/local/lib/libykcs11.dylib
+
+Enter Yubikey PIN when it's asked for passphrase for PKCS#11
+All set up now but you have to confirm decryption by touching yubico button
+if it't not convinient for you to touch button all the time you can disable this behaviour by removeing
+"--touch-policy=cached" param during key import
+
+
+# Use it with apps which demands config files which have to contain some token or password
+
+Just create a shell script with which you can access your application here is an example:
+
+```bash
+#! /bin/bash
+
+TOKEN='{V|B;*R$Ep:HtO~*;QAd?yR#b?V9~a34?!!sxqQT%{!x)bNby^5'
+
+CONFIG="apiVersion: v1
+clusters:
+- cluster:
+    certificate-authority-data: ***somesertdata**
+    server: https://kuber-api-host:6443
+  name: app
+contexts:
+- context:
+    cluster: app
+    namespace: some-namespace
+    user: max
+  name: app
+current-context: app
+kind: Config
+preferences: {}
+users:
+- name: max
+  user:
+    token:
+     $(ssh-crypt -d -s $TOKEN)
+"
+
+kubectl --kubeconfig <(echo "$CONFIG") $*
+```
+
+# Using SSH-Agent Forwarding
+
+This module also allows you to use scripts with encrypted passwords on remote hosts by connecting to them via ssh.
+This can be done by using the ssh-agent to forward your ssh key to the remote host, allowing you to decrypt
+the passwords within your scripts on the remote host.
+
+    ssh -A user@somehost
+
+"-A" parameter enables SSH-Agent forwarding.
+**Beware!** never use this technique if you don't fully trust remote host
+as someone who has enough permissions on remote host may use your ssh agent for bad purpose
+
+
+# Options
+
+-h, --help
+
+Prints brief usage information.
+
+-e, --encrypt
+
+Encrypt incomming data
+
+Examples:
+
+    ssh-crypt -e -s 'testpassword'
+    echo 'testpassword' | ssh-crypt -e
+
+
+-d, --decrypt
+
+Decrypt incomming data, encrypt mode will be enabled if not set
+
+Examples:
+
+    ssh-crypt -d -s '{V|B;*R$Ep:HtO~*;QAd?yR#b?V9~a34?!!sxqQT%{!x)bNby^5'
+    echo '{V|B;*R$Ep:HtO~*;QAd?yR#b?V9~a34?!!sxqQT%{!x)bNby^5' | ssh-crypt -e
+
+
+-i, --input
+
+Input file, STDIN will be used if not set
+
+Examples:
+
+    ssh-crypt -e -i /tmp/testfile
+    ssh-crypt -d -i /tmp/testfile
+    ssh-crypt -e -b -i /tmp/testfile
+
+
+-o, --output
+
+Output file, STDOUT will be used if not set
+
+Examples:
+
+    ssh-crypt -e -s 'testpassword' -o /tmp/testfile
+    echo 'testpassword' | ssh-crypt -e -o /tmp/testfile
+
+
+-s, --string
+
+Use passed string as an input data
+
+Examples:
+
+    ssh-crypt -e -s 'testpassword'
+    ssh-crypt -d -s '{V|B;*R$Ep:HtO~*;QAd?yR#b?V9~a34?!!sxqQT%{!x)bNby^5'
+
+
+-b, --binary
+
+Not use base85(used to make encrypted data look more like text file, to allow to copy it inside shell scripts) for payload
+
+Examples:
+
+    ssh-crypt -e -s 'testpassword' -b -o /tmp/testfile
+    ssh-crypt -e -i /tmp/testfile -b
+
+
+-k, --key
+
+Pick key from ssh-agent keys list by its fingerprint
+
+    ssh-add -l -E md5
+    2048 MD5:12:34:56:78:90:ab:cd:ef:01:23:34:56:78:90:12:34 Public key for PIV Authentication (RSA)
+
+Examples:
+
+    ssh-crypt -e -s 'testpassword' --key '12:34:56:78:90:ab:cd:ef:01:23:34:56:78:90:12:34'
+    ssh-crypt -d -s '{V|B;*R$Ep:HtO~*;QAd?yR#b?V9~a34?!!sxqQT%{!x)bNby^5' -k '12:34:56:78:90:ab:cd:ef:01:23:34:56:78:90:12:34'
+
+
+# Bugs
+
+See github issues: https://github.com/Sets88/ssh-crypt/issues
```

