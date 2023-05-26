# Comparing `tmp/fyerspysdk1-1.5-py3-none-any.whl.zip` & `tmp/fyerspysdk1-1.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 12401 bytes, number of entries: 9
+Zip file size: 12619 bytes, number of entries: 9
 -rw-rw-r--  2.0 unx       20 b- defN 23-May-22 12:28 fyerstest/__init__.py
--rw-rw-r--  2.0 unx    16456 b- defN 23-May-23 06:08 fyerstest/fyersApi.py
--rw-rw-r--  2.0 unx    16544 b- defN 23-May-23 06:09 fyerstest/hsmFyers.py
--rw-rw-r--  2.0 unx     8236 b- defN 23-May-23 06:09 fyerstest/ws.py
--rwxrwxr-x  2.0 unx     1063 b- defN 23-May-23 06:09 fyerspysdk1-1.5.dist-info/LICENSE.txt
--rw-rw-r--  2.0 unx      622 b- defN 23-May-23 06:09 fyerspysdk1-1.5.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-23 06:09 fyerspysdk1-1.5.dist-info/WHEEL
--rw-rw-r--  2.0 unx       10 b- defN 23-May-23 06:09 fyerspysdk1-1.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      705 b- defN 23-May-23 06:09 fyerspysdk1-1.5.dist-info/RECORD
-9 files, 43748 bytes uncompressed, 11193 bytes compressed:  74.4%
+-rw-rw-r--  2.0 unx    16942 b- defN 23-May-23 12:11 fyerstest/fyersApi.py
+-rw-rw-r--  2.0 unx    18823 b- defN 23-May-26 12:43 fyerstest/hsmFyers.py
+-rw-rw-r--  2.0 unx     8276 b- defN 23-May-23 12:17 fyerstest/ws.py
+-rwxrwxr-x  2.0 unx     1063 b- defN 23-May-26 12:48 fyerspysdk1-1.6.dist-info/LICENSE.txt
+-rw-rw-r--  2.0 unx      622 b- defN 23-May-26 12:48 fyerspysdk1-1.6.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-26 12:48 fyerspysdk1-1.6.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       10 b- defN 23-May-26 12:48 fyerspysdk1-1.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      705 b- defN 23-May-26 12:48 fyerspysdk1-1.6.dist-info/RECORD
+9 files, 46553 bytes uncompressed, 11411 bytes compressed:  75.5%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: fyerstest/hsmFyers.py
 Comment: 
 
 Filename: fyerstest/ws.py
 Comment: 
 
-Filename: fyerspysdk1-1.5.dist-info/LICENSE.txt
+Filename: fyerspysdk1-1.6.dist-info/LICENSE.txt
 Comment: 
 
-Filename: fyerspysdk1-1.5.dist-info/METADATA
+Filename: fyerspysdk1-1.6.dist-info/METADATA
 Comment: 
 
-Filename: fyerspysdk1-1.5.dist-info/WHEEL
+Filename: fyerspysdk1-1.6.dist-info/WHEEL
 Comment: 
 
-Filename: fyerspysdk1-1.5.dist-info/top_level.txt
+Filename: fyerspysdk1-1.6.dist-info/top_level.txt
 Comment: 
 
-Filename: fyerspysdk1-1.5.dist-info/RECORD
+Filename: fyerspysdk1-1.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fyerstest/fyersApi.py

```diff
@@ -42,89 +42,113 @@
     dataVendorTD = 'truedata-ws'
     # multi_orders = 'orders-multi'
     sync_multi_order =  '/multi-order/sync'
     multi_orders = '/multi-order'
     history = '/history'
     quotes = '/quotes'
     market_depth = '/depth'
+    error_response = {"code":404 , "message":"The requested URL was not found"}
 
 class FyersServiceSync:
 
     def __init__(self):
         self.content = 'application/json'    
 
     def postCall(self, api, header, data=None):
-        response = requests.post(Config.Api+api,data=json.dumps(data),headers={'Authorization':header, 'Content-Type': self.content})
-        return response.json()
-    
+        try:
+
+            response = requests.post(Config.Api+api,data=json.dumps(data),headers={'Authorization':header, 'Content-Type': self.content})
+            return response.json()
+        except:
+            return Config.error_response
 
     def getCall(self, api, header, data=None,data_flag=False):
-        if data_flag:
-            if api == '/history':
-                URL = Config.historyDataUrl + api
+        try:
+            if data_flag:
+                if api == '/history':
+                    URL = Config.historyDataUrl + api
+                else:
+                    URL =  Config.data_Api +api
             else:
-                URL =  Config.data_Api +api
-        else:
-            URL = Config.Api + api
+                URL = Config.Api + api
 
-        if data is not None:
-            url_params = urllib.parse.urlencode(data)
-            URL = URL+ '?' + url_params
-        response = requests.get(url = URL,headers={'Authorization':header, 'Content-Type': self.content , 'version':'2.1'})    
-        return response.json()
+            if data is not None:
+                url_params = urllib.parse.urlencode(data)
+                URL = URL+ '?' + url_params
+            response = requests.get(url = URL,headers={'Authorization':header, 'Content-Type': self.content , 'version':'2.1'})    
+            return response.json()
+        except:
+            return Config.error_response
 
     def deleteCall(self,api, header, data):
-        response =  requests.delete(url = Config.Api+api,data=json.dumps(data), headers={'Authorization':header, 'Content-Type': self.content})
-        return response.json()
+        try:
+            response =  requests.delete(url = Config.Api+api,data=json.dumps(data), headers={'Authorization':header, 'Content-Type': self.content})
+            return response.json()
+        except:
+            return Config.error_response
 
     def patchCall(self,api,header,data):
-        response = requests.patch(url = Config.Api+api,data=json.dumps(data) ,headers={'Authorization':header, 'Content-Type': self.content})
-        return response.json()
+        try:
+            response = requests.patch(url = Config.Api+api,data=json.dumps(data) ,headers={'Authorization':header, 'Content-Type': self.content})
+            return response.json()
+        except:
+            return Config.error_response
 
 class FyersServiceAsync:
 
     def __init__(self):
         self.content = 'application/json'    
 
 
     async def postAsyncCall(self,api, header, data=None):
-        async with aiohttp.ClientSession(headers={'Authorization': header, 'Content-Type': self.content}) as session:
-            url = Config.Api + api
-            async with session.post(url, data=json.dumps(data)) as response:
-                    response = await response.json()
-                    return response
+        try:
+            async with aiohttp.ClientSession(headers={'Authorization': header, 'Content-Type': self.content}) as session:
+                url = Config.Api + api
+                async with session.post(url, data=json.dumps(data)) as response:
+                        response = await response.json()
+                        return response
+        except:
+            return Config.error_response
 
     async def getAsyncCall(self, api, header, params=None, data_flag=False):
-        
-        if data_flag:
-            if api == '/history':
-                URL = Config.historyDataUrl + api
+        try:
+            if data_flag:
+                if api == '/history':
+                    URL = Config.historyDataUrl + api
+                else:
+                    URL =  Config.data_Api +api
             else:
-                URL =  Config.data_Api +api
-        else:
-            URL = Config.Api + api
-        async with aiohttp.ClientSession(headers={'Authorization': header, 'Content-Type': self.content , 'version':'2.1'}) as session:
-            async with session.get(URL, params=params) as response:
-                response_data = await response.json()
-                return response_data
+                URL = Config.Api + api
+            async with aiohttp.ClientSession(headers={'Authorization': header, 'Content-Type': self.content , 'version':'2.1'}) as session:
+                async with session.get(URL, params=params) as response:
+                    response_data = await response.json()
+                    return response_data
 
+        except:
+            return Config.error_response
 
     async def deleteAsyncCall(self, api, header, data):
-        async with aiohttp.ClientSession(headers={'Authorization': header, 'Content-Type': self.content}) as session:
-            url = Config.Api + api
-            async with session.delete(url, data=json.dumps(data)) as response:
-                return await response.json()
+        try:
+            async with aiohttp.ClientSession(headers={'Authorization': header, 'Content-Type': self.content}) as session:
+                url = Config.Api + api
+                async with session.delete(url, data=json.dumps(data)) as response:
+                    return await response.json()
+        except:
+            return Config.error_response
 
     async def patchAsyncCall(self, api, header, data):
-        async with aiohttp.ClientSession(headers={'Authorization': header, 'Content-Type': self.content}) as session:
-            url = Config.Api + api
-            json_data = json.dumps(data).encode('utf-8')
-
-            async with session.patch(url,  data=json_data ) as response:
-                return await response.json()
+        try:
+            async with aiohttp.ClientSession(headers={'Authorization': header, 'Content-Type': self.content}) as session:
+                url = Config.Api + api
+                json_data = json.dumps(data).encode('utf-8')
+
+                async with session.patch(url,  data=json_data ) as response:
+                    return await response.json()
+        except:
+            return Config.error_response
 
 
 class SessionModel:
     def __init__(self, client_id=None, redirect_uri=None, response_type=None, scope=None, state=None, nonce=None, secret_key=None, grant_type=None):
         self.client_id = client_id
         self.redirect_uri = redirect_uri
         self.response_type = response_type
@@ -158,15 +182,14 @@
 
     def generate_token(self):
         data = {
             'grant_type': self.grant_type,
             'appIdHash': self.get_hash().hexdigest(),
             'code': self.auth_token
         }
-        print("----------------------",data)
         response = requests.post(Config.authUrl+Config.generateAccessToken,headers='' ,json = data)
         return response.json()
 
 
 
 class FyersModelv3():
     '''
@@ -187,65 +210,54 @@
 
     def __init__(self, is_async=False, client_id='', token=''):
         self.client_id = client_id
         self.token = token
         self.is_async = is_async
         self.header = '{}:{}'.format(self.client_id, self.token)
         if is_async:
-            print('FyersAsyncService1')
             self.service = FyersServiceAsync()
         else:
-            print('FyersServiceSYnc')
             self.service = FyersServiceSync()
 
         
 
 
 
 
     def get_profile(self):
         '''
         Retrieves the user profile information.
 
         '''
         if self.is_async:
-            print('Tradebook async')
             response = asyncio.run(self.service.getAsyncCall(Config.get_profile, self.header))
         else:
-            print('Tradebook SYnc profile')
             response = self.service.getCall(Config.get_profile, self.header)
         return response
         
     def tradebook(self, data=None):
 
         '''
         Retrieves daily trade details of the day
 
         '''
         if self.is_async:
-            print('Tradebook async')
             response = asyncio.run(self.service.getAsyncCall(Config.tradebook, self.header , params=data))
         else:
-            print('Tradebook SYnc')
             response = self.service.getCall(Config.tradebook, self.header, data=data)
         return response
     
     def funds(self, data=None):
         '''
         Retrieves funds details
 
         '''
-
         if self.is_async:
-            
-
             response = asyncio.run(self.service.getAsyncCall(Config.funds, self.header))
         else:
-            
-
             response = self.service.getCall(Config.funds, self.header, data=data)
         return response
    
     def positions(self):
         '''
         Retrieves information about current open positions
 
@@ -260,15 +272,14 @@
         return response
    
     def holdings(self, data=None):
         '''
         Retrieves information about current open positions
 
         '''
-
         if self.is_async:
             
             response = asyncio.run(self.service.getAsyncCall(Config.holdings, self.header, params=data))
         else:
             
             response = self.service.getCall(Config.holdings, self.header, data=data)
         return response
@@ -349,19 +360,16 @@
     
     def place_order(self, data):
         '''
         Order Placement
 
         '''
         if self.is_async:
-            print('innnnns7777777')
             response = asyncio.run(self.service.postAsyncCall(Config.orders, self.header, data))
         else:  
-            print('syncc-----')
-
             response = self.service.postCall(Config.orders, self.header, data)
         return response
     
     def modify_order(self, data):
         '''
         Modify order
         
@@ -397,21 +405,22 @@
     
     def get_gttorders(self):
 
         '''
         Retrieves order details by Id
 
         '''
-
-        if self.is_async:
-            response = asyncio.run(self.service.getAsyncCall(Config.gttorders, self.header))
-        else:
-            response = self.service.getCall(Config.gttorders, self.header)
-        return response
-    
+        try:
+            if self.is_async:
+                response = asyncio.run(self.service.getAsyncCall(Config.gttorders, self.header))
+            else:
+                response = self.service.getCall(Config.gttorders, self.header)
+            return response
+        except:
+            return 
     def modify_gttorder(self, data):
             '''
             Modify order
             
             '''
             if self.is_async:
```

## fyerstest/hsmFyers.py

```diff
@@ -12,18 +12,20 @@
         self.channelNum = 1
         self.scrips = scrips
         self.channels = [1,2,3,4,5]
         self.ackCount = None
         self.updateCount = 0
         self.lite = litemode
         self.output = {}
+        self.literesp = {}
         self.resp = {}
         self.symDict = {}
+        self.ack_bool = False
 
-    def TokenByteMsg(self):
+    def token_to_byte(self):
         buffer_size = 18 + len(self.access_token) + len(self.Source)
         byte_buffer = bytearray(buffer_size)
         data_len = buffer_size - 2  
         struct.pack_into("!H", byte_buffer, 0, data_len)
         # ReqType
         byte_buffer[2] = 1 
 
@@ -55,23 +57,16 @@
         field4_id = 4
         field4_size = len(self.Source)
         struct.pack_into("!B", byte_buffer, 15+field1_size, field4_id)
         struct.pack_into("!H", byte_buffer, 16+field1_size, field4_size)
         struct.pack_into(f"!{field4_size}s", byte_buffer, 18+field1_size, self.Source.encode())
 
         return byte_buffer
-
-    def channelArray(self):
-        bits = 0
-        for channel_num in self.channels:
-            if 0 <= channel_num < 64:
-                bits |= 1 << channel_num
-        return bits
     
-    def SetToFullMode(self):
+    def full_mode_msg(self):
         data = bytearray()
 
         data.extend(struct.pack('>H', 0))
 
         data.extend(struct.pack('B', 12))
 
         data.extend(struct.pack('B', 2))
@@ -95,76 +90,93 @@
 
         data_length = len(data) - 2
         data[0] = (data_length >> 8) & 0xFF
         data[1] = data_length & 0xFF
 
         return data    
 
-    def SubscribeMsgByte(self):
+    def subscription_msg(self):
         self.scripsData = bytearray()
         self.scripsData.append(len(self.scrips) >> 8 & 0xFF)
         self.scripsData.append(len(self.scrips) & 0xFF)
         for scrip in self.scrips:
             scripBytes = scrip.encode("ascii")
             self.scripsData.append(len(scripBytes))
             self.scripsData.extend(scripBytes)
 
         dataLen = 18 + len(self.scripsData) + len(self.access_token) + len(self.Source)
         reqType = 4
         fieldCount = 2
-        buffer = bytearray()
-        buffer.extend(struct.pack(">H", dataLen))
-        buffer.append(reqType)
-        buffer.append(fieldCount)
+        buffer_msg = bytearray()
+        buffer_msg.extend(struct.pack(">H", dataLen))
+        buffer_msg.append(reqType)
+        buffer_msg.append(fieldCount)
 
         # Field-1
-        buffer.append(1)
-        buffer.extend(struct.pack(">H", len(self.scripsData)))
-        buffer.extend(self.scripsData)
+        buffer_msg.append(1)
+        buffer_msg.extend(struct.pack(">H", len(self.scripsData)))
+        buffer_msg.extend(self.scripsData)
 
         # Field-2
-        buffer.append(2) 
-        buffer.extend(struct.pack(">H", 1))
-        buffer.append(self.channelNum)
+        buffer_msg.append(2) 
+        buffer_msg.extend(struct.pack(">H", 1))
+        buffer_msg.append(self.channelNum)
+
+        return buffer_msg
 
-        return buffer
     
-    def UnSubscribeByte(self,scrips):
-        # self.channelNum = 1
+    def unsubscription_msg(self,scrips):
         scripsData = bytearray()
         scripsData.append(len(scrips) >> 8 & 0xFF)
         scripsData.append(len(scrips) & 0xFF)
         for scrip in scrips:
             scripBytes = scrip.encode("ascii")
             scripsData.append(len(scripBytes))
             scripsData.extend(scripBytes)
 
         dataLen = 18 + len(scripsData) + len(self.access_token) + len(self.Source)
         reqType = 5
         fieldCount = 2
-        buffer = bytearray()
-        buffer.extend(struct.pack(">H", dataLen))
-        buffer.append(reqType)
-        buffer.append(fieldCount)
+        buffer_msg = bytearray()
+        buffer_msg.extend(struct.pack(">H", dataLen))
+        buffer_msg.append(reqType)
+        buffer_msg.append(fieldCount)
 
         # Field-1
-        buffer.append(1) 
-        buffer.extend(struct.pack(">H", len(scripsData)))
-        buffer.extend(scripsData)
+        buffer_msg.append(1) 
+        buffer_msg.extend(struct.pack(">H", len(scripsData)))
+        buffer_msg.extend(scripsData)
 
         # Field-2
-        buffer.append(2) 
-        buffer.extend(struct.pack(">H", 1))
-        buffer.append(self.channelNum)
-
-        return buffer
-
-    def ByteToJson(self , data):
-        ValName = ["ltp","vol_traded_today" , "last_traded_time" , "ExFeedTime" , "bidSize" , "askSize" , "bidPrice" , "askPrice" , "last_traded_qty" , "tot_buy_qty" , "tot_sell_qty" ,"avg_trade_price","OI","low_price","high_price" ,"Yhigh", "Ylow", "lowCircuit" , "upCircuit" ,"open_price", "close_price"]
+        buffer_msg.append(2) 
+        buffer_msg.extend(struct.pack(">H", 1))
+        buffer_msg.append(self.channelNum)
 
+        return buffer_msg
+    
+    def ackowledgement_msg(self, messae_number):
+        total_size = 11
+        req_type = 3
+        field_count = 1
+        field_id = 1
+        field_size = 4
+        field_value = messae_number
+        buffer_msg = bytearray()
+        # Pack the data into the byte array
+        buffer_msg.extend(struct.pack('>H', total_size - 2))
+        buffer_msg.extend(struct.pack('B', req_type))
+        buffer_msg.extend(struct.pack('B', field_count))
+        buffer_msg.extend(struct.pack('B', field_id))
+        buffer_msg.extend(struct.pack('>H', field_size))
+        buffer_msg.extend(struct.pack('>I', field_value))
+        return buffer_msg
+    
+    def response_msg(self , data):
+        ValName = ["ltp","vol_traded_today" , "last_traded_time" , "ExFeedTime" , "bidSize" , "askSize" , "bidPrice" , "askPrice" , "last_traded_qty" , "tot_buy_qty" , "tot_sell_qty" ,"avg_trade_price","-","low_price","high_price" ,"-", "-", "lowCircuit" , "upCircuit" ,"open_price", "close_price"]
+        litename = ["ltp","vol_traded_today" , "last_traded_time" ]
         depthvalue = ["bidPrice1","bidPrice2","bidPrice3","bidPrice4","bidPrice5",
                     "askPrice1", "askPrice2", "askPrice3", "askPrice4", "askPrice5", 
                     "bidsize1","bidsize2","bidsize3","bidsize4","bidsize5",
                     "askSize1","askSize2","askSize3","askSize4","askSize5",
                     "bidorder1","bidorder2","bidorder3","bidorder4","bidorder5",
                     "askorder1","askorder2","askorder3","askorder4","askorder5",]
         
@@ -182,21 +194,27 @@
             field_id = struct.unpack('!B', data[7:8])[0]
             field_length = struct.unpack('!H', data[8:10])[0]
             self.ack_count = struct.unpack('>I', data[10+field_length:14+field_length])[0]
             json_obj = data[14+field_length:].decode()
 
         elif respType == 5: # Unsubsciption response
 
-            fieldCount = struct.unpack('!B', data[3:4])[0]
-            field_id = struct.unpack('!B', data[4:5])[0]
-            string_val = data[7:9].decode('utf-8')
-            if string_val == "K":
-                print("Unsubs done")
+            field_count = struct.unpack('B', data[3:4])[0]
+            # Read field-Id
+            field_id = struct.unpack('B', data[4:5])[0]
+
+            # Read String field Length
+            field_length = struct.unpack('H', data[4:6])[0]
+            # Read & construct string using field-length
+            string_val = data[7:7+field_length].decode('utf-8')
+
+            if string_val == 'K':
+                print("Unsubscription done")
             else:
-                print("unsubs failed")
+                print("Unsubscription failed")
 
         elif respType == 12: # Full Mode Data Response
 
             fieldCount = struct.unpack('!B', data[3:4])[0]
             if fieldCount >= 1:
                 field_id = struct.unpack('!B', data[4:5])[0]
                 field_length = struct.unpack('!H', data[5:7])[0]
@@ -208,159 +226,186 @@
         elif respType == 6: # Data Feed Response
             updateCount = 0
 
             if self.ack_count > 0:
                 updateCount += 1
                 msgNum = struct.unpack('>I', data[3:7])[0]
                 if updateCount == self.ack_count:
-                    # send acknoledgement 
+                    self.ack_bool = True
+                    self.ack_msg = self.ackowledgement_msg(msgNum)
                     updateCount = 0
             scripCount = struct.unpack('!H', data[7:9])[0]
             offset = 9
             for _ in range(scripCount):
                 dataType = struct.unpack('B', data[offset:offset+1])[0]
-                print("dataType",dataType)
                 if dataType == 83: 
                     self.output = {}
                     offset += 1
                     topicId = struct.unpack('H', data[offset:offset+2])[0]
-                    print("topicid",topicId)
                     offset += 2
                     topicNameLength = struct.unpack('B', data[offset:offset+1])[0]
                     offset += 1
                     topicName = data[offset:offset+topicNameLength].decode('utf-8')
                     offset += topicNameLength
+                    # Maintaining dict - topicId : topicName
                     self.symDict[topicId] = topicName
-                    print("topic Name ------",topicName)
                     fieldCount = struct.unpack('B', data[offset:offset+1])[0]
                     offset += 1
                     for index in range(fieldCount):
                         value = struct.unpack('>I', data[offset:offset+4])[0]
                         offset += 4
                         if fieldCount < 23:
-                            self.output[ValName[index]] = value
+                            if ValName[index] != '-':
+                                self.output[ValName[index]] = value
                         else:
                             self.output[depthvalue[index]] = value                    
-
                     stringFieldLength = struct.unpack('H', data[offset:offset+2])[0]
                     offset += 2
                     multiplier = struct.unpack('H', data[offset:offset+2])[0]
-                    # print("multiplier",multiplier)
+                    self.output["multiplier"] = multiplier
                     offset += 2
                     precision = struct.unpack('B', data[offset:offset+1])[0]
-                    # print("precision",precision)
                     self.output["precision"] = precision
                     offset += 1
-                    val = ["EX", "ExToken","Symbol"]
+                    val = ["exch", "exch_token","symbol"]
                     for i in range(3):
                         stringLength = struct.unpack('B', data[offset:offset+1])[0]
                         offset += 1
                         stringData = data[offset:offset+stringLength].decode('utf-8')
                         self.output[val[i]] = stringData
-                        if i == 2:
-                            symb = stringData
                         offset += stringLength
                     
                     self.resp[self.symDict[topicId]] = self.output
-
-                    print("======",self.symDict[topicId])
-                    print("Response : ", self.output)
+                    print(self.resp[self.symDict[topicId]])
                     
                 elif dataType == 85:
                     offset += 1
                     topicId = struct.unpack('H', data[offset:offset+2])[0]
-                    print("topicId",topicId)
-                    # self.output[self.symDict[topicId]] = {}
-                    # self.output = {}
                     offset += 2
                     fieldCount = struct.unpack('B', data[offset:offset+1])[0]
                     offset += 1
                     for index in range(fieldCount):
                         value = struct.unpack('>I', data[offset:offset+4])[0]
                         offset += 4
-                        # print("--------------------",self.output[self.symDict[topicId]])
                         if fieldCount < 23:
-                            self.resp[self.symDict[topicId]][ValName[index]] = value
+                            if ValName[index] != '-':
+
+                                if index in [0,6,7,11,13,14,17,18,19,20]:
+                                    self.resp[self.symDict[topicId]][ValName[index]] = value / (10 ** self.resp[self.symDict[topicId]]['precision'])
+                                else:
+                                    self.resp[self.symDict[topicId]][ValName[index]] = value
                         else:
-                            self.resp[self.symDict[topicId]][depthvalue[index]] = value
+                            if 0 <= index <= 9:
+                                self.resp[self.symDict[topicId]][depthvalue[index]] = value / (10 ** self.resp[self.symDict[topicId]]['precision'])
+                            else:
+                                self.resp[self.symDict[topicId]][depthvalue[index]] = value
+                            
+                    print(self.resp[self.symDict[topicId]])
+                elif dataType == 76:
+                    offset += 1
+                    topicId = struct.unpack('H', data[offset:offset+2])[0]
+                    offset += 2
+                    print("topicID :",topicId)
+                    self.literesp[self.symDict[topicId]] = {}
 
-                    # self.output["symbol"] = self.symDict[topicId]
-                    print("finalresponse :",self.symDict[topicId], "---" ,self.resp[self.symDict[topicId]])
+                    for index in range(3):
+                        value = struct.unpack('>I', data[offset:offset+4])[0]
+                        offset += 4
+                        self.literesp[self.symDict[topicId]][litename[index]] = value
+                    self.literesp[self.symDict[topicId]]['symbol']  = self.resp[self.symDict[topicId]]['symbol']
+                        # print(f"Field {index+1}: {value}")
+                    print(self.literesp[self.symDict[topicId]])
                 else:
-                    print("Invalid Datatype Error : ", data)
+                    pass
+
 
+    async def close(self):
+        # if hasattr(self, 'websocket') and self.websocket.open:
+        await self.websocket.close()
+        # if not websocket_task.done():
+        #     websocket = websocket_task.result()
+        #     if not websocket.closed:
+        #         await websocket.close()
 
-    async def close(self, websocket_task):
-        if not websocket_task.done():
-            websocket = websocket_task.result()
-            if not websocket.closed:
-                await websocket.close()
     async def send_ping(self, websocket):
         await websocket.ping() 
-        print("ping")
         asyncio.get_event_loop().call_later(10, lambda: asyncio.ensure_future(self.send_ping(websocket)))
     
     async def connectWS(self):
-        async with websockets.connect("wss://socket.fydev.tech/hsm/v1-5/dev" ) as websocket:
-            # message = bytearray(b'\x00W\x01\x04\x01\x0083fd5caefeb662931c6560cf5991b55e327f33ddf8ca0b2a1b0ed7165\x02\x00\x01N\x03\x00\x01\x01\x04\x00\x0fPythonSDK-1.0.0')
-            message = self.TokenByteMsg()
-            await websocket.send(message)
-            print(f"Sent message: {message}")
-            response = await websocket.recv()
-            # print(response)
-            self.ByteToJson(response)
-            # message = b'\x00\x11\x0c\x02\x01\x00\x08\x00\x00\x00\x00\x00\x00\x12&\x02\x00\x01F'
-            if not self.lite:
-                message = self.SetToFullMode()
+        try:
+            async with websockets.connect("wss://socket.fydev.tech/hsm/v1-5/dev" ) as websocket:
+                self.websocket = websocket
+                message = self.token_to_byte()
                 await websocket.send(message)
                 response = await websocket.recv()
-                self.ByteToJson(response)
-                
-            # message = bytearray(b'\x00\xaf\x04\x02\x01\x00V\x00\x06\x0fsf|nse_cm|11536\x0fdp|nse_cm|11536\x0csf|nse_cm|25\x0cdp|nse_cm|25\x0csf|nse_cm|22\x0cdp|nse_cm|22\x02\x00\x01\x01')
-            # message =bytearray(b'\x00{\x04\x02\x01\x00"\x00\x02\x0fsf|nse_cm|11536\x0fdp|nse_cm|11536\x02\x00\x01\x01')
-            message = self.SubscribeMsgByte()
-            await websocket.send(message)
-            print(f"Sent message: {message}")
-            asyncio.ensure_future(self.send_ping(websocket))
-            x = 0
-            while True:
-                response = await websocket.recv()
-                self.ByteToJson(response)
-                # x += 1
-                # print("-------------------------------",x)
-                # if x == 10:
-                #     scrips = ["sf|nse_cm|25","dp|nse_cm|25", "sf|nse_cm|22", "dp|nse_cm|22"]
-                #     msg = self.UnSubscribeByte(scrips)
-                #     await websocket.send(msg)
-                #     response = await websocket.recv()
-                #     self.ByteToJson(response)
+                self.response_msg(response)
+                if not self.lite:
+                    message = self.full_mode_msg()
+                    await websocket.send(message)
+                    response = await websocket.recv()
+                    self.response_msg(response)
 
+                message = self.subscription_msg()
+                await websocket.send(message)
+                asyncio.ensure_future(self.send_ping(websocket))
+                x = 0
+                while True:
+                    response = await websocket.recv()
+                    self.response_msg(response)
+
+                    if self.ack_bool:
+                        await websocket.send(self.ack_msg)
+                        self.ack_bool = False
+        except:
+            print("Error While Connecting")
 
-    # async def main(self):
-    #     ws_task = asyncio.create_task(self.connectWS())
 
-    #     await ws_task
     def subscribe(self):
         loop = asyncio.get_event_loop()
         websocket_task = loop.create_task(self.connectWS())
         try:
             loop.run_until_complete(websocket_task)
         except KeyboardInterrupt:
             websocket_task.cancel()
             try:
                 loop.run_until_complete(websocket_task)
             except asyncio.CancelledError:
                 pass
             finally:
-                loop.run_until_complete(self.close(websocket_task))
+                loop.run_until_complete(self.close())
         finally:
             loop.close()
+
+
 # access_token ="3fd5caefeb662931c6560cf5991b55e327f33ddf8ca0b2a1b0ed7165"
 # access_token = "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJodHRwczovL2xvZ2luLmZ5ZXJzLmluIiwiaWF0IjoxNjg0NzMwNDA2LCJleHAiOjE2ODQ4MDE4MDYsIm5iZiI6MTY4NDczMDQwNiwiYXVkIjpbIng6MCJdLCJzdWIiOiJhY2Nlc3NfdG9rZW4iLCJhdF9oYXNoIjoiZ0FBQUFBQmthdkltdGMtQUFueTVnR2liMGRtVHdXeko5TmFuTUtEVlBzYTVHRnRFaUdCczN1OTh2ZE01UFlZanNOc3Bfd2szbEpYcUU5cXJTQVQ2eXJDZTh0R0pBcnlFcFJtaWhaSVMtSVBPZmY1VkVlX3M3U0U9IiwiZGlzcGxheV9uYW1lIjoiVklOQVkgS1VNQVIgTUFVUllBIiwiZnlfaWQiOiJYVjIwOTg2IiwiYXBwVHlwZSI6IiIsIm9tcyI6IksxIiwicG9hX2ZsYWciOiJOIiwiaHNtX2tleSI6IjNmZDVjYWVmZWI2NjI5MzFjNjU2MGNmNTk5MWI1NWUzMjdmMzNkZGY4Y2EwYjJhMWIwZWQ3MTY1In0.8I11EvKNf-Z4dHn8nd6gSM0AhN0D4zf0-e59GWaEP_8"
 # access_token = "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJhcGkuZnllcnMuaW4iLCJpYXQiOjE2ODQ3MzgzMjUsImV4cCI6MTY4NDgwMTgwNSwibmJmIjoxNjg0NzM4MzI1LCJhdWQiOlsieDowIiwieDoxIiwieDoyIiwiZDoxIiwiZDoyIiwieDoxIiwieDowIl0sInN1YiI6ImFjY2Vzc190b2tlbiIsImF0X2hhc2giOiJnQUFBQUFCa2F4RVZLSWZPVGVUNkZtYmw4b29wLW9sTU1JaG0waU1IOGIzZmNESlVxNjI1andudnM1LXdTTnA0RTR0TmY1aGxDWWNFUm56QXlnNWVmWFFTUVFiR0M2Y0NaMVVKN3hkc2ptZ3FMZkxOejhsa3FWZz0iLCJkaXNwbGF5X25hbWUiOiJWSU5BWSBLVU1BUiBNQVVSWUEiLCJvbXMiOiJLMSIsImZ5X2lkIjoiWFYyMDk4NiIsImFwcFR5cGUiOjEwMCwicG9hX2ZsYWciOiJOIn0.8GfqzLmubDCX-FCcjIppkzurYhz4wakgaeeD5Ryk30s"
-access_token = "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJhcGkuZnllcnMuaW4iLCJpYXQiOjE2ODMwMDE4OTgsImV4cCI6MTY4MzA3MzgzOCwibmJmIjoxNjgzMDAxODk4LCJhdWQiOlsieDowIiwieDoxIiwieDoyIiwiZDoxIiwiZDoyIiwieDoxIiwieDowIl0sInN1YiI6ImFjY2Vzc190b2tlbiIsImF0X2hhc2giOiJnQUFBQUFCa1VKSXFKLTNQMl9BSXFWWFNWUlg5UXlIVW5QWlpGRnFnNG5xRkNWRzYwQU5qX0F6T2hVWmxPZmtCNUV4ak03MXBMWVlqSEpjWXBsaVpVNWpFREQ1R3JFVkt4Rmx0SzR4RDh2SERVdkZndWgwUEVGRT0iLCJkaXNwbGF5X25hbWUiOiJWSU5BWSBLVU1BUiBNQVVSWUEiLCJvbXMiOiJLMSIsImZ5X2lkIjoiWFYyMDk4NiIsImFwcFR5cGUiOjEwMCwicG9hX2ZsYWciOiJOIn0.MghUuBXEV3INDwH-buwTUvJDvBQ0HS37d69nwRCE7nE"
-scrips =  ["sf|nse_cm|11536","sf|nse_cm|25","dp|nse_cm|25", "sf|nse_cm|22", "dp|nse_cm|22"]
-client = FyersHsmSocket(access_token,scrips)
+# access_token = "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJhcGkuZnllcnMuaW4iLCJpYXQiOjE2ODMwMDE4OTgsImV4cCI6MTY4MzA3MzgzOCwibmJmIjoxNjgzMDAxODk4LCJhdWQiOlsieDowIiwieDoxIiwieDoyIiwiZDoxIiwiZDoyIiwieDoxIiwieDowIl0sInN1YiI6ImFjY2Vzc190b2tlbiIsImF0X2hhc2giOiJnQUFBQUFCa1VKSXFKLTNQMl9BSXFWWFNWUlg5UXlIVW5QWlpGRnFnNG5xRkNWRzYwQU5qX0F6T2hVWmxPZmtCNUV4ak03MXBMWVlqSEpjWXBsaVpVNWpFREQ1R3JFVkt4Rmx0SzR4RDh2SERVdkZndWgwUEVGRT0iLCJkaXNwbGF5X25hbWUiOiJWSU5BWSBLVU1BUiBNQVVSWUEiLCJvbXMiOiJLMSIsImZ5X2lkIjoiWFYyMDk4NiIsImFwcFR5cGUiOjEwMCwicG9hX2ZsYWciOiJOIn0.MghUuBXEV3INDwH-buwTUvJDvBQ0HS37d69nwRCE7nE"
+# scrips =  ["sf|nse_cm|11536","sf|nse_cm|25","dp|nse_cm|25", "sf|nse_cm|22", "dp|nse_cm|22"]
+# # ,"sf|nse_cm|11536","sf|nse_cm|25","dp|nse_cm|25", "sf|nse_cm|22", "dp|nse_cm|22"
+# client = FyersHsmSocket(access_token,scrips)
+
+# # result = asyncio.run(client.main())
+# client.subscribe()
+# asyncio.sleep(5)
+# asyncio.run(client.close())
+
+# async def main():
+#     access_token = "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJhcGkuZnllcnMuaW4iLCJpYXQiOjE2ODMwMDE4OTgsImV4cCI6MTY4MzA3MzgzOCwibmJmIjoxNjgzMDAxODk4LCJhdWQiOlsieDowIiwieDoxIiwieDoyIiwiZDoxIiwiZDoyIiwieDoxIiwieDowIl0sInN1YiI6ImFjY2Vzc190b2tlbiIsImF0X2hhc2giOiJnQUFBQUFCa1VKSXFKLTNQMl9BSXFWWFNWUlg5UXlIVW5QWlpGRnFnNG5xRkNWRzYwQU5qX0F6T2hVWmxPZmtCNUV4ak03MXBMWVlqSEpjWXBsaVpVNWpFREQ1R3JFVkt4Rmx0SzR4RDh2SERVdkZndWgwUEVGRT0iLCJkaXNwbGF5X25hbWUiOiJWSU5BWSBLVU1BUiBNQVVSWUEiLCJvbXMiOiJLMSIsImZ5X2lkIjoiWFYyMDk4NiIsImFwcFR5cGUiOjEwMCwicG9hX2ZsYWciOiJOIn0.MghUuBXEV3INDwH-buwTUvJDvBQ0HS37d69nwRCE7nE"
+#     scrips =  ["sf|nse_cm|11536","sf|nse_cm|25","dp|nse_cm|25", "sf|nse_cm|22", "dp|nse_cm|22"]
+#     client = FyersHsmSocket(access_token,scrips)
+#     await client.subscribe()
+#     await asyncio.sleep(5)
+#     await client.close()
+# asyncio.run(main())
+
+
 
-# result = asyncio.run(client.main())
-client.subscribe()
 
+                # x += 1
+                # if x == 10:
+                #     scrips = ["sf|nse_cm|25","dp|nse_cm|25","dp|nse_cm|22","sf|nse_cm|11536"]
+                #     msg = self.unsubscription_msg(scrips)
+                #     await websocket.send(msg)
+                #     response = await websocket.recv()
+                #     print("unsub response : ",response)
+                #     self.response_msg(response)
```

## fyerstest/ws.py

```diff
@@ -155,21 +155,23 @@
     def subscribe(self,data_type):
         self.data_type = [self.socket_type[(type)] for type in data_type.split(",")]
         loop = self.get_or_create_eventloop()
         websocket_task = loop.create_task(self.ScoketConnect())
         try:
             loop.run_until_complete(websocket_task)
         except KeyboardInterrupt:
-            websocket_task.cancel()
-            try:
-                loop.run_until_complete(websocket_task)
-            except asyncio.CancelledError:
-                pass
-            finally:
-                loop.run_until_complete(self.close(websocket_task))
+            # websocket_task.cancel()
+            loop.close()
+
+            # try:
+            #     loop.run_until_complete(websocket_task)
+            # except asyncio.CancelledError:
+            #     pass
+            # finally:
+            #     loop.run_until_complete(self.close(websocket_task))
         finally:
             loop.close()
 
 
     def logger_setup(self):
         if self.log_path is None:
             self.log_path = os.getcwd()
```

## Comparing `fyerspysdk1-1.5.dist-info/LICENSE.txt` & `fyerspysdk1-1.6.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `fyerspysdk1-1.5.dist-info/METADATA` & `fyerspysdk1-1.6.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyerspysdk1
-Version: 1.5
+Version: 1.6
 Summary: XX trc APIs.
 Home-page: https://github.com
 Author: my-Tech
 Author-email: support@f.in
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

