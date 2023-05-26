# Comparing `tmp/betterdataclass-202.4.tar.gz` & `tmp/betterdataclass-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "betterdataclass-202.4.tar", last modified: Mon May 22 15:46:48 2023, max compression
+gzip compressed data, was "betterdataclass-3.0.tar", last modified: Fri May 26 05:29:40 2023, max compression
```

## Comparing `betterdataclass-202.4.tar` & `betterdataclass-3.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:46:48.981143 betterdataclass-202.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-22 15:46:37.000000 betterdataclass-202.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-22 15:46:48.977143 betterdataclass-202.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8175 2023-05-22 15:46:37.000000 betterdataclass-202.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:46:48.977143 betterdataclass-202.4/betterdataclass/
--rw-r--r--   0 runner    (1001) docker     (123)     5457 2023-05-22 15:46:37.000000 betterdataclass-202.4/betterdataclass/StrictDictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-05-22 15:46:37.000000 betterdataclass-202.4/betterdataclass/StrictList.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 15:46:37.000000 betterdataclass-202.4/betterdataclass/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:46:48.977143 betterdataclass-202.4/betterdataclass/helper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 15:46:37.000000 betterdataclass-202.4/betterdataclass/helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-22 15:46:37.000000 betterdataclass-202.4/betterdataclass/helper/initiate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-22 15:46:37.000000 betterdataclass-202.4/betterdataclass/helper/to_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-22 15:46:37.000000 betterdataclass-202.4/betterdataclass/helper/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:46:48.977143 betterdataclass-202.4/betterdataclass.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-22 15:46:48.000000 betterdataclass-202.4/betterdataclass.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-22 15:46:48.000000 betterdataclass-202.4/betterdataclass.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 15:46:48.000000 betterdataclass-202.4/betterdataclass.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-22 15:46:48.000000 betterdataclass-202.4/betterdataclass.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-22 15:46:37.000000 betterdataclass-202.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 15:46:48.981143 betterdataclass-202.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-05-22 15:46:37.000000 betterdataclass-202.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 05:29:40.711869 betterdataclass-3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-26 05:29:25.000000 betterdataclass-3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9819 2023-05-26 05:29:40.711869 betterdataclass-3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8990 2023-05-26 05:29:25.000000 betterdataclass-3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 05:29:40.711869 betterdataclass-3.0/betterdataclass/
+-rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-05-26 05:29:25.000000 betterdataclass-3.0/betterdataclass/StrictDictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-05-26 05:29:25.000000 betterdataclass-3.0/betterdataclass/StrictList.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 05:29:25.000000 betterdataclass-3.0/betterdataclass/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 05:29:40.711869 betterdataclass-3.0/betterdataclass/helper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 05:29:25.000000 betterdataclass-3.0/betterdataclass/helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-26 05:29:25.000000 betterdataclass-3.0/betterdataclass/helper/initiate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-26 05:29:25.000000 betterdataclass-3.0/betterdataclass/helper/to_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-26 05:29:25.000000 betterdataclass-3.0/betterdataclass/helper/validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-26 05:29:25.000000 betterdataclass-3.0/betterdataclass/strictEnum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 05:29:40.711869 betterdataclass-3.0/betterdataclass.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9819 2023-05-26 05:29:40.000000 betterdataclass-3.0/betterdataclass.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-26 05:29:40.000000 betterdataclass-3.0/betterdataclass.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 05:29:40.000000 betterdataclass-3.0/betterdataclass.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-26 05:29:40.000000 betterdataclass-3.0/betterdataclass.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 05:29:40.711869 betterdataclass-3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-26 05:29:25.000000 betterdataclass-3.0/setup.py
```

### Comparing `betterdataclass-202.4/LICENSE` & `betterdataclass-3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `betterdataclass-202.4/README.md` & `betterdataclass-3.0/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,293 +1,337 @@
+betterdataclass
+===============
 
-# betterdataclass
+``betterdataclass`` is a Python library that enhances the functionality
+of the existing ``dataclass`` system. It provides additional features
+and improvements to make working with data classes even better.
 
-`betterdataclass` is a Python library that enhances the functionality of the existing `dataclass` system. It provides additional features and improvements to make working with data classes even better.
+Features
+--------
 
-## Features
+1. StrictDictionary
+~~~~~~~~~~~~~~~~~~~
 
-### 1. StrictDictionary
+The ``StrictDictionary`` class is a powerful data class that acts like a
+dictionary, allowing you to store and access key-value pairs. It
+enforces strict typing of the values based on the annotations of the
+class attributes, ensuring data integrity and preventing type-related
+bugs.
 
-The `StrictDictionary` class is a powerful data class that acts like a dictionary, allowing you to store and access key-value pairs. It enforces strict typing of the values based on the annotations of the class attributes, ensuring data integrity and preventing type-related bugs.
-
-### 2. StrictList
-
-The `StrictList` class is an enhanced version of the built-in list class. It allows you to create lists with strict typing and restrictions on the elements. You can define the allowed types or even customize restrictions to ensure that only valid elements are added to the list.
-
-## Authors
-
-- [@Asutosh Rath](https://www.github.com/dvnasutosh)
-
-## **Installation**
-You can install `betterdataclass` using pip:
-
-```shell
-    pip install betterdataclass
-```
-## **Restrictions**
-- Accepted typing Types
-  - `Union`
-  - `Optional`
-  - `Final`
-  - `Dict`
-  - `Tuple`
-  - `Set`
-  - `List`
-  - `Literal`
-  - *anything that `typing.get_origin()` 1 times leads to the aforementioned types or the default generic types*
--  Can't produce JSON file out of `Enum`,  but it is accepted.
--  Can't add data members post *class defination*, i.e. in *runtime*.
-
-## **Usage Example- StrictDictionary**
-
-Let's see a simple example of using `betterdataclass` to create a strict dictionary and list.
-
-### **Creating a `StrictDictionary`**
-
-```python
-from betterdataclass import StrictDictionary
-
-class Person(StrictDictionary):
-    name: str
-    age: int
-
-# Create an instance of the strict dictionary
-person = Person(name='John', age=30)
-
-# Access the attributes
-print(person.name)  # Output: John
-print(person.age)   # Output: 30
-
-# Add new attribute with type checking
-person['address'] = '123 Main Street'
-
-# Print the strict dictionary
-print(person)       # Output: {'name': 'John', 'age': 30, 'address': '123 Main Street'}
-```
-### **Creating a `StrictList`**
-```Python
-from betterdataclass import StrictList
-
-class NumberList(StrictList):
-    types = (int, float)
-
-# Create an instance of the strict list
-numbers = NumberList([1, 2, 3.14])
-
-# Access the elements
-print(numbers[0])   # Output: 1
-print(numbers[1])   # Output: 2
-print(numbers[2])   # Output: 3.14
-
-# Add new element with type checking
-numbers.append(4)
-
-# Print the strict list
-print(numbers)      # Output: [1, 2, 3.14, 4]
-
-```
-
-
-## **More  `StrictDictionary` complex Example**
- This will speed you up what are the edge capabilities of the library is.
-1. ### Example 1
-    ```python
-    from betterdataclass import StrictDictionary
-    from typing import List, Optional
-
-    class Address(StrictDictionary):
-        street: str
-        city: str
-        postal_code: str
-
-    class Person(StrictDictionary):
-        name: str
-        age: int
-        addresses: List[Address]
-        phone: Optional[str] = None
-
-    # Create an instance of the strict dictionary
-    person = Person(
-        name='John',
-        age=30,
-        addresses=[
-            Address(street='123 Main Street', city='New York', postal_code='10001'),
-            Address(street='456 Elm Street', city='Los Angeles', postal_code='90001')
-        ],
-        phone='555-1234'
-    )
-
-    # Access the attributes
-    print(person.name)
-    print(person.age)
-    print(person.addresses)
-    print(person.phone)
-
-    # Add new attribute with type checking
-
-    # Print the strict dictionary
-    print(person)
-    ```
-    ~~``` person['email'] = 'john@example.com' ```~~
-    <br>*This won't work. I can't add new data members on the go. Hence the name StrictDictionary.*
-2. ### Example 2.
-    ``` python
-    from betterdataclass import StrictDictionary
-    from typing import List, Dict, Any
-
-    class Address(StrictDictionary):
-        street: str
-        city: str
-        postal_code: str
-
-    class Contact(StrictDictionary):
-        email: str
-        phone: str
-
-    class Person(StrictDictionary):
-        name: str
-        age: int
-        addresses: List[Address]
-        contacts: Dict[str, Contact]
-        metadata: Dict[str, Any]
-
-    # Create an instance of the strict dictionary
-    person = Person(
-        name='John',
-        age=30,
-        addresses=[
-            Address(street='123 Main Street', city='New York', postal_code='10001'),
-            Address(street='456 Elm Street', city='Los Angeles', postal_code='90001')
-        ],
-        contacts={
-            'personal': Contact(email='john@example.com', phone='555-1234'),
-            'work': Contact(email='john@work.com', phone='555-5678')
-        },
-        metadata={
-            'employee_id': 12345,
-            'position': 'Manager',
-            'active': True
-        }
-    )
-
-    # Access the attributes
-    print(person.name)
-    print(person.age)
-    print(person.addresses)
-    print(person.contacts)
-    print(person.metadata)
-
-    # Access nested attributes
-    print(person.addresses[0].street)
-    print(person.contacts['personal'].email)
-    print(person.metadata['position'])
-    ```
-3. ### Example 3.
-    ``` python
-        from betterdataclass import StrictDictionary
-        from typing import Dict, Union, Optional
-
-        class Address(StrictDictionary):
-            street: str
-            city: str
-            postal_code: str
-
-        class Contact(StrictDictionary):
-            email: str
-            phone: Union[str, int]
-
-        class Person(StrictDictionary):
-            name: str
-            age: int
-            address: Optional[Address]
-            contacts: Optional[Dict[str, Union[Contact, Dict[str, str]]]]
-
-        # Create an empty instance of the strict dictionary
-        person = Person()
-
-        # Add data using key mapping and attribute setting
-        person['name'] = 'John'
-        person.name = 'John'
-        person['age'] = 30
-        person.age = 30
-
-        # Add nested data using key mapping
-        person['address'] = Address(street='123 Main Street', city='New York', postal_code='10001')
-
-        # Add nested data using attribute setting
-        person.address = Address(street='123 Main Street', city='New York', postal_code='10001')
-
-        # Add multiple levels of nested data using key mapping
-        person['contacts'] = {
-            'personal': Contact(email='john@example.com', phone='555-1234'),
-            'work': {
-                'email': 'john@work.com',
-                'phone': 12345
-            }
-        }
-
-        # Add multiple levels of nested data using attribute setting
-        person.contacts = {
-            'personal': Contact(email='john@example.com', phone='555-1234'),
-            'work': {
-                'email': 'john@work.com',
-                'phone': 12345
-            }
-        }
-
-        # Print the strict dictionary
-        print(person)
-
-    ```
-
-## **Usage Example- StrictList**
-### **Creating a `StrictList`**
-```Python
-from betterdataclass import StrictList
-
-class NumberList(StrictList):
-    types = (int, float)
-
-# Create an instance of the strict list
-numbers = NumberList([1, 2, 3.14])
-
-# Access the elements
-print(numbers[0])   # Output: 1
-print(numbers[1])   # Output: 2
-print(numbers[2])   # Output: 3.14
-
-# Add new element with type checking
-numbers.append(4)
-
-# Print the strict list
-print(numbers)      # Output: [1, 2, 3.14, 4]
-
-```
-### **Validation usage `StrictList` example**
-```Python
-from betterdataclass import StrictList
-import re
-
-class EmailList(StrictList):
-    def restriction(self, value):
-        email_regex = r'^[\w\.-]+@[\w\.-]+\.\w+$'
-        if not re.match(email_regex, str(value)):
-            return False
-        return True
-
-# Create an instance of the EmailList
-emails = EmailList()
-
-# Add email values
-emails.append('john@example.com')
-emails.append('jane@example.com')
-emails.append('invalid_email')  # Throws error
-
-# Print the list
-print(emails)
-```
-## Roadmap
-- [ ] Make Validation decorators
-- [ ] Make StrictDictionary comply with Enum
-- [ ] Make it work with other dataclasses
+2. StrictList
+~~~~~~~~~~~~~
 
-**The Long and the short is I want generalise all the dataclass options we got** 
+The ``StrictList`` class is an enhanced version of the built-in list
+class. It allows you to create lists with strict typing and restrictions
+on the elements. You can define the allowed types or even customize
+restrictions to ensure that only valid elements are added to the list.
+
+Authors
+-------
+
+-  `@Asutosh Rath <https://www.github.com/dvnasutosh>`__
+
+**Installation**
+----------------
+
+You can install ``betterdataclass`` using pip:
+
+.. code:: shell
+
+       pip install betterdataclass
+
+**Restrictions**
+----------------
+
+-  Accepted typing Types
+
+   -  ``Union``
+   -  ``Optional``
+   -  ``Final``
+   -  ``Dict``
+   -  ``Tuple``
+   -  ``Set``
+   -  ``List``
+   -  ``Literal``
+   -  *anything that ``typing.get_origin()`` 1 times leads to the
+      aforementioned types or the default generic types*
+
+-  Can’t produce JSON file out of ``Enum``, but it is accepted.
+-  Can’t add data members post *class defination*, i.e. in *runtime*.
+
+**Usage Example- StrictDictionary**
+-----------------------------------
+
+Let’s see a simple example of using ``betterdataclass`` to create a
+strict dictionary and list.
+
+**Creating a ``StrictDictionary``**
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. code:: python
+
+   from betterdataclass import StrictDictionary
+
+   class Person(StrictDictionary):
+       name: str
+       age: int
+
+   # Create an instance of the strict dictionary
+   person = Person(name='John', age=30)
+
+   # Access the attributes
+   print(person.name)  # Output: John
+   print(person.age)   # Output: 30
+
+   # Add new attribute with type checking
+   person['address'] = '123 Main Street'
+
+   # Print the strict dictionary
+   print(person)       # Output: {'name': 'John', 'age': 30, 'address': '123 Main Street'}
+
+**Creating a ``StrictList``**
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. code:: python
+
+   from betterdataclass import StrictList
+
+   class NumberList(StrictList):
+       types = (int, float)
+
+   # Create an instance of the strict list
+   numbers = NumberList([1, 2, 3.14])
+
+   # Access the elements
+   print(numbers[0])   # Output: 1
+   print(numbers[1])   # Output: 2
+   print(numbers[2])   # Output: 3.14
+
+   # Add new element with type checking
+   numbers.append(4)
+
+   # Print the strict list
+   print(numbers)      # Output: [1, 2, 3.14, 4]
+
+**More ``StrictDictionary`` complex Example**
+---------------------------------------------
+
+This will speed you up what are the edge capabilities of the library is.
+1. ### Example 1 \```python from betterdataclass import StrictDictionary
+from typing import List, Optional
+
+::
+
+   class Address(StrictDictionary):
+       street: str
+       city: str
+       postal_code: str
+
+   class Person(StrictDictionary):
+       name: str
+       age: int
+       addresses: List[Address]
+       phone: Optional[str] = None
+
+   # Create an instance of the strict dictionary
+   person = Person(
+       name='John',
+       age=30,
+       addresses=[
+           Address(street='123 Main Street', city='New York', postal_code='10001'),
+           Address(street='456 Elm Street', city='Los Angeles', postal_code='90001')
+       ],
+       phone='555-1234'
+   )
+
+   # Access the attributes
+   print(person.name)
+   print(person.age)
+   print(person.addresses)
+   print(person.phone)
+
+   # Add new attribute with type checking
+
+   # Print the strict dictionary
+   print(person)
+   ```
+   ~~``` person['email'] = 'john@example.com' ```~~
+   <br>*This won't work. I can't add new data members on the go. Hence the name StrictDictionary.*
+
+2. .. rubric:: Example 2.
+      :name: example-2.
+
+   .. code:: python
+
+      from betterdataclass import StrictDictionary
+      from typing import List, Dict, Any
+
+      class Address(StrictDictionary):
+          street: str
+          city: str
+          postal_code: str
+
+      class Contact(StrictDictionary):
+          email: str
+          phone: str
+
+      class Person(StrictDictionary):
+          name: str
+          age: int
+          addresses: List[Address]
+          contacts: Dict[str, Contact]
+          metadata: Dict[str, Any]
+
+      # Create an instance of the strict dictionary
+      person = Person(
+          name='John',
+          age=30,
+          addresses=[
+              Address(street='123 Main Street', city='New York', postal_code='10001'),
+              Address(street='456 Elm Street', city='Los Angeles', postal_code='90001')
+          ],
+          contacts={
+              'personal': Contact(email='john@example.com', phone='555-1234'),
+              'work': Contact(email='john@work.com', phone='555-5678')
+          },
+          metadata={
+              'employee_id': 12345,
+              'position': 'Manager',
+              'active': True
+          }
+      )
+
+      # Access the attributes
+      print(person.name)
+      print(person.age)
+      print(person.addresses)
+      print(person.contacts)
+      print(person.metadata)
+
+      # Access nested attributes
+      print(person.addresses[0].street)
+      print(person.contacts['personal'].email)
+      print(person.metadata['position'])
+
+3. .. rubric:: Example 3.
+      :name: example-3.
+
+   .. code:: python
+
+          from betterdataclass import StrictDictionary
+          from typing import Dict, Union, Optional
+
+          class Address(StrictDictionary):
+              street: str
+              city: str
+              postal_code: str
+
+          class Contact(StrictDictionary):
+              email: str
+              phone: Union[str, int]
+
+          class Person(StrictDictionary):
+              name: str
+              age: int
+              address: Optional[Address]
+              contacts: Optional[Dict[str, Union[Contact, Dict[str, str]]]]
+
+          # Create an empty instance of the strict dictionary
+          person = Person()
+
+          # Add data using key mapping and attribute setting
+          person['name'] = 'John'
+          person.name = 'John'
+          person['age'] = 30
+          person.age = 30
+
+          # Add nested data using key mapping
+          person['address'] = Address(street='123 Main Street', city='New York', postal_code='10001')
+
+          # Add nested data using attribute setting
+          person.address = Address(street='123 Main Street', city='New York', postal_code='10001')
+
+          # Add multiple levels of nested data using key mapping
+          person['contacts'] = {
+              'personal': Contact(email='john@example.com', phone='555-1234'),
+              'work': {
+                  'email': 'john@work.com',
+                  'phone': 12345
+              }
+          }
+
+          # Add multiple levels of nested data using attribute setting
+          person.contacts = {
+              'personal': Contact(email='john@example.com', phone='555-1234'),
+              'work': {
+                  'email': 'john@work.com',
+                  'phone': 12345
+              }
+          }
+
+          # Print the strict dictionary
+          print(person)
+
+**Usage Example- StrictList**
+-----------------------------
+
+.. _creating-a-strictlist-1:
+
+**Creating a ``StrictList``**
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. code:: python
+
+   from betterdataclass import StrictList
+
+   class NumberList(StrictList):
+       types = (int, float)
+
+   # Create an instance of the strict list
+   numbers = NumberList([1, 2, 3.14])
+
+   # Access the elements
+   print(numbers[0])   # Output: 1
+   print(numbers[1])   # Output: 2
+   print(numbers[2])   # Output: 3.14
+
+   # Add new element with type checking
+   numbers.append(4)
+
+   # Print the strict list
+   print(numbers)      # Output: [1, 2, 3.14, 4]
+
+**Validation usage ``StrictList`` example**
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. code:: python
+
+   from betterdataclass import StrictList
+   import re
+
+   class EmailList(StrictList):
+       def restriction(self, value):
+           email_regex = r'^[\w\.-]+@[\w\.-]+\.\w+$'
+           if not re.match(email_regex, str(value)):
+               return False
+           return True
+
+   # Create an instance of the EmailList
+   emails = EmailList()
+
+   # Add email values
+   emails.append('john@example.com')
+   emails.append('jane@example.com')
+   emails.append('invalid_email')  # Throws error
+
+   # Print the list
+   print(emails)
+
+Roadmap
+-------
+
+-  ☐ Make Validation decorators
+-  ☐ Make StrictDictionary comply with Enum
+-  ☐ Make it work with other dataclasses
+
+**The Long and the short is I want generalise all the dataclass options
+we got**
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `betterdataclass-202.4/betterdataclass/StrictDictionary.py` & `betterdataclass-3.0/betterdataclass/StrictDictionary.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 
-from typing import get_args, get_args, get_args, Final, Final, Final, Any,get_origin
+from typing import get_args,get_origin
+from typing import Final, Any
 
 import json
 from .helper.to_dict import to_raw_dict
 from .helper.validate import validate
 from .helper.initiate import initialize
 
 class Dictionary(object):
@@ -35,20 +36,20 @@
     
     def __call__(self,raw:bool=False) -> dict:
         return self.__raw__() if raw else self.__data__
     
     def __str__(self):
         return str(self.__raw__())
 
-    def __json__(self):
+    def __json__(self)->str:
         return json.dumps(self.__raw__())
     
     def __raw__(self):
         # print(type(self.__data__['nested']))
-        return (self.__data__)
+        return to_raw_dict(self.__data__)
 
     def __setitem__(self, name, value) -> None:
         """
         Provides indexing and assignment functionality to the object.
         """
         self.__data__[name]=value
         
@@ -88,22 +89,21 @@
                 #SECTION: validation logic 
                 if not validate(self.__annotations__[i],j):
                     raise TypeError(
                         f'{i} key has a value {j} which is of type {type(j)}. {self.__annotations__[i]} expected.')
                 #!SECTION
                 
                 super().__setitem__(i,j)
-                # NOTE: If it is in data AND NOT IN annot than 
+
     
     def __init_subclass__(cls) -> None:
         cls.__data__= {}
         
         for k,v in cls.__dict__.items():
             if len(k)>=2 and k[0]!='_' and k[1]!='_':
-                print("hello")
                 # Handling when it is present in dict but not in annot.(It will default to What is provided)
                 if k not in cls.__annotations__:
                     pass
                 elif Final == cls.__annotations__[k]:
                     pass         
                 elif Final == get_origin(cls.__annotations__[k]):
                     if not validate(get_args(cls.__annotations__[k])[0],v):
```

### Comparing `betterdataclass-202.4/betterdataclass/StrictList.py` & `betterdataclass-3.0/betterdataclass/StrictList.py`

 * *Files identical despite different names*

### Comparing `betterdataclass-202.4/betterdataclass/helper/initiate.py` & `betterdataclass-3.0/betterdataclass/helper/initiate.py`

 * *Files identical despite different names*

### Comparing `betterdataclass-202.4/betterdataclass/helper/to_dict.py` & `betterdataclass-3.0/betterdataclass/helper/to_dict.py`

 * *Files identical despite different names*

### Comparing `betterdataclass-202.4/betterdataclass/helper/validate.py` & `betterdataclass-3.0/betterdataclass/helper/validate.py`

 * *Files identical despite different names*

### Comparing `betterdataclass-202.4/setup.py` & `betterdataclass-3.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from setuptools import find_packages, setup
+import setuptools
+
 
 setup(
     name="betterdataclass",
-    version="202.4",
+    version="3.0",
     description="A multipurpose dataclass libarary used for validation and data structuring.",
-    long_description="Go to github.com/dvnasutosh/betterdataclasses",
+    long_description=open('./README.rst').read(),
     url='https://github.com/dvnasutosh/betterdataclasses',
     
     author="Asutosh Rath",
     author_email="dvnasutosh@gmail.com",
     packages=find_packages(),
```

