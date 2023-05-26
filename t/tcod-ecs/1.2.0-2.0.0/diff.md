# Comparing `tmp/tcod-ecs-1.2.0.tar.gz` & `tmp/tcod_ecs-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tcod-ecs-1.2.0.tar", last modified: Wed Apr 26 22:04:51 2023, max compression
+gzip compressed data, was "tcod_ecs-2.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `tcod-ecs-1.2.0.tar` & `tcod_ecs-2.0.0.tar`

### file list

```diff
@@ -1,25 +1,7 @@
--rw-r--r--   0        0        0      110 2022-12-09 23:27:48.971884 tcod-ecs-1.2.0/.flake8
--rw-r--r--   0        0        0     2450 2022-12-09 22:01:20.751676 tcod-ecs-1.2.0/.gitattributes
--rw-r--r--   0        0        0      188 2022-12-07 02:28:46.295094 tcod-ecs-1.2.0/.github/FUNDING.yml
--rw-r--r--   0        0        0     1706 2023-04-09 03:23:14.272745 tcod-ecs-1.2.0/.github/workflows/python-package.yml
--rw-r--r--   0        0        0     4409 2023-03-27 00:31:15.054038 tcod-ecs-1.2.0/.gitignore
--rw-r--r--   0        0        0      772 2023-03-25 01:31:11.142017 tcod-ecs-1.2.0/.readthedocs.yml
--rw-r--r--   0        0        0     1325 2023-03-23 23:46:53.826542 tcod-ecs-1.2.0/.vscode/launch.json
--rw-r--r--   0        0        0     1516 2023-04-26 21:46:29.875591 tcod-ecs-1.2.0/.vscode/settings.json
--rw-r--r--   0        0        0     1238 2023-03-23 23:46:52.209465 tcod-ecs-1.2.0/.vscode/tasks.json
--rw-r--r--   0        0        0      777 2023-04-26 22:04:07.822052 tcod-ecs-1.2.0/CHANGELOG.md
--rw-r--r--   0        0        0     1100 2023-03-26 20:09:04.799655 tcod-ecs-1.2.0/LICENSE
--rw-r--r--   0        0        0     8642 2023-04-12 01:06:47.372874 tcod-ecs-1.2.0/README.md
--rw-r--r--   0        0        0      581 2023-04-12 01:13:36.306949 tcod-ecs-1.2.0/conftest.py
--rw-r--r--   0        0        0      634 2022-12-10 22:58:25.072843 tcod-ecs-1.2.0/docs/Makefile
--rw-r--r--   0        0        0      115 2023-03-24 00:06:33.545046 tcod-ecs-1.2.0/docs/api.rst
--rw-r--r--   0        0        0     2072 2023-03-24 00:06:35.156705 tcod-ecs-1.2.0/docs/conf.py
--rw-r--r--   0        0        0       32 2022-12-10 23:30:30.594162 tcod-ecs-1.2.0/docs/head.md
--rw-r--r--   0        0        0      255 2023-01-06 20:05:00.073778 tcod-ecs-1.2.0/docs/index.rst
--rwxr-xr-x   0        0        0      800 2022-12-10 22:58:25.073843 tcod-ecs-1.2.0/docs/make.bat
--rw-r--r--   0        0        0       46 2023-03-25 01:28:10.449866 tcod-ecs-1.2.0/docs/requirements.txt
--rw-r--r--   0        0        0     3569 2023-04-12 08:17:44.588593 tcod-ecs-1.2.0/pyproject.toml
--rw-r--r--   0        0        0    32536 2023-04-26 22:04:17.748971 tcod-ecs-1.2.0/tcod/ecs/__init__.py
--rw-r--r--   0        0        0        0 2023-04-26 20:09:12.939518 tcod-ecs-1.2.0/tcod/ecs/py.typed
--rw-r--r--   0        0        0     7530 2023-04-22 05:35:25.347051 tcod-ecs-1.2.0/tcod/ecs/test_ecs.py
--rw-r--r--   0        0        0     9609 1970-01-01 00:00:00.000000 tcod-ecs-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1079 2023-05-26 10:42:53.718165 tcod_ecs-2.0.0/LICENSE
+-rw-r--r--   0        0        0     8626 2023-05-26 10:42:53.718165 tcod_ecs-2.0.0/README.md
+-rw-r--r--   0        0        0     3688 2023-05-26 10:42:53.722166 tcod_ecs-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0    35712 2023-05-26 10:42:53.722166 tcod_ecs-2.0.0/tcod/ecs/__init__.py
+-rw-r--r--   0        0        0      160 2023-05-26 10:43:03.010447 tcod_ecs-2.0.0/tcod/ecs/_version.py
+-rw-r--r--   0        0        0        0 2023-05-26 10:42:53.722166 tcod_ecs-2.0.0/tcod/ecs/py.typed
+-rw-r--r--   0        0        0     9821 1970-01-01 00:00:00.000000 tcod_ecs-2.0.0/PKG-INFO
```

### Comparing `tcod-ecs-1.2.0/LICENSE` & `tcod_ecs-2.0.0/LICENSE`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-The MIT License (MIT)
-
-Copyright (c) 2023 Kyle Benesch
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
-THE SOFTWARE.
+The MIT License (MIT)
+
+Copyright (c) 2023 Kyle Benesch
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
+THE SOFTWARE.
```

### Comparing `tcod-ecs-1.2.0/README.md` & `tcod_ecs-2.0.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,228 +1,235 @@
-# About
-
-[![PyPI](https://img.shields.io/pypi/v/tcod-ec)](https://pypi.org/project/tcod-ecs/)
-[![PyPI - License](https://img.shields.io/pypi/l/tcod-ecs)](https://github.com/HexDecimal/python-tcod-ecs/blob/main/LICENSE)
-[![Documentation Status](https://readthedocs.org/projects/python-tcod-ecs/badge/?version=latest)](https://python-tcod-ecs.readthedocs.io)
-[![codecov](https://codecov.io/gh/HexDecimal/python-tcod-ecs/branch/main/graph/badge.svg?token=4Ak5QpTLZB)](https://codecov.io/gh/HexDecimal/python-tcod-ecs)
-
-This is an [Entity-component-system](https://en.wikipedia.org/wiki/Entity_component_system) implemented in Python.
-See the [ECS FAQ](https://github.com/SanderMertens/ecs-faq) for more info.
-
-This implementation focuses on type-hinting, organization, and is designed to work well with Python.
-The following features are currently implemented:
-
-- Entities can have store components which are instances of any Python object. Components are looked up by their type.
-- Entities can have one instance of a type, or multiple instances of a type with a string or other hashable to differentiate them.
-- Components can be registered as abstract, allowing a base type to hold subclasses of that component.
-- Entity tags are distinct from components, tags are any hashable Python object rather than empty class.
-- Entity relationships are supported, either as many-to-many or many-to-one relationships.
-- ECS Queries can be made to fetch entities having a combination of components/tags/relations or the absence of such.
-
-A lightweight version which implements only the entity-component framework exists called [tcod-ec](https://pypi.org/project/tcod-ec/).
-
-# Installation
-
-Use pip to install this library:
-```
-pip install tcod-ecs
-```
-
-If `tcod` is installed and the version is less than `14.0.0` then `import tcod.ecs` will fail.
-Remove or update `tcod` to fix this issue.
-
-# Examples
-
-## World
-
-```py
->>> import tcod.ecs
->>> world = tcod.ecs.World()  # New empty world.
-
-```
-
-## Entity
-
-New entities can be created with `World.new_entity`.
-An entity always knows about its assigned world.
-Worlds only know about their entities once the entity is assigned a name, component, tag, or relation.
-An entity is identified by its "Python identity" rather than with a low-level stand-in identifier.
-
-```py
->>> entity = world.new_entity(name="MyEntity")  # Name is optional and can be any hashable, not just str.
->>> entity
-<Entity name='MyEntity'>
->>> entity.world is world  # Worlds can always be accessed from their entity.
-True
->>> world.named["MyEntity"]  # Named entities can be accessed with `World.named`.
-<Entity name='MyEntity'>
->>> world.named.get("Missing") is None  # `World.named` acts like a dictionary, including assignment and `.get()`.
-True
-
-```
-
-## Serialization
-
-Worlds are normal Python objects and can be pickled as long as all stored components can be pickled.
-
-```py
->>> import pickle
->>> pickled_data: bytes = pickle.dumps(world)
->>> world = pickle.loads(pickled_data)
-
-```
-
-## Components
-
-Components are instances of any Python type.
-These can be accessed, assigned, or removed from entities via the dict-like `Entity.components` attribute.
-The type is used as the key to access the component.
-The types used can be custom classes or standard Python types.
-
-```py
->>> import attrs
->>> entity = world.new_entity()
->>> entity.components[int] = 42
->>> entity.components[int]
-42
->>> int in entity.components
-True
->>> del entity.components[int]
->>> entity.components[int]  # Missing keys raise KeyError
-Traceback (most recent call last):
-  ...
-KeyError: <Entity ...>
->>> entity.components.get(int, "default")  # Test keys with `.get()` like a dictionary.
-'default'
->>> @attrs.define
-... class Vector2:
-...     x: int = 0
-...     y: int = 0
->>> entity.components[Vector2] = Vector2(1, 2)
->>> entity.components[Vector2]
-Vector2(x=1, y=2)
->>> entity.components.set(Vector2(3, 4))  # Shorter syntax derives the type from the value when assigning a component.
->>> entity.components[Vector2]
-Vector2(x=3, y=4)
->>> entity.components.update_values([11, Vector2(0, 0)])  # Multiple values can be assigned without keys.
->>> entity.components[int]
-11
->>> entity.components[Vector2]
-Vector2(x=0, y=0)
-
-# Queries can be made on all entities of a world with matching components.
->>> for e in world.Q.all_of(components=[Vector2]):
-...     e.components[Vector2].x += 10
->>> entity.components[Vector2]
-Vector2(x=10, y=0)
-
-# You can match components and iterate over them at the same time.  This can be combined with the above.
->>> for pos, i in world.Q[Vector2, int]:
-...     print((pos, i))
-(Vector2(x=10, y=0), 11)
-
-# You can include `Entity` to iterate over entities with their components.
-# This always iterates over the entity itself instead of an Entity component.
->>> for e, pos, i in world.Q[tcod.ecs.Entity, Vector2, int]:
-...     print((e, pos, i))
-(<Entity ...>, Vector2(x=10, y=0), 11)
-
-```
-
-## Named Components
-
-Only one component can be assigned unless that component is given a unique name.
-You can name components with the key syntax `(name, type)` when assigning components.
-Names are not limited to strings, and can be any hashable or frozen object.
-The syntax `[type]` and `[(name, type)]` can be used interchangeably in all places accepting a component key.
-Queries on components access named components with the same syntax and must use names explicitly.
-
-```py
->>> entity = world.new_entity()
->>> entity.components[Vector2] = Vector2(0, 0)
->>> entity.components[("velocity", Vector2)] = Vector2(1, 1)
->>> entity.components[("velocity", Vector2)]
-Vector2(x=1, y=1)
->>> @attrs.define(frozen=True)
-... class Slot:
-...     index: int
->>> entity.components.update(  # Like a dict Entity.components has the `.update()` method.
-...     {
-...         ("hp", int): 10,
-...         ("max_hp", int): 12,
-...         ("atk", int): 1,
-...         str: "foo",
-...         (Slot(1), str): "empty",
-...     }
-... )
->>> entity.components[("hp", int)]
-10
->>> entity.components[str]
-'foo'
->>> entity.components[(Slot(1), str)]
-'empty'
-
-# Queries can be made on all named components with the same syntax as normal ones.
->>> for e in world.Q.all_of(components=[("hp", int), ("max_hp", int)]):
-...     e.components[("hp", int)] = e.components[("max_hp", int)]
->>> entity.components[("hp", int)]
-12
->>> for e, pos, delta in world.Q[tcod.ecs.Entity, Vector2, ("velocity", Vector2)]:
-...     e.components[Vector2] = Vector2(pos.x + delta.x, pos.y + delta.y)
->>> entity.components[Vector2]
-Vector2(x=1, y=1)
-
-```
-
-## Tags
-
-Tags are hashable objects stored in the set-like `Entity.tags`.
-These are useful as flags or to group entities together.
-
-```py
->>> entity = world.new_entity()
->>> entity.tags.add("player")  # Works well for groups
->>> "player" in entity.tags
-True
->>> entity.tags.add(("eats", "fruit"))
->>> entity.tags.add(("eats", "meat"))
->>> set(world.Q.all_of(tags=["player"])) == {entity}
-True
-
-```
-
-## Relations
-
-Use `Entity.relation_components[component_key][target] = component` to associate a relation with data.
-Use `Entity.relation_tags[tag] = target` to associate a tag exclusively with a target entity.
-Use `Entity.relation_tags_many[tag].add(target)` to associate a tag with multiple targets.
-Tags and relations share the same space then queried, so tags can not be in the format of a component key.
-Relations are unidirectional.
-
-```py
->>> @attrs.define
-... class OrbitOf:  # OrbitOf component.
-...     dist: int
->>> LandedOn = "LandedOn"  # LandedOn tag.
->>> star = world.new_entity()
->>> planet = world.new_entity()
->>> moon = world.new_entity()
->>> ship = world.new_entity()
->>> player = world.new_entity()
->>> moon_rock = world.new_entity()
->>> planet.relation_components[OrbitOf][star] = OrbitOf(dist=1000)
->>> moon.relation_components[OrbitOf][planet] = OrbitOf(dist=10)
->>> ship.relation_tags[LandedOn] = moon
->>> moon_rock.relation_tags[LandedOn] = moon
->>> player.relation_tags[LandedOn] = moon_rock
->>> set(world.Q.all_of(relations=[(OrbitOf, planet)])) == {moon}
-True
->>> set(world.Q.all_of(relations=[(OrbitOf, ...)])) == {planet, moon}  # Get objects in an orbit.
-True
->>> set(world.Q.all_of(relations=[(..., OrbitOf, None)])) == {star, planet}  # Get objects being orbited.
-True
->>> set(world.Q.all_of(relations=[(LandedOn, ...)])) == {ship, moon_rock, player}
-True
->>> set(world.Q.all_of(relations=[(LandedOn, ...)]).none_of(relations=[(LandedOn, moon)])) == {player}
-True
-
-```
+# About
+
+[![PyPI](https://img.shields.io/pypi/v/tcod-ec)](https://pypi.org/project/tcod-ecs/)
+[![PyPI - License](https://img.shields.io/pypi/l/tcod-ecs)](https://github.com/HexDecimal/python-tcod-ecs/blob/main/LICENSE)
+[![Documentation Status](https://readthedocs.org/projects/python-tcod-ecs/badge/?version=latest)](https://python-tcod-ecs.readthedocs.io)
+[![codecov](https://codecov.io/gh/HexDecimal/python-tcod-ecs/branch/main/graph/badge.svg?token=4Ak5QpTLZB)](https://codecov.io/gh/HexDecimal/python-tcod-ecs)
+
+This is an [Entity-component-system](https://en.wikipedia.org/wiki/Entity_component_system) implemented in Python.
+See the [ECS FAQ](https://github.com/SanderMertens/ecs-faq) for more info.
+
+This implementation focuses on type-hinting, organization, and is designed to work well with Python.
+The following features are currently implemented:
+
+- Entities can have store components which are instances of any Python object. Components are looked up by their type.
+- Entities can have one instance of a type, or multiple instances of a type with a string or other hashable to differentiate them.
+- Components can be registered as abstract, allowing a base type to hold subclasses of that component.
+- Entity tags are distinct from components, tags are any hashable Python object rather than empty class.
+- Entity relationships are supported, either as many-to-many or many-to-one relationships.
+- ECS Queries can be made to fetch entities having a combination of components/tags/relations or the absence of such.
+
+A lightweight version which implements only the entity-component framework exists called [tcod-ec](https://pypi.org/project/tcod-ec/).
+
+# Installation
+
+Use pip to install this library:
+```
+pip install tcod-ecs
+```
+
+If `tcod` is installed and the version is less than `14.0.0` then `import tcod.ecs` will fail.
+Remove or update `tcod` to fix this issue.
+
+# Examples
+
+## World
+
+```py
+>>> import tcod.ecs
+>>> world = tcod.ecs.World()  # New empty world.
+
+```
+
+## Entity
+
+Each Entity is identified by its unique id (`uid`) which can be any hashable object and the `world` it belongs to.
+New unique entities can be created with `World.new_entity` which uses a new `object()` as the `uid`.
+An entity always knows about its assigned world.
+Worlds only know about their entities once the entity is assigned a name, component, tag, or relation.
+
+```py
+>>> entity = world.new_entity()  # Creates a unique entity using `object()` as the uid
+>>> entity
+<Entity(uid=object at ...)>
+>>> entity.world is world  # Worlds can always be accessed from their entity
+True
+>>> world[entity.uid] is entity  # Entities with the same world/uid are compared using `is`
+True
+
+# Reference an entity with the given uid, can be any hashable object:
+>>> entity = world["MyEntity"]
+>>> entity
+<Entity(uid='MyEntity')>
+>>> world["MyEntity"] is entity
+True
+
+```
+
+Use `World.new_entity` to create unique entities and use `World[x]` to reference a global entity or relation with an id.
+
+## Serialization
+
+Worlds are normal Python objects and can be pickled as long as all stored components can be pickled.
+
+```py
+>>> import pickle
+>>> pickled_data: bytes = pickle.dumps(world)
+>>> world = pickle.loads(pickled_data)
+
+```
+
+## Components
+
+Components are instances of any Python type.
+These can be accessed, assigned, or removed from entities via the dict-like `Entity.components` attribute.
+The type is used as the key to access the component.
+The types used can be custom classes or standard Python types.
+
+```py
+>>> import attrs
+>>> entity = world.new_entity()
+>>> entity.components[int] = 42
+>>> entity.components[int]
+42
+>>> int in entity.components
+True
+>>> del entity.components[int]
+>>> entity.components[int]  # Missing keys raise KeyError
+Traceback (most recent call last):
+  ...
+KeyError: <Entity...>
+>>> entity.components.get(int, "default")  # Test keys with `.get()` like a dictionary.
+'default'
+>>> @attrs.define
+... class Vector2:
+...     x: int = 0
+...     y: int = 0
+>>> entity.components[Vector2] = Vector2(1, 2)
+>>> entity.components[Vector2]
+Vector2(x=1, y=2)
+>>> entity.components.set(Vector2(3, 4))  # Shorter syntax derives the type from the value when assigning a component.
+>>> entity.components[Vector2]
+Vector2(x=3, y=4)
+>>> entity.components.update_values([11, Vector2(0, 0)])  # Multiple values can be assigned without keys.
+>>> entity.components[int]
+11
+>>> entity.components[Vector2]
+Vector2(x=0, y=0)
+
+# Queries can be made on all entities of a world with matching components.
+>>> for e in world.Q.all_of(components=[Vector2]):
+...     e.components[Vector2].x += 10
+>>> entity.components[Vector2]
+Vector2(x=10, y=0)
+
+# You can match components and iterate over them at the same time.  This can be combined with the above.
+>>> for pos, i in world.Q[Vector2, int]:
+...     print((pos, i))
+(Vector2(x=10, y=0), 11)
+
+# You can include `Entity` to iterate over entities with their components.
+# This always iterates over the entity itself instead of an Entity component.
+>>> for e, pos, i in world.Q[tcod.ecs.Entity, Vector2, int]:
+...     print((e, pos, i))
+(<Entity...>, Vector2(x=10, y=0), 11)
+
+```
+
+## Named Components
+
+Only one component can be assigned unless that component is given a unique name.
+You can name components with the key syntax `(name, type)` when assigning components.
+Names are not limited to strings, and can be any hashable or frozen object.
+The syntax `[type]` and `[(name, type)]` can be used interchangeably in all places accepting a component key.
+Queries on components access named components with the same syntax and must use names explicitly.
+
+```py
+>>> entity = world.new_entity()
+>>> entity.components[Vector2] = Vector2(0, 0)
+>>> entity.components[("velocity", Vector2)] = Vector2(1, 1)
+>>> entity.components[("velocity", Vector2)]
+Vector2(x=1, y=1)
+>>> @attrs.define(frozen=True)
+... class Slot:
+...     index: int
+>>> entity.components.update(  # Like a dict Entity.components has the `.update()` method.
+...     {
+...         ("hp", int): 10,
+...         ("max_hp", int): 12,
+...         ("atk", int): 1,
+...         str: "foo",
+...         (Slot(1), str): "empty",
+...     }
+... )
+>>> entity.components[("hp", int)]
+10
+>>> entity.components[str]
+'foo'
+>>> entity.components[(Slot(1), str)]
+'empty'
+
+# Queries can be made on all named components with the same syntax as normal ones.
+>>> for e in world.Q.all_of(components=[("hp", int), ("max_hp", int)]):
+...     e.components[("hp", int)] = e.components[("max_hp", int)]
+>>> entity.components[("hp", int)]
+12
+>>> for e, pos, delta in world.Q[tcod.ecs.Entity, Vector2, ("velocity", Vector2)]:
+...     e.components[Vector2] = Vector2(pos.x + delta.x, pos.y + delta.y)
+>>> entity.components[Vector2]
+Vector2(x=1, y=1)
+
+```
+
+## Tags
+
+Tags are hashable objects stored in the set-like `Entity.tags`.
+These are useful as flags or to group entities together.
+
+```py
+>>> entity = world.new_entity()
+>>> entity.tags.add("player")  # Works well for groups
+>>> "player" in entity.tags
+True
+>>> entity.tags.add(("eats", "fruit"))
+>>> entity.tags.add(("eats", "meat"))
+>>> set(world.Q.all_of(tags=["player"])) == {entity}
+True
+
+```
+
+## Relations
+
+Use `Entity.relation_components[component_key][target] = component` to associate a relation with data.
+Use `Entity.relation_tags[tag] = target` to associate a tag exclusively with a target entity.
+Use `Entity.relation_tags_many[tag].add(target)` to associate a tag with multiple targets.
+Tags and relations share the same space then queried, so tags can not be in the format of a component key.
+Relations are unidirectional.
+
+```py
+>>> @attrs.define
+... class OrbitOf:  # OrbitOf component.
+...     dist: int
+>>> LandedOn = "LandedOn"  # LandedOn tag.
+>>> star = world.new_entity()
+>>> planet = world.new_entity()
+>>> moon = world.new_entity()
+>>> ship = world.new_entity()
+>>> player = world.new_entity()
+>>> moon_rock = world.new_entity()
+>>> planet.relation_components[OrbitOf][star] = OrbitOf(dist=1000)
+>>> moon.relation_components[OrbitOf][planet] = OrbitOf(dist=10)
+>>> ship.relation_tags[LandedOn] = moon
+>>> moon_rock.relation_tags[LandedOn] = moon
+>>> player.relation_tags[LandedOn] = moon_rock
+>>> set(world.Q.all_of(relations=[(OrbitOf, planet)])) == {moon}
+True
+>>> set(world.Q.all_of(relations=[(OrbitOf, ...)])) == {planet, moon}  # Get objects in an orbit.
+True
+>>> set(world.Q.all_of(relations=[(..., OrbitOf, None)])) == {star, planet}  # Get objects being orbited.
+True
+>>> set(world.Q.all_of(relations=[(LandedOn, ...)])) == {ship, moon_rock, player}
+True
+>>> set(world.Q.all_of(relations=[(LandedOn, ...)]).none_of(relations=[(LandedOn, moon)])) == {player}
+True
+
+```
```

### Comparing `tcod-ecs-1.2.0/pyproject.toml` & `tcod_ecs-2.0.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,118 +1,125 @@
-[build-system]
-requires = ["flit_core >=3.2,<4"]
-build-backend = "flit_core.buildapi"
-
-[project]
-name = "tcod-ecs"
-authors = [{ name = "Kyle Benesch", email = "4b796c65+github@gmail.com" }]
-readme = "README.md"
-license = { file = "LICENSE" }
-classifiers = [
-    "Development Status :: 5 - Production/Stable",
-    "Intended Audience :: Developers",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-    "Programming Language :: Python :: 3",
-    "Topic :: Software Development :: Libraries :: Python Modules",
-    "Typing :: Typed",
-]
-dynamic = ["version", "description"]
-requires-python = ">=3.8"
-dependencies = ["typing-extensions >=4.4.0"]
-
-[project.optional-dependencies]
-test = [
-    "attrs >=22.2.0",
-    "pytest >=7.2.0",
-    "pytest-cov >=4.0.0",
-    "pytest-benchmark >=4.0.0",
-    "mypy >=1.1.1",
-]
-
-[tool.flit.module]
-name = "tcod.ecs"
-
-[project.urls]
-Home = "https://github.com/HexDecimal"
-Changelog = "https://github.com/HexDecimal/python-tcod-ecs/blob/main/CHANGELOG.md"
-Documentation = "https://python-tcod-ecs.readthedocs.io"
-Source = "https://github.com/HexDecimal/python-tcod-ecs"
-
-[tool.black] # https://black.readthedocs.io/en/stable/usage_and_configuration/the_basics.html#configuration-via-a-file
-target-version = ["py38"]
-line-length = 120
-
-[tool.isort] # https://pycqa.github.io/isort/docs/configuration/options.html
-py_version = "38"
-line_length = 120
-profile = "black"
-skip_gitignore = true
-
-[tool.mypy] # https://mypy.readthedocs.io/en/stable/config_file.html
-files = "**/*.py"
-explicit_package_bases = true
-python_version = "3.10"            # Type check Python version with EllipsisType.
-warn_unused_configs = true
-disallow_any_generics = true
-disallow_subclassing_any = true
-disallow_untyped_calls = true
-disallow_untyped_defs = true
-disallow_incomplete_defs = true
-check_untyped_defs = true
-disallow_untyped_decorators = true
-no_implicit_optional = true
-warn_redundant_casts = true
-warn_unused_ignores = true
-warn_return_any = true
-no_implicit_reexport = true
-strict_equality = true
-
-[tool.pytest.ini_options]
-minversion = "6.0"
-required_plugins = ["pytest-cov>=4.0.0", "pytest-benchmark>=4.0.0"]
-addopts = "--doctest-modules --cov=tcod --doctest-glob=*.md"
-testpaths = ["."]
-
-[tool.ruff]
-# https://beta.ruff.rs/docs/rules/
-select = [
-    "C90", # mccabe
-    "E",   # pycodestyle
-    "W",   # pycodestyle
-    "F",   # Pyflakes
-    "I",   # isort
-    "UP",  # pyupgrade
-    "YTT", # flake8-2020
-    "ANN", # flake8-annotations
-    "S",   # flake8-bandit
-    "B",   # flake8-bugbear
-    "C4",  # flake8-comprehensions
-    "DTZ", # flake8-datetimez
-    "EM",  # flake8-errmsg
-    "EXE", # flake8-executable
-    "RET", # flake8-return
-    "ICN", # flake8-import-conventions
-    "INP", # flake8-no-pep420
-    "PIE", # flake8-pie
-    "PT",  # flake8-pytest-style
-    "SIM", # flake8-simplify
-    "PTH", # flake8-use-pathlib
-    "PL",  # Pylint
-    "TRY", # tryceratops
-    "RUF", # NumPy-specific rules
-    "G",   # flake8-logging-format
-    "D",   # pydocstyle
-]
-ignore = [
-    "E501",   # line-too-long
-    "S101",   # assert
-    "ANN101", # missing-type-self
-    "D203",   # one-blank-line-before-class
-    "D204",   # one-blank-line-after-class
-    "D213",   # multi-line-summary-second-line
-    "D407",   # dashed-underline-after-section
-    "D408",   # section-underline-after-name
-    "D409",   # section-underline-matches-section-length
-]
-line-length = 120
-target-version = "py38"
+[build-system]
+requires = ["flit_scm"]
+build-backend = "flit_scm:buildapi"
+
+[project]
+name = "tcod-ecs"
+authors = [{ name = "Kyle Benesch", email = "4b796c65+github@gmail.com" }]
+readme = "README.md"
+license = { file = "LICENSE" }
+classifiers = [
+    "Development Status :: 5 - Production/Stable",
+    "Intended Audience :: Developers",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+    "Programming Language :: Python :: 3",
+    "Topic :: Software Development :: Libraries :: Python Modules",
+    "Typing :: Typed",
+]
+dynamic = ["version", "description"]
+requires-python = ">=3.8"
+dependencies = ["typing-extensions >=4.4.0"]
+
+[tool.setuptools_scm]
+write_to = "tcod/ecs/_version.py"
+
+[project.optional-dependencies]
+test = [
+    "attrs >=22.2.0",
+    "pytest >=7.2.0",
+    "pytest-cov >=4.0.0",
+    "pytest-benchmark >=4.0.0",
+    "mypy >=1.1.1",
+]
+
+[tool.flit.module]
+name = "tcod.ecs"
+
+[project.urls]
+Home = "https://github.com/HexDecimal"
+Changelog = "https://github.com/HexDecimal/python-tcod-ecs/blob/main/CHANGELOG.md"
+Documentation = "https://python-tcod-ecs.readthedocs.io"
+Source = "https://github.com/HexDecimal/python-tcod-ecs"
+
+[tool.black] # https://black.readthedocs.io/en/stable/usage_and_configuration/the_basics.html#configuration-via-a-file
+target-version = ["py38"]
+line-length = 120
+
+[tool.isort] # https://pycqa.github.io/isort/docs/configuration/options.html
+py_version = "38"
+line_length = 120
+profile = "black"
+skip_gitignore = true
+
+[tool.mypy] # https://mypy.readthedocs.io/en/stable/config_file.html
+files = "**/*.py"
+explicit_package_bases = true
+python_version = "3.10"            # Type check Python version with EllipsisType.
+warn_unused_configs = true
+disallow_any_generics = true
+disallow_subclassing_any = true
+disallow_untyped_calls = true
+disallow_untyped_defs = true
+disallow_incomplete_defs = true
+check_untyped_defs = true
+disallow_untyped_decorators = true
+no_implicit_optional = true
+warn_redundant_casts = true
+warn_unused_ignores = true
+warn_return_any = true
+no_implicit_reexport = true
+strict_equality = true
+
+[tool.pytest.ini_options]
+minversion = "6.0"
+required_plugins = ["pytest-cov>=4.0.0", "pytest-benchmark>=4.0.0"]
+addopts = "--doctest-modules --cov=tcod --cov-report=term-missing --doctest-glob=*.md"
+testpaths = ["."]
+
+[tool.coverage.report] # https://coverage.readthedocs.io/en/latest/config.html
+exclude_lines = ['$\s*\.\.\.', "if TYPE_CHECKING:"]
+
+[tool.ruff]
+# https://beta.ruff.rs/docs/rules/
+select = [
+    "C90", # mccabe
+    "E",   # pycodestyle
+    "W",   # pycodestyle
+    "F",   # Pyflakes
+    "I",   # isort
+    "UP",  # pyupgrade
+    "YTT", # flake8-2020
+    "ANN", # flake8-annotations
+    "S",   # flake8-bandit
+    "B",   # flake8-bugbear
+    "C4",  # flake8-comprehensions
+    "DTZ", # flake8-datetimez
+    "EM",  # flake8-errmsg
+    "EXE", # flake8-executable
+    "RET", # flake8-return
+    "ICN", # flake8-import-conventions
+    "INP", # flake8-no-pep420
+    "PIE", # flake8-pie
+    "PT",  # flake8-pytest-style
+    "SIM", # flake8-simplify
+    "PTH", # flake8-use-pathlib
+    "PL",  # Pylint
+    "TRY", # tryceratops
+    "RUF", # NumPy-specific rules
+    "G",   # flake8-logging-format
+    "D",   # pydocstyle
+]
+ignore = [
+    "E501",   # line-too-long
+    "S101",   # assert
+    "ANN101", # missing-type-self
+    "ANN102", # missing-type-cls
+    "D203",   # one-blank-line-before-class
+    "D204",   # one-blank-line-after-class
+    "D213",   # multi-line-summary-second-line
+    "D407",   # dashed-underline-after-section
+    "D408",   # section-underline-after-name
+    "D409",   # section-underline-matches-section-length
+]
+line-length = 120
+target-version = "py38"
```

### Comparing `tcod-ecs-1.2.0/tcod/ecs/__init__.py` & `tcod_ecs-2.0.0/tcod/ecs/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,807 +1,913 @@
-"""A type-hinted Entity Component System based on Python dictionaries and sets."""
-from __future__ import annotations
-
-__version__ = "1.2.0"
-import sys
-from functools import partial
-from typing import (
-    TYPE_CHECKING,
-    AbstractSet,
-    Any,
-    DefaultDict,
-    Final,
-    Generic,
-    Iterable,
-    Iterator,
-    Mapping,
-    MutableMapping,
-    MutableSet,
-    Tuple,
-    Type,
-    TypeVar,
-    Union,
-    overload,
-)
-
-from typing_extensions import Self
-
-if sys.version_info >= (3, 10):
-    from types import EllipsisType
-else:
-    EllipsisType = Any
-
-T = TypeVar("T")
-_T1 = TypeVar("_T1")
-_T2 = TypeVar("_T2")
-_T3 = TypeVar("_T3")
-_T4 = TypeVar("_T4")
-_T5 = TypeVar("_T5")
-_ComponentKey = Union[Type[T], Tuple[object, Type[T]]]
-"""ComponentKey is plain `type` or tuple `(tag, type)`."""
-
-
-def abstract_component(cls: type[T]) -> type[T]:
-    """Register class `cls` as an abstract component and return it."""
-    cls._TCOD_BASE_COMPONENT = cls  # type: ignore[attr-defined]
-    return cls
-
-
-class Entity:
-    """A unique entity in a world.
-
-    Example::
-
-        >>> import tcod.ecs
-        >>> world = tcod.ecs.World()  # Create a new world.
-        >>> entity = world.new_entity(name="entity")  # Create a new entity, name is optional.
-        >>> other_entity = world.new_entity(name="other_entity")
-    """  # Changes here should be reflected in conftest.py.
-
-    __slots__ = ("world", "__weakref__")
-
-    def __init__(self, world: World) -> None:
-        """Initialize a new unique entity."""
-        self.world: Final = world
-        """The :any:`World` this entity belongs to."""
-
-    @property
-    def components(self) -> EntityComponents:
-        """Access an entities components.
-
-        Example::
-
-            >>> entity.components[str] = "foo"  # Assign component.
-            >>> entity.components[("name", str)] = "my_name" # Assign named component.
-            >>> ("name", str) in entity.components
-            True
-            >>> {str, ("name", str)}.issubset(entity.components.keys())
-            True
-            >>> list(world.Q.all_of(components=[str]))  # Query components.
-            [<Entity name='entity'>]
-            >>> list(world.Q[tcod.ecs.Entity, str, ("name", str)])  # Query zip components.
-            [(<Entity name='entity'>, 'foo', 'my_name')]
-        """
-        return EntityComponents(self)
-
-    @property
-    def tags(self) -> EntityTags:
-        """Access an entities tags.
-
-        Example::
-
-            >>> entity.tags.add("tag") # Add tag.
-            >>> "tag" in entity.tags  # Check tag.
-            True
-            >>> list(world.Q.all_of(tags=["tag"]))  # Query tags.
-            [<Entity name='entity'>]
-            >>> entity.tags.discard("tag")
-        """
-        return EntityTags(self)
-
-    @property
-    def relation_components(self) -> EntityComponentRelations:
-        """Access an entities relation components.
-
-        Example::
-
-            >>> entity.relation_components[str][other_entity] = "foo" # Assign component to relation.
-            >>> entity.relation_components[("distance", int)][other_entity] = 42 # Also works for named components.
-            >>> other_entity in entity.relation_components[str]
-            True
-            >>> list(world.Q.all_of(relations=[(str, other_entity)]))
-            [<Entity name='entity'>]
-            >>> list(world.Q.all_of(relations=[(str, ...)]))
-            [<Entity name='entity'>]
-            >>> list(world.Q.all_of(relations=[(entity, str, None)]))
-            [<Entity name='other_entity'>]
-            >>> list(world.Q.all_of(relations=[(..., str, None)]))
-            [<Entity name='other_entity'>]
-        """
-        return EntityComponentRelations(self)
-
-    @property
-    def relation_tags(self) -> EntityRelationsExclusive:
-        """Access an entities exclusive relations.
-
-        Example::
-
-            >>> entity.relation_tags["ChildOf"] = other_entity  # Assign relation.
-            >>> list(world.Q.all_of(relations=[("ChildOf", other_entity)]))  # Get children of other_entity.
-            [<Entity name='entity'>]
-            >>> list(world.Q.all_of(relations=[(entity, "ChildOf", None)]))  # Get parents of entity.
-            [<Entity name='other_entity'>]
-            >>> del entity.relation_tags["ChildOf"]
-        """
-        return EntityRelationsExclusive(self)
-
-    @property
-    def relation_tags_many(self) -> EntityRelations:
-        """Access an entities many-to-many relations.
-
-        Example::
-
-            >>> entity.relation_tags_many["KnownBy"].add(other_entity)  # Assign relation.
-        """
-        return EntityRelations(self)
-
-    @property
-    def name(self) -> object:
-        """The unique name of this entity or None.
-
-        You may assign a new name, but if an entity of the world already has that name then it will lose it.
-        """
-        return self.world._names_by_entity.get(self)
-
-    @name.setter
-    def name(self, value: object) -> None:
-        old_name = self.name
-        if old_name is not None:  # Remove self from names.
-            del self.world._names_by_name[old_name]
-            del self.world._names_by_entity[self]
-
-        if value is not None:  # Add self to names.
-            old_entity = self.world._names_by_name.get(value)
-            if old_entity is not None:  # Remove entity with old name, name will be overwritten.
-                del self.world._names_by_entity[old_entity]
-            self.world._names_by_name[value] = self
-            self.world._names_by_entity[self] = value
-
-    def __repr__(self) -> str:
-        """Return a representation of this entity."""
-        items = [self.__class__.__name__]
-        name = self.name
-        items.append(f"0x{id(self):X}" if name is None else f"name={name!r}")
-        return f"<{' '.join(items)}>"
-
-    def __reduce__(self) -> tuple[type[Entity], tuple[World]]:  # Private function.  # noqa: D105
-        # Note: This was added after version 1.0.0, objects pickled in <=1.0.0 will call __setstate__.
-        return self.__class__, (self.world,)
-
-
-class EntityComponents(MutableMapping[Union[Type[Any], Tuple[object, Type[Any]]], Any]):
-    """A proxy attribute to access an entities components like a dictionary.
-
-    See :any:`Entity.components`.
-    """
-
-    __slots__ = ("entity",)
-
-    def __init__(self, entity: Entity) -> None:
-        """Initialize this attribute for the given entity."""
-        self.entity: Final = entity
-
-    def set(self, value: object) -> None:
-        """Assign or overwrite a component, automatically deriving the key."""
-        key = getattr(value, "_TCOD_BASE_COMPONENT", value.__class__)
-        self[key] = value
-
-    @staticmethod
-    def __assert_key(key: _ComponentKey[Any]) -> bool:
-        """Verify that abstract classes are accessed correctly."""
-        if isinstance(key, tuple):
-            key = key[1]
-        assert (
-            getattr(key, "_TCOD_BASE_COMPONENT", key) is key
-        ), "Abstract components must be accessed via the base class."
-        return True
-
-    def __getitem__(self, key: _ComponentKey[T]) -> T:
-        """Return a component belonging to this entity."""
-        assert self.__assert_key(key)
-        return self.entity.world._components_by_type[key][self.entity]  # type: ignore[no-any-return]
-
-    def __setitem__(self, key: _ComponentKey[T], value: T) -> None:
-        """Assign a component to an entity."""
-        assert self.__assert_key(key)
-        self.entity.world._components_by_type[key][self.entity] = value
-        self.entity.world._components_by_entity[self.entity].add(key)
-
-    def __delitem__(self, key: type[object] | tuple[object, type[object]]) -> None:
-        """Delete a component from an entity."""
-        assert self.__assert_key(key)
-
-        del self.entity.world._components_by_type[key][self.entity]
-        if not self.entity.world._components_by_type[key]:
-            del self.entity.world._components_by_type[key]
-
-        self.entity.world._components_by_entity[self.entity].remove(key)
-        if not self.entity.world._components_by_entity[self.entity]:
-            del self.entity.world._components_by_entity[self.entity]
-
-    def __contains__(self, key: _ComponentKey[object]) -> bool:  # type: ignore[override]
-        """Return True if this entity has the provided component."""
-        return key in self.entity.world._components_by_entity.get(self.entity, ())
-
-    def __iter__(self) -> Iterator[_ComponentKey[Any]]:
-        """Iterate over the component types belonging to this entity."""
-        return iter(self.entity.world._components_by_entity.get(self.entity, ()))
-
-    def __len__(self) -> int:
-        """Return the number of components belonging to this entity."""
-        return len(self.entity.world._components_by_entity.get(self.entity, ()))
-
-    def update_values(self, values: Iterable[object]) -> None:
-        """Add or overwrite multiple components inplace, deriving the keys from the values."""
-        for value in values:
-            self.set(value)
-
-    if TYPE_CHECKING:  # Type-hinted overrides
-
-        @overload
-        def get(self, __key: _ComponentKey[T]) -> T | None:
-            ...
-
-        @overload
-        def get(self, __key: _ComponentKey[T], __default: T) -> T:
-            ...
-
-        def get(self, __key: _ComponentKey[T], __default: T | None = None) -> T | None:
-            """Return a component, returns None or a default value when the component is missing."""
-
-        def setdefault(self, __key: _ComponentKey[T], __default: T) -> T:  # type: ignore[override]
-            """Assign a default value if a component is missing, then returns the current value."""
-
-
-class EntityTags(MutableSet[Any]):
-    """A proxy attribute to access an entities tags like a set.
-
-    See :any:`Entity.tags`.
-    """
-
-    __slots__ = ("entity",)
-
-    def __init__(self, entity: Entity) -> None:
-        """Initialize this attribute for the given entity."""
-        self.entity: Final = entity
-
-    def add(self, tag: object) -> None:
-        """Add a tag to the entity."""
-        self.entity.world._tags_by_entity[self.entity].add(tag)
-        self.entity.world._tags_by_key[tag].add(self.entity)
-
-    def discard(self, tag: object) -> None:
-        """Discard a tag from an entity."""
-        self.entity.world._tags_by_entity[self.entity].discard(tag)
-        if not self.entity.world._tags_by_entity[self.entity]:
-            del self.entity.world._tags_by_entity[self.entity]
-
-        self.entity.world._tags_by_key[tag].discard(self.entity)
-        if not self.entity.world._tags_by_key[tag]:
-            del self.entity.world._tags_by_key[tag]
-
-    def __contains__(self, x: object) -> bool:
-        """Return True if this entity has the given tag."""
-        return x in self.entity.world._tags_by_entity.get(self.entity, ())
-
-    def __iter__(self) -> Iterator[Any]:
-        """Iterate over this entities tags."""
-        return iter(self.entity.world._tags_by_entity.get(self.entity, ()))
-
-    def __len__(self) -> int:
-        """Return the number of tags this entity has."""
-        return len(self.entity.world._tags_by_entity.get(self.entity, ()))
-
-
-class EntityRelationsMapping(MutableSet[Entity]):
-    """A proxy attribute to access entity relation targets like a set.
-
-    See :any:`Entity.relation_tags_many`.
-    """
-
-    __slots__ = ("entity", "key")
-
-    def __init__(self, entity: Entity, key: object) -> None:
-        """Initialize this attribute for the given entity."""
-        self.entity: Final = entity
-        self.key: Final = key
-        assert key not in {None, Ellipsis}
-
-    def add(self, target: Entity) -> None:
-        """Add a relation target to this tag."""
-        world = self.entity.world
-        world._relation_tags_by_entity[self.entity][self.key].add(target)
-
-        world._relations_lookup[(self.key, target)].add(self.entity)
-        world._relations_lookup[(self.key, ...)].add(self.entity)
-        world._relations_lookup[(self.entity, self.key, None)].add(target)
-        world._relations_lookup[(..., self.key, None)].add(target)
-
-    def discard(self, target: Entity) -> None:
-        """Discard a relation target from this tag."""
-        world = self.entity.world
-
-        world._relation_tags_by_entity[self.entity][self.key].discard(target)
-        if not world._relation_tags_by_entity[self.entity][self.key]:
-            del world._relation_tags_by_entity[self.entity][self.key]
-            if not world._relation_tags_by_entity[self.entity]:
-                del world._relation_tags_by_entity[self.entity]
-
-        world._relations_lookup[(self.key, target)].discard(self.entity)
-        if not world._relations_lookup[(self.key, target)]:
-            del world._relations_lookup[(self.key, target)]
-
-        world._relations_lookup[(self.key, ...)].discard(self.entity)
-        if not world._relations_lookup[(self.key, ...)]:
-            del world._relations_lookup[(self.key, ...)]
-
-        world._relations_lookup[(self.entity, self.key, None)].discard(target)
-        if not world._relations_lookup[(self.entity, self.key, None)]:
-            del world._relations_lookup[(self.entity, self.key, None)]
-
-        world._relations_lookup[(..., self.key, None)].discard(target)
-        if not world._relations_lookup[(..., self.key, None)]:
-            del world._relations_lookup[(..., self.key, None)]
-
-    def __contains__(self, target: Entity) -> bool:  # type: ignore[override]
-        """Return True if this relation contains the given value."""
-        return bool(self.entity.world._relations_lookup.get((self.key, target), ()))
-
-    def __iter__(self) -> Iterator[Entity]:
-        """Iterate over this relation tags targets."""
-        by_entity = self.entity.world._relation_tags_by_entity.get(self.entity)
-        return iter(by_entity.get(self.key, ())) if by_entity is not None else iter(())
-
-    def __len__(self) -> int:
-        """Return the number of targets for this relation tag."""
-        by_entity = self.entity.world._relation_tags_by_entity.get(self.entity)
-        return len(by_entity.get(self.key, ())) if by_entity is not None else 0
-
-
-class EntityRelations(MutableMapping[object, EntityRelationsMapping]):
-    """A proxy attribute to access entity relations like a dict of sets.
-
-    See :any:`Entity.relation_tags_many`.
-    """
-
-    __slots__ = ("entity",)
-
-    def __init__(self, entity: Entity) -> None:
-        """Initialize this attribute for the given entity."""
-        self.entity: Final = entity
-
-    def __getitem__(self, key: object) -> EntityRelationsMapping:
-        """Return the relation mapping for a tag."""
-        return EntityRelationsMapping(self.entity, key)
-
-    def __setitem__(self, key: object, values: Iterable[Entity]) -> None:
-        """Overwrite the targets of a relation tag with the new values."""
-        assert not isinstance(values, Entity), "Did you mean `entity.relations[key] = (target,)`?"
-        mapping = EntityRelationsMapping(self.entity, key)
-        mapping.clear()
-        for v in values:
-            mapping.add(v)
-
-    def __delitem__(self, key: object) -> None:
-        """Clear the relation tags of an entity.
-
-        This does not remove relation tags towards this entity.
-        """
-        self[key].clear()
-
-    def __iter__(self) -> Iterator[Any]:
-        """Iterate over the unique relation tags of this entity."""
-        return iter(self.entity.world._relation_tags_by_entity.get(self.entity, {}).keys())
-
-    def __len__(self) -> int:
-        """Return the number of unique relation tags this entity has."""
-        return len(self.entity.world._relation_tags_by_entity.get(self.entity, {}))
-
-
-class EntityRelationsExclusive(MutableMapping[object, Entity]):
-    """A proxy attribute to access entity relations exclusively.
-
-    See :any:`Entity.relation_tags`.
-    """
-
-    __slots__ = ("entity",)
-
-    def __init__(self, entity: Entity) -> None:
-        """Initialize this attribute for the given entity."""
-        self.entity: Final = entity
-
-    def __getitem__(self, key: object) -> Entity:
-        """Return the relation target for a key.
-
-        If the relation has no target then raises KeyError.
-        If the relation is not exclusive then raises ValueError.
-        """
-        values = tuple(EntityRelationsMapping(self.entity, key))
-        if not values:
-            raise KeyError(key)
-        try:
-            (target,) = values
-        except ValueError:
-            msg = "Entity relation has multiple targets but an exclusive value was expected."
-            raise ValueError(msg) from None
-        return target
-
-    def __setitem__(self, key: object, target: Entity) -> None:
-        """Set a relation exclusively to a new target."""
-        mapping = EntityRelationsMapping(self.entity, key)
-        mapping.clear()
-        mapping.add(target)
-
-    def __delitem__(self, key: object) -> None:
-        """Clear the relation targets of a relation key."""
-        EntityRelationsMapping(self.entity, key).clear()
-
-    def __iter__(self) -> Iterator[Any]:
-        """Iterate over the keys of this entities relations."""
-        return EntityRelations(self.entity).__iter__()
-
-    def __len__(self) -> int:
-        """Return the number of relations this entity has."""
-        return EntityRelations(self.entity).__len__()
-
-
-class EntityComponentRelationMapping(Generic[T], MutableMapping[Entity, T]):
-    """An entity-component mapping to access the relation target component objects.
-
-    See :any:`Entity.relation_components`.
-    """
-
-    __slots__ = ("entity", "key")
-
-    def __init__(self, entity: Entity, key: _ComponentKey[T]) -> None:
-        """Initialize this attribute for the given entity."""
-        assert isinstance(entity, Entity), entity
-        self.entity: Final = entity
-        self.key: _ComponentKey[T] = key
-
-    def __getitem__(self, target: Entity) -> T:
-        """Return the component related to a target entity."""
-        return self.entity.world._relation_components_by_entity[self.entity][self.key][target]  # type: ignore[no-any-return]
-
-    def __setitem__(self, target: Entity, component: T) -> None:
-        """Assign a component to the target entity."""
-        world = self.entity.world
-        if target in world._relation_components_by_entity[self.entity][self.key] is not None:
-            del self[target]
-        world._relation_components_by_entity[self.entity][self.key][target] = component
-
-        world._relations_lookup[(self.key, target)] = {self.entity}
-        world._relations_lookup[(self.key, ...)].add(self.entity)
-        world._relations_lookup[(self.entity, self.key, None)] = {target}
-        world._relations_lookup[(..., self.key, None)].add(target)
-
-    def __delitem__(self, target: Entity) -> None:
-        """Delete a component assigned to the target entity."""
-        world = self.entity.world
-        del world._relation_components_by_entity[self.entity][self.key][target]
-        if not world._relation_components_by_entity[self.entity][self.key]:
-            del world._relation_components_by_entity[self.entity][self.key]
-        if not world._relation_components_by_entity[self.entity]:
-            del world._relation_components_by_entity[self.entity]
-
-        world._relations_lookup[(self.key, target)].discard(self.entity)
-        if not world._relations_lookup[(self.key, target)]:
-            del world._relations_lookup[(self.key, target)]
-
-        world._relations_lookup[(self.key, ...)].discard(self.entity)
-        if not world._relations_lookup[(self.key, ...)]:
-            del world._relations_lookup[(self.key, ...)]
-
-        world._relations_lookup[(self.entity, self.key, None)].discard(self.entity)
-        if not world._relations_lookup[(self.entity, self.key, None)]:
-            del world._relations_lookup[(self.entity, self.key, None)]
-
-        world._relations_lookup[(..., self.key, None)].discard(self.entity)
-        if not world._relations_lookup[(..., self.key, None)]:
-            del world._relations_lookup[(..., self.key, None)]
-
-    def __iter__(self) -> Iterator[Entity]:
-        """Iterate over the targets with assigned components."""
-        by_entity = self.entity.world._relation_components_by_entity.get(self.entity)
-        return iter(()) if by_entity is None else iter(by_entity.get(self.key, ()))
-
-    def __len__(self) -> int:
-        """Return the count of targets for this component relation."""
-        by_entity = self.entity.world._relation_components_by_entity.get(self.entity)
-        return 0 if by_entity is None else len(by_entity.get(self.key, ()))
-
-
-class EntityComponentRelations:
-    """Proxy to access the component relations of an entity.
-
-    See :any:`Entity.relation_components`.
-    """
-
-    __slots__ = ("entity",)
-
-    def __init__(self, entity: Entity) -> None:
-        """Initialize this attribute for the given entity."""
-        assert isinstance(entity, Entity), entity
-        self.entity: Final = entity
-
-    def __getitem__(self, key: _ComponentKey[T]) -> EntityComponentRelationMapping[T]:
-        """Access relations for this component key as a `{target: component}` dict-like object."""
-        return EntityComponentRelationMapping(self.entity, key)
-
-    def __delitem__(self, key: _ComponentKey[object]) -> None:
-        """Remove all relations associated with this component key."""
-        EntityComponentRelationMapping(self.entity, key).clear()
-
-
-class World:
-    """A container for entities and components."""
-
-    def __init__(self) -> None:
-        """Initialize a new world."""
-        self._components_by_type: DefaultDict[_ComponentKey[object], dict[Entity, Any]] = DefaultDict(dict)
-        """Query table entity components.
-
-        dict[ComponentKey][Entity] = component_instance
-        """
-        self._components_by_entity: DefaultDict[Entity, set[_ComponentKey[object]]] = DefaultDict(set)
-        """Random access entity components.
-
-        dict[Entity] = {component_keys_owned_by_entity}
-        """
-
-        self._tags_by_key: DefaultDict[object, set[Entity]] = DefaultDict(set)
-        """Query table entity tags.
-
-        dict[tag] = {all_entities_with_tag}
-        """
-        self._tags_by_entity: DefaultDict[Entity, set[Any]] = DefaultDict(set)
-        """Random access entity tags.
-
-        dict[Entity] = {all_tags_for_entity}
-        """
-
-        self._relation_tags_by_entity: DefaultDict[Entity, DefaultDict[object, set[Entity]]] = DefaultDict(
-            partial(DefaultDict, set)  # type: ignore[arg-type]
-        )
-        """Random access tag multi-relations.
-
-        dict[entity][tag] = {target_entities}
-        """
-        self._relation_components_by_entity: DefaultDict[
-            Entity, DefaultDict[_ComponentKey[object], dict[Entity, Any]]
-        ] = DefaultDict(
-            partial(DefaultDict, dict)  # type: ignore[arg-type]
-        )
-        """Random access relations owning components.
-
-        dict[entity][ComponentKey][target_entity] = component
-        """
-        self._relations_lookup: DefaultDict[
-            tuple[Any, Entity | EllipsisType] | tuple[Entity | EllipsisType, Any, None], set[Entity]
-        ] = DefaultDict(set)
-        """Relations query table.  Tags and components are mixed together.
-
-        Tag:
-            dict[(tag, this_entity)] = {target_entities_for_entity}
-            dict[(tag, None)] = {target_entities_for_tag}
-            dict[(target_entity, tag, None)] = {origin_entities_for_target}
-            dict[(None, tag, None)] = {all_origen_entities_for_tag}
-        Component:
-            dict[(ComponentKey, target_entity)] = {origin_entities}
-            dict[(ComponentKey, None)] = {all_origin_entities}
-            dict[(origin_entity, ComponentKey, None)] = {target_entities}
-            dict[(None, ComponentKey, None)] = {all_target_entities}
-        """
-
-        self._names_by_name: dict[object, Entity] = {}
-        """Name query table.
-
-        dict[name] = named_entity
-        """
-        self._names_by_entity: dict[Entity, object] = {}
-        """Name lookup table.
-
-        dict[Entity] = entities_name
-        """
-
-        self.global_: Final = Entity(self)
-        """A unique globally accessible entity.
-
-        This can be used to store globally accessible components in the world itself without any extra boilerplate.
-        Otherwise this entity is not special and will show up with other entities in queries, etc.
-
-        .. versionadded:: 1.1
-
-        Example::
-
-            >>> world.global_.components[("turn", int)] = 0
-        """
-
-    def __setstate__(self, state: dict[str, Any]) -> None:
-        """Unpickle this object and handle state migration."""
-        # Migrate from version <=1.0.0.
-        state.setdefault("global_", Entity(self))
-        if "_relation_components" in state:
-            _relation_components: dict[_ComponentKey[object], dict[Entity, dict[Entity, Any]]] = state.pop(
-                "_relation_components"
-            )
-            self._relation_components_by_entity = DefaultDict(partial(DefaultDict, dict))  # type: ignore[arg-type]
-            for component_key, component_key_relations in _relation_components.items():
-                for entity, entities_component_table in component_key_relations.items():
-                    for target_entity, target_component in entities_component_table.items():
-                        self._relation_components_by_entity[entity][component_key][target_entity] = target_component
-
-            _relations_by_key: dict[object, dict[Entity, set[Entity]]] = state.pop("_relations_by_key")
-            self._relation_tags_by_entity = DefaultDict(partial(DefaultDict, set))  # type: ignore[arg-type]
-            for tag, tag_relations in _relations_by_key.items():
-                for entity, targets in tag_relations.items():
-                    self._relation_tags_by_entity[entity][tag] = targets
-
-        self.__dict__.update(state)
-
-    @property
-    def named(self) -> Mapping[object, Entity]:
-        """A view into this worlds named entities."""
-        return self._names_by_name
-
-    def new_entity(
-        self,
-        components: Iterable[object] = (),
-        *,
-        name: object = None,
-        tags: Iterable[Any] = (),
-    ) -> Entity:
-        """Create and return a new entity."""
-        entity = Entity(self)
-        entity.components.update_values(components)
-        entity_tags = entity.tags
-        for tag in tags:
-            entity_tags.add(tag)
-        entity.name = name
-        return entity
-
-    @property
-    def Q(self) -> Query:
-        """Start a new Query for this world.
-
-        Alias for ``tcod.ecs.Query(world)``.
-        """
-        return Query(self)
-
-
-class Query:
-    """Collect a set of entities with the provided conditions."""
-
-    def __init__(self, world: World) -> None:
-        """Initialize a Query."""
-        self.world: Final = world
-
-        self._all_of_components: set[_ComponentKey[object]] = set()
-        self._none_of_components: set[_ComponentKey[object]] = set()
-        self._all_of_tags: set[object] = set()
-        self._none_of_tags: set[object] = set()
-        self._all_of_relations: set[tuple[Any, Entity | EllipsisType] | tuple[Entity | EllipsisType, Any, None]] = set()
-        self._none_of_relations: set[
-            tuple[Any, Entity | EllipsisType] | tuple[Entity | EllipsisType, Any, None]
-        ] = set()
-
-    def __iter_requires(self, extra_components: AbstractSet[_ComponentKey[object]]) -> Iterator[AbstractSet[Entity]]:
-        collect_components = self._all_of_components | extra_components
-        for component in collect_components:
-            yield self.world._components_by_type.get(component, {}).keys()
-        for tag in self._all_of_tags:
-            yield self.world._tags_by_key.get(tag, set())
-        for relation in self._all_of_relations:
-            yield self.world._relations_lookup.get(relation, set())
-
-    def __iter_excludes(self) -> Iterator[AbstractSet[Entity]]:
-        for component in self._none_of_components:
-            yield self.world._components_by_type.get(component, {}).keys()
-        for tag in self._none_of_tags:
-            yield self.world._tags_by_key.get(tag, set())
-        for relation in self._none_of_relations:
-            yield self.world._relations_lookup.get(relation, set())
-
-    def _get_entities(self, extra_components: AbstractSet[_ComponentKey[object]] = frozenset()) -> set[Entity]:
-        # Place the smallest sets first to speed up intersections.
-        requires = sorted(self.__iter_requires(extra_components), key=len)
-        excludes = list(self.__iter_excludes())
-
-        if not requires:
-            if excludes:
-                msg = "A Query can not function only excluding entities."
-            else:
-                msg = "This Query did not include any entities."
-            raise AssertionError(msg)
-
-        entities = set(requires[0])
-        for require in requires[1:]:
-            entities.intersection_update(require)
-        for exclude in excludes:
-            entities.difference_update(exclude)
-        return entities
-
-    def all_of(
-        self,
-        components: Iterable[_ComponentKey[object]] = (),
-        *,
-        tags: Iterable[object] = (),
-        relations: Iterable[tuple[object, Entity | EllipsisType] | tuple[Entity | EllipsisType, Any, None]] = (),
-    ) -> Self:
-        """Filter entities based on having all of the provided elements."""
-        self._all_of_components.update(components)
-        self._all_of_tags.update(tags)
-        self._all_of_relations.update(relations)
-        return self
-
-    def none_of(
-        self,
-        components: Iterable[_ComponentKey[object]] = (),
-        *,
-        tags: Iterable[object] = (),
-        relations: Iterable[tuple[object, Entity | EllipsisType] | tuple[Entity | EllipsisType, Any, None]] = (),
-    ) -> Self:
-        """Filter entities based on having none of the provided elements."""
-        self._none_of_components.update(components)
-        self._none_of_tags.update(tags)
-        self._none_of_relations.update(relations)
-        return self
-
-    def __iter__(self) -> Iterator[Entity]:
-        """Iterate over the matching entities."""
-        return iter(self._get_entities())
-
-    @overload
-    def __getitem__(self, key: tuple[_ComponentKey[_T1]]) -> Iterable[tuple[_T1]]:
-        ...
-
-    @overload
-    def __getitem__(self, key: tuple[_ComponentKey[_T1], _ComponentKey[_T2]]) -> Iterable[tuple[_T1, _T2]]:
-        ...
-
-    @overload
-    def __getitem__(
-        self, key: tuple[_ComponentKey[_T1], _ComponentKey[_T2], _ComponentKey[_T3]]
-    ) -> Iterable[tuple[_T1, _T2, _T3]]:
-        ...
-
-    @overload
-    def __getitem__(
-        self, key: tuple[_ComponentKey[_T1], _ComponentKey[_T2], _ComponentKey[_T3], _ComponentKey[_T4]]
-    ) -> Iterable[tuple[_T1, _T2, _T3, _T4]]:
-        ...
-
-    @overload
-    def __getitem__(
-        self,
-        key: tuple[_ComponentKey[_T1], _ComponentKey[_T2], _ComponentKey[_T3], _ComponentKey[_T4], _ComponentKey[_T5]],
-    ) -> Iterable[tuple[_T1, _T2, _T3, _T4, _T5]]:
-        ...
-
-    @overload
-    def __getitem__(self, key: tuple[_ComponentKey[object], ...]) -> Iterable[tuple[Any, ...]]:
-        ...
-
-    def __getitem__(self, key: tuple[_ComponentKey[object], ...]) -> Iterable[tuple[Any, ...]]:
-        """Collect components from a query."""
-        assert key is not None
-        assert isinstance(key, tuple)
-
-        entities = list(self._get_entities(set(key) - {Entity}))
-        entity_components = []
-        for component_key in key:
-            if component_key is Entity:
-                entity_components.append(entities)
-                continue
-            world_components = self.world._components_by_type[component_key]
-            entity_components.append([world_components[entity] for entity in entities])
-        return zip(*entity_components)
+"""A type-hinted Entity Component System based on Python dictionaries and sets."""
+from __future__ import annotations
+
+import sys
+from collections import defaultdict
+from functools import partial
+from typing import (
+    TYPE_CHECKING,
+    AbstractSet,
+    Any,
+    Final,
+    Generic,
+    Iterable,
+    Iterator,
+    Mapping,
+    MutableMapping,
+    MutableSet,
+    Tuple,
+    Type,
+    TypeVar,
+    Union,
+    overload,
+)
+from weakref import WeakKeyDictionary, WeakValueDictionary
+
+from typing_extensions import Self
+
+from tcod.ecs import _version
+
+__version__ = _version.__version__
+
+if sys.version_info >= (3, 10):
+    from types import EllipsisType
+else:
+    EllipsisType = Any
+
+T = TypeVar("T")
+_T1 = TypeVar("_T1")
+_T2 = TypeVar("_T2")
+_T3 = TypeVar("_T3")
+_T4 = TypeVar("_T4")
+_T5 = TypeVar("_T5")
+_ComponentKey = Union[Type[T], Tuple[object, Type[T]]]
+"""ComponentKey is plain `type` or tuple `(tag, type)`."""
+
+
+def abstract_component(cls: type[T]) -> type[T]:
+    """Register class `cls` as an abstract component and return it."""
+    cls._TCOD_BASE_COMPONENT = cls  # type: ignore[attr-defined]
+    return cls
+
+
+_entity_table: WeakKeyDictionary[World, WeakValueDictionary[object, Entity]] = WeakKeyDictionary()
+"""A weak table of worlds and unique identifiers to entity objects.
+
+This table is used to that non-unique Entity's won't create a new object and thus will always share identities.
+
+_entity_table[world][uid] = entity
+"""
+
+
+class Entity:
+    """A unique entity in a world.
+
+    Example::
+
+        >>> import tcod.ecs
+        >>> world = tcod.ecs.World()  # Create a new world.
+        >>> entity = world.new_entity(name="entity")  # Create a new entity, name is optional.
+        >>> other_entity = world.new_entity(name="other_entity")
+    """  # Changes here should be reflected in conftest.py.
+
+    __slots__ = ("world", "uid", "__weakref__")
+
+    world: Final[World]  # type:ignore[misc]  # https://github.com/python/mypy/issues/5774
+    """The :any:`World` this entity belongs to."""
+    uid: Final[object]  # type:ignore[misc]
+    """This entities unique identifier."""
+
+    def __new__(cls, world: World, uid: object = object) -> Entity:
+        """Return a unique entity for the given `world` and `uid`.
+
+        If an entity already exists with a matching `world` and `uid` then that entity is returned.
+
+        The `uid` default of `object` will create an instance of :any:`object` as the `uid`.
+        An entity created this way will never match or collide with an existing entity.
+
+        Example::
+
+            >>> world = World()
+            >>> Entity(world, "foo")
+            <Entity(uid='foo')>
+            >>> Entity(world, "foo") is Entity(world, "foo")
+            True
+            >>> Entity(world) is Entity(world)
+            False
+        """
+        if uid is object:
+            uid = object()
+        try:
+            table = _entity_table[world]
+        except KeyError:
+            table = WeakValueDictionary()
+            _entity_table[world] = table
+        try:
+            return table[uid]
+        except KeyError:
+            pass
+        self = super().__new__(cls)
+        self.world = world  # type:ignore[misc]  # https://github.com/python/mypy/issues/5774
+        self.uid = uid  # type:ignore[misc]
+        _entity_table[world][uid] = self
+        return self
+
+    @property
+    def components(self) -> EntityComponents:
+        """Access an entities components.
+
+        Example::
+
+            >>> entity.components[str] = "foo"  # Assign component.
+            >>> entity.components[("name", str)] = "my_name" # Assign named component.
+            >>> ("name", str) in entity.components
+            True
+            >>> {str, ("name", str)}.issubset(entity.components.keys())
+            True
+            >>> list(world.Q.all_of(components=[str]))  # Query components.
+            [<Entity name='entity'>]
+            >>> list(world.Q[tcod.ecs.Entity, str, ("name", str)])  # Query zip components.
+            [(<Entity name='entity'>, 'foo', 'my_name')]
+        """
+        return EntityComponents(self)
+
+    @property
+    def tags(self) -> EntityTags:
+        """Access an entities tags.
+
+        Example::
+
+            >>> entity.tags.add("tag") # Add tag.
+            >>> "tag" in entity.tags  # Check tag.
+            True
+            >>> list(world.Q.all_of(tags=["tag"]))  # Query tags.
+            [<Entity name='entity'>]
+            >>> entity.tags.discard("tag")
+        """
+        return EntityTags(self)
+
+    @property
+    def relation_components(self) -> EntityComponentRelations:
+        """Access an entities relation components.
+
+        Example::
+
+            >>> entity.relation_components[str][other_entity] = "foo" # Assign component to relation.
+            >>> entity.relation_components[("distance", int)][other_entity] = 42 # Also works for named components.
+            >>> other_entity in entity.relation_components[str]
+            True
+            >>> list(world.Q.all_of(relations=[(str, other_entity)]))
+            [<Entity name='entity'>]
+            >>> list(world.Q.all_of(relations=[(str, ...)]))
+            [<Entity name='entity'>]
+            >>> list(world.Q.all_of(relations=[(entity, str, None)]))
+            [<Entity name='other_entity'>]
+            >>> list(world.Q.all_of(relations=[(..., str, None)]))
+            [<Entity name='other_entity'>]
+        """
+        return EntityComponentRelations(self)
+
+    @property
+    def relation_tags(self) -> EntityRelationsExclusive:
+        """Access an entities exclusive relations.
+
+        Example::
+
+            >>> entity.relation_tags["ChildOf"] = other_entity  # Assign relation.
+            >>> list(world.Q.all_of(relations=[("ChildOf", other_entity)]))  # Get children of other_entity.
+            [<Entity name='entity'>]
+            >>> list(world.Q.all_of(relations=[(entity, "ChildOf", None)]))  # Get parents of entity.
+            [<Entity name='other_entity'>]
+            >>> del entity.relation_tags["ChildOf"]
+        """
+        return EntityRelationsExclusive(self)
+
+    @property
+    def relation_tags_many(self) -> EntityRelations:
+        """Access an entities many-to-many relations.
+
+        Example::
+
+            >>> entity.relation_tags_many["KnownBy"].add(other_entity)  # Assign relation.
+        """
+        return EntityRelations(self)
+
+    @property
+    def name(self) -> object:
+        """The unique name of this entity or None.
+
+        You may assign a new name, but if an entity of the world already has that name then it will lose it.
+        """
+        return self.world._names_by_entity.get(self)
+
+    @name.setter
+    def name(self, value: object) -> None:
+        old_name = self.name
+        if old_name is not None:  # Remove self from names.
+            del self.world._names_by_name[old_name]
+            del self.world._names_by_entity[self]
+
+        if value is not None:  # Add self to names.
+            old_entity = self.world._names_by_name.get(value)
+            if old_entity is not None:  # Remove entity with old name, name will be overwritten.
+                del self.world._names_by_entity[old_entity]
+            self.world._names_by_name[value] = self
+            self.world._names_by_entity[self] = value
+
+    def __repr__(self) -> str:
+        """Return a representation of this entity.
+
+        Example::
+
+            >>> world.new_entity()
+            <Entity(uid=object at ...)>
+            >>> world["foo"]
+            <Entity(uid='foo')>
+            >>> world.new_entity(name="foo")
+            <Entity name='foo'>
+        """
+        uid_str = f"object at 0x{id(self.uid):X}" if self.uid.__class__ == object else repr(self.uid)
+        items = [f"{self.__class__.__name__}(uid={uid_str})"]
+        name = self.name
+        if name is not None:  # Switch to older style.
+            items = [self.__class__.__name__, f"name={name!r}"]
+        return f"<{' '.join(items)}>"
+
+    def __reduce__(self) -> tuple[type[Entity], tuple[World, object]]:
+        """Pickle this Entity.
+
+        Note that any pickled entity will include the world it belongs to and all the entities of that world.
+        """
+        # Note: This was added after version 1.0.0, objects pickled in <=1.0.0 will call __setstate__.
+        return self.__class__, (self.world, self.uid)
+
+    def _force_remap(self, new_uid: object) -> None:
+        """Remap this Entity to a new uid, both and old and new uid's will use this entity."""
+        _entity_table[self.world][new_uid] = self
+        self.uid = new_uid  # type: ignore[misc]
+
+
+class EntityComponents(MutableMapping[Union[Type[Any], Tuple[object, Type[Any]]], Any]):
+    """A proxy attribute to access an entities components like a dictionary.
+
+    See :any:`Entity.components`.
+    """
+
+    __slots__ = ("entity",)
+
+    def __init__(self, entity: Entity) -> None:
+        """Initialize this attribute for the given entity."""
+        self.entity: Final = entity
+
+    def set(self, value: object) -> None:
+        """Assign or overwrite a component, automatically deriving the key."""
+        key = getattr(value, "_TCOD_BASE_COMPONENT", value.__class__)
+        self[key] = value
+
+    @staticmethod
+    def __assert_key(key: _ComponentKey[Any]) -> bool:
+        """Verify that abstract classes are accessed correctly."""
+        if isinstance(key, tuple):
+            key = key[1]
+        assert (
+            getattr(key, "_TCOD_BASE_COMPONENT", key) is key
+        ), "Abstract components must be accessed via the base class."
+        return True
+
+    def __getitem__(self, key: _ComponentKey[T]) -> T:
+        """Return a component belonging to this entity."""
+        assert self.__assert_key(key)
+        return self.entity.world._components_by_type[key][self.entity]  # type: ignore[no-any-return]
+
+    def __setitem__(self, key: _ComponentKey[T], value: T) -> None:
+        """Assign a component to an entity."""
+        assert self.__assert_key(key)
+        self.entity.world._components_by_type[key][self.entity] = value
+        self.entity.world._components_by_entity[self.entity].add(key)
+
+    def __delitem__(self, key: type[object] | tuple[object, type[object]]) -> None:
+        """Delete a component from an entity."""
+        assert self.__assert_key(key)
+
+        del self.entity.world._components_by_type[key][self.entity]
+        if not self.entity.world._components_by_type[key]:
+            del self.entity.world._components_by_type[key]
+
+        self.entity.world._components_by_entity[self.entity].remove(key)
+        if not self.entity.world._components_by_entity[self.entity]:
+            del self.entity.world._components_by_entity[self.entity]
+
+    def __contains__(self, key: _ComponentKey[object]) -> bool:  # type: ignore[override]
+        """Return True if this entity has the provided component."""
+        return key in self.entity.world._components_by_entity.get(self.entity, ())
+
+    def __iter__(self) -> Iterator[_ComponentKey[Any]]:
+        """Iterate over the component types belonging to this entity."""
+        return iter(self.entity.world._components_by_entity.get(self.entity, ()))
+
+    def __len__(self) -> int:
+        """Return the number of components belonging to this entity."""
+        return len(self.entity.world._components_by_entity.get(self.entity, ()))
+
+    def update_values(self, values: Iterable[object]) -> None:
+        """Add or overwrite multiple components inplace, deriving the keys from the values."""
+        for value in values:
+            self.set(value)
+
+    if TYPE_CHECKING:  # Type-hinted overrides
+
+        @overload
+        def get(self, __key: _ComponentKey[T]) -> T | None:
+            ...
+
+        @overload
+        def get(self, __key: _ComponentKey[T], __default: T) -> T:
+            ...
+
+        def get(self, __key: _ComponentKey[T], __default: T | None = None) -> T | None:
+            """Return a component, returns None or a default value when the component is missing."""
+
+        def setdefault(self, __key: _ComponentKey[T], __default: T) -> T:  # type: ignore[override]
+            """Assign a default value if a component is missing, then returns the current value."""
+
+
+class EntityTags(MutableSet[Any]):
+    """A proxy attribute to access an entities tags like a set.
+
+    See :any:`Entity.tags`.
+    """
+
+    __slots__ = ("entity",)
+
+    def __init__(self, entity: Entity) -> None:
+        """Initialize this attribute for the given entity."""
+        self.entity: Final = entity
+
+    def add(self, tag: object) -> None:
+        """Add a tag to the entity."""
+        self.entity.world._tags_by_entity[self.entity].add(tag)
+        self.entity.world._tags_by_key[tag].add(self.entity)
+
+    def discard(self, tag: object) -> None:
+        """Discard a tag from an entity."""
+        self.entity.world._tags_by_entity[self.entity].discard(tag)
+        if not self.entity.world._tags_by_entity[self.entity]:
+            del self.entity.world._tags_by_entity[self.entity]
+
+        self.entity.world._tags_by_key[tag].discard(self.entity)
+        if not self.entity.world._tags_by_key[tag]:
+            del self.entity.world._tags_by_key[tag]
+
+    def __contains__(self, x: object) -> bool:
+        """Return True if this entity has the given tag."""
+        return x in self.entity.world._tags_by_entity.get(self.entity, ())
+
+    def __iter__(self) -> Iterator[Any]:
+        """Iterate over this entities tags."""
+        return iter(self.entity.world._tags_by_entity.get(self.entity, ()))
+
+    def __len__(self) -> int:
+        """Return the number of tags this entity has."""
+        return len(self.entity.world._tags_by_entity.get(self.entity, ()))
+
+
+class EntityRelationsMapping(MutableSet[Entity]):
+    """A proxy attribute to access entity relation targets like a set.
+
+    See :any:`Entity.relation_tags_many`.
+    """
+
+    __slots__ = ("entity", "key")
+
+    def __init__(self, entity: Entity, key: object) -> None:
+        """Initialize this attribute for the given entity."""
+        self.entity: Final = entity
+        self.key: Final = key
+        assert key not in {None, Ellipsis}
+
+    def add(self, target: Entity) -> None:
+        """Add a relation target to this tag."""
+        world = self.entity.world
+        world._relation_tags_by_entity[self.entity][self.key].add(target)
+
+        world._relations_lookup[(self.key, target)].add(self.entity)
+        world._relations_lookup[(self.key, ...)].add(self.entity)
+        world._relations_lookup[(self.entity, self.key, None)].add(target)
+        world._relations_lookup[(..., self.key, None)].add(target)
+
+    def discard(self, target: Entity) -> None:
+        """Discard a relation target from this tag."""
+        world = self.entity.world
+
+        world._relation_tags_by_entity[self.entity][self.key].discard(target)
+        if not world._relation_tags_by_entity[self.entity][self.key]:
+            del world._relation_tags_by_entity[self.entity][self.key]
+            if not world._relation_tags_by_entity[self.entity]:
+                del world._relation_tags_by_entity[self.entity]
+
+        world._relations_lookup[(self.key, target)].discard(self.entity)
+        if not world._relations_lookup[(self.key, target)]:
+            del world._relations_lookup[(self.key, target)]
+
+        world._relations_lookup[(self.key, ...)].discard(self.entity)
+        if not world._relations_lookup[(self.key, ...)]:
+            del world._relations_lookup[(self.key, ...)]
+
+        world._relations_lookup[(self.entity, self.key, None)].discard(target)
+        if not world._relations_lookup[(self.entity, self.key, None)]:
+            del world._relations_lookup[(self.entity, self.key, None)]
+
+        world._relations_lookup[(..., self.key, None)].discard(target)
+        if not world._relations_lookup[(..., self.key, None)]:
+            del world._relations_lookup[(..., self.key, None)]
+
+    def __contains__(self, target: Entity) -> bool:  # type: ignore[override]
+        """Return True if this relation contains the given value."""
+        return bool(self.entity.world._relations_lookup.get((self.key, target), ()))
+
+    def __iter__(self) -> Iterator[Entity]:
+        """Iterate over this relation tags targets."""
+        by_entity = self.entity.world._relation_tags_by_entity.get(self.entity)
+        return iter(by_entity.get(self.key, ())) if by_entity is not None else iter(())
+
+    def __len__(self) -> int:
+        """Return the number of targets for this relation tag."""
+        by_entity = self.entity.world._relation_tags_by_entity.get(self.entity)
+        return len(by_entity.get(self.key, ())) if by_entity is not None else 0
+
+
+class EntityRelations(MutableMapping[object, EntityRelationsMapping]):
+    """A proxy attribute to access entity relations like a dict of sets.
+
+    See :any:`Entity.relation_tags_many`.
+    """
+
+    __slots__ = ("entity",)
+
+    def __init__(self, entity: Entity) -> None:
+        """Initialize this attribute for the given entity."""
+        self.entity: Final = entity
+
+    def __getitem__(self, key: object) -> EntityRelationsMapping:
+        """Return the relation mapping for a tag."""
+        return EntityRelationsMapping(self.entity, key)
+
+    def __setitem__(self, key: object, values: Iterable[Entity]) -> None:
+        """Overwrite the targets of a relation tag with the new values."""
+        assert not isinstance(values, Entity), "Did you mean `entity.relations[key] = (target,)`?"
+        mapping = EntityRelationsMapping(self.entity, key)
+        mapping.clear()
+        for v in values:
+            mapping.add(v)
+
+    def __delitem__(self, key: object) -> None:
+        """Clear the relation tags of an entity.
+
+        This does not remove relation tags towards this entity.
+        """
+        self[key].clear()
+
+    def __iter__(self) -> Iterator[Any]:
+        """Iterate over the unique relation tags of this entity."""
+        return iter(self.entity.world._relation_tags_by_entity.get(self.entity, {}).keys())
+
+    def __len__(self) -> int:
+        """Return the number of unique relation tags this entity has."""
+        return len(self.entity.world._relation_tags_by_entity.get(self.entity, {}))
+
+
+class EntityRelationsExclusive(MutableMapping[object, Entity]):
+    """A proxy attribute to access entity relations exclusively.
+
+    See :any:`Entity.relation_tags`.
+    """
+
+    __slots__ = ("entity",)
+
+    def __init__(self, entity: Entity) -> None:
+        """Initialize this attribute for the given entity."""
+        self.entity: Final = entity
+
+    def __getitem__(self, key: object) -> Entity:
+        """Return the relation target for a key.
+
+        If the relation has no target then raises KeyError.
+        If the relation is not exclusive then raises ValueError.
+        """
+        values = tuple(EntityRelationsMapping(self.entity, key))
+        if not values:
+            raise KeyError(key)
+        try:
+            (target,) = values
+        except ValueError:
+            msg = "Entity relation has multiple targets but an exclusive value was expected."
+            raise ValueError(msg) from None
+        return target
+
+    def __setitem__(self, key: object, target: Entity) -> None:
+        """Set a relation exclusively to a new target."""
+        mapping = EntityRelationsMapping(self.entity, key)
+        mapping.clear()
+        mapping.add(target)
+
+    def __delitem__(self, key: object) -> None:
+        """Clear the relation targets of a relation key."""
+        EntityRelationsMapping(self.entity, key).clear()
+
+    def __iter__(self) -> Iterator[Any]:
+        """Iterate over the keys of this entities relations."""
+        return EntityRelations(self.entity).__iter__()
+
+    def __len__(self) -> int:
+        """Return the number of relations this entity has."""
+        return EntityRelations(self.entity).__len__()
+
+
+class EntityComponentRelationMapping(Generic[T], MutableMapping[Entity, T]):
+    """An entity-component mapping to access the relation target component objects.
+
+    See :any:`Entity.relation_components`.
+    """
+
+    __slots__ = ("entity", "key")
+
+    def __init__(self, entity: Entity, key: _ComponentKey[T]) -> None:
+        """Initialize this attribute for the given entity."""
+        assert isinstance(entity, Entity), entity
+        self.entity: Final = entity
+        self.key: _ComponentKey[T] = key
+
+    def __getitem__(self, target: Entity) -> T:
+        """Return the component related to a target entity."""
+        return self.entity.world._relation_components_by_entity[self.entity][self.key][target]  # type: ignore[no-any-return]
+
+    def __setitem__(self, target: Entity, component: T) -> None:
+        """Assign a component to the target entity."""
+        world = self.entity.world
+        if target in world._relation_components_by_entity[self.entity][self.key] is not None:
+            del self[target]
+        world._relation_components_by_entity[self.entity][self.key][target] = component
+
+        world._relations_lookup[(self.key, target)] = {self.entity}
+        world._relations_lookup[(self.key, ...)].add(self.entity)
+        world._relations_lookup[(self.entity, self.key, None)] = {target}
+        world._relations_lookup[(..., self.key, None)].add(target)
+
+    def __delitem__(self, target: Entity) -> None:
+        """Delete a component assigned to the target entity."""
+        world = self.entity.world
+        del world._relation_components_by_entity[self.entity][self.key][target]
+        if not world._relation_components_by_entity[self.entity][self.key]:
+            del world._relation_components_by_entity[self.entity][self.key]
+        if not world._relation_components_by_entity[self.entity]:
+            del world._relation_components_by_entity[self.entity]
+
+        world._relations_lookup[(self.key, target)].discard(self.entity)
+        if not world._relations_lookup[(self.key, target)]:
+            del world._relations_lookup[(self.key, target)]
+
+        world._relations_lookup[(self.key, ...)].discard(self.entity)
+        if not world._relations_lookup[(self.key, ...)]:
+            del world._relations_lookup[(self.key, ...)]
+
+        world._relations_lookup[(self.entity, self.key, None)].discard(self.entity)
+        if not world._relations_lookup[(self.entity, self.key, None)]:
+            del world._relations_lookup[(self.entity, self.key, None)]
+
+        world._relations_lookup[(..., self.key, None)].discard(self.entity)
+        if not world._relations_lookup[(..., self.key, None)]:
+            del world._relations_lookup[(..., self.key, None)]
+
+    def __iter__(self) -> Iterator[Entity]:
+        """Iterate over the targets with assigned components."""
+        by_entity = self.entity.world._relation_components_by_entity.get(self.entity)
+        return iter(()) if by_entity is None else iter(by_entity.get(self.key, ()))
+
+    def __len__(self) -> int:
+        """Return the count of targets for this component relation."""
+        by_entity = self.entity.world._relation_components_by_entity.get(self.entity)
+        return 0 if by_entity is None else len(by_entity.get(self.key, ()))
+
+
+class EntityComponentRelations:
+    """Proxy to access the component relations of an entity.
+
+    See :any:`Entity.relation_components`.
+    """
+
+    __slots__ = ("entity",)
+
+    def __init__(self, entity: Entity) -> None:
+        """Initialize this attribute for the given entity."""
+        assert isinstance(entity, Entity), entity
+        self.entity: Final = entity
+
+    def __getitem__(self, key: _ComponentKey[T]) -> EntityComponentRelationMapping[T]:
+        """Access relations for this component key as a `{target: component}` dict-like object."""
+        return EntityComponentRelationMapping(self.entity, key)
+
+    def __delitem__(self, key: _ComponentKey[object]) -> None:
+        """Remove all relations associated with this component key."""
+        EntityComponentRelationMapping(self.entity, key).clear()
+
+
+class World:
+    """A container for entities and components."""
+
+    def __init__(self) -> None:
+        """Initialize a new world."""
+        self._components_by_type: defaultdict[_ComponentKey[object], dict[Entity, Any]] = defaultdict(dict)
+        """Query table entity components.
+
+        dict[ComponentKey][Entity] = component_instance
+        """
+        self._components_by_entity: defaultdict[Entity, set[_ComponentKey[object]]] = defaultdict(set)
+        """Random access entity components.
+
+        dict[Entity] = {component_keys_owned_by_entity}
+        """
+
+        self._tags_by_key: defaultdict[object, set[Entity]] = defaultdict(set)
+        """Query table entity tags.
+
+        dict[tag] = {all_entities_with_tag}
+        """
+        self._tags_by_entity: defaultdict[Entity, set[Any]] = defaultdict(set)
+        """Random access entity tags.
+
+        dict[Entity] = {all_tags_for_entity}
+        """
+
+        self._relation_tags_by_entity: defaultdict[Entity, defaultdict[object, set[Entity]]] = defaultdict(
+            partial(defaultdict, set)  # type: ignore[arg-type]
+        )
+        """Random access tag multi-relations.
+
+        dict[entity][tag] = {target_entities}
+        """
+        self._relation_components_by_entity: defaultdict[
+            Entity, defaultdict[_ComponentKey[object], dict[Entity, Any]]
+        ] = defaultdict(
+            partial(defaultdict, dict)  # type: ignore[arg-type]
+        )
+        """Random access relations owning components.
+
+        dict[entity][ComponentKey][target_entity] = component
+        """
+        self._relations_lookup: defaultdict[
+            tuple[Any, Entity | EllipsisType] | tuple[Entity | EllipsisType, Any, None], set[Entity]
+        ] = defaultdict(set)
+        """Relations query table.  Tags and components are mixed together.
+
+        Tag:
+            dict[(tag, this_entity)] = {target_entities_for_entity}
+            dict[(tag, None)] = {target_entities_for_tag}
+            dict[(target_entity, tag, None)] = {origin_entities_for_target}
+            dict[(None, tag, None)] = {all_origen_entities_for_tag}
+        Component:
+            dict[(ComponentKey, target_entity)] = {origin_entities}
+            dict[(ComponentKey, None)] = {all_origin_entities}
+            dict[(origin_entity, ComponentKey, None)] = {target_entities}
+            dict[(None, ComponentKey, None)] = {all_target_entities}
+        """
+
+        self._names_by_name: dict[object, Entity] = {}
+        """Name query table.
+
+        dict[name] = named_entity
+        """
+        self._names_by_entity: dict[Entity, object] = {}
+        """Name lookup table.
+
+        dict[Entity] = entities_name
+        """
+
+    @property
+    def global_(self) -> Entity:
+        """A unique globally accessible entity.
+
+        This can be used to store globally accessible components in the world itself without any extra boilerplate.
+        Otherwise this entity is not special and will show up with other entities in queries, etc.
+
+        This entity has a `uid` of `None` and may be accessed that way.
+        This syntax my be better for globals in general since it can use any hashable object.
+
+        .. versionadded:: 1.1
+
+        Example::
+
+            >>> world.global_.components[("turn", int)] = 0
+            >>> world[None].components[("turn", int)]  # Alternative syntax
+            0
+        """
+        return Entity(self, None)
+
+    def __setstate__(self, state: dict[str, Any]) -> None:
+        """Unpickle this object and handle state migration."""
+        # Migrate from version <=1.0.0.
+        if "_relation_components" in state:
+            _relation_components: dict[_ComponentKey[object], dict[Entity, dict[Entity, Any]]] = state.pop(
+                "_relation_components"
+            )
+            self._relation_components_by_entity = defaultdict(partial(defaultdict, dict))  # type: ignore[arg-type]
+            for component_key, component_key_relations in _relation_components.items():
+                for entity, entities_component_table in component_key_relations.items():
+                    for target_entity, target_component in entities_component_table.items():
+                        self._relation_components_by_entity[entity][component_key][target_entity] = target_component
+
+            _relations_by_key: dict[object, dict[Entity, set[Entity]]] = state.pop("_relations_by_key")
+            self._relation_tags_by_entity = defaultdict(partial(defaultdict, set))  # type: ignore[arg-type]
+            for tag, tag_relations in _relations_by_key.items():
+                for entity, targets in tag_relations.items():
+                    self._relation_tags_by_entity[entity][tag] = targets
+
+        state.pop("global_", None)  # Migrate from version <=1.2.0.
+
+        self.__dict__.update(state)
+
+    def __getitem__(self, uid: object) -> Entity:
+        """Return an entity associated with a unique id.
+
+        Example::
+
+            >>> world = World()
+            >>> foo = world["foo"]  # Referencing a new entity returns a new empty entity
+            >>> foo is world["foo"]
+            True
+            >>> entity = world.new_entity()
+            >>> world[entity.uid] is entity  # Anonymous entities can be referred to by their uid
+            True
+        """
+        assert uid is not object, "This is reserved."
+        return Entity(self, uid)
+
+    @property
+    def named(self) -> Mapping[object, Entity]:
+        """A view into this worlds named entities.
+
+        Example::
+
+            >>> entity = world.new_entity(name="MyEntity")  # Name is optional and can be any hashable, not just str.
+            >>> entity
+            <Entity name='MyEntity'>
+            >>> entity.world is world  # Worlds can always be accessed from their entity.
+            True
+            >>> world.named["MyEntity"]  # Named entities can be accessed with `World.named`.
+            <Entity name='MyEntity'>
+            >>> world.named.get("Missing") is None  # `World.named` acts like a dictionary, including assignment and `.get()`.
+            True
+        """
+        return self._names_by_name
+
+    def new_entity(
+        self,
+        components: Iterable[object] = (),
+        *,
+        name: object = None,
+        tags: Iterable[Any] = (),
+    ) -> Entity:
+        """Create and return a new entity."""
+        entity = Entity(self)
+        entity.components.update_values(components)
+        entity_tags = entity.tags
+        for tag in tags:
+            entity_tags.add(tag)
+        entity.name = name
+        return entity
+
+    @property
+    def Q(self) -> Query:
+        """Start a new Query for this world.
+
+        Alias for ``tcod.ecs.Query(world)``.
+        """
+        return Query(self)
+
+
+class Query:
+    """Collect a set of entities with the provided conditions."""
+
+    def __init__(self, world: World) -> None:
+        """Initialize a Query."""
+        self.world: Final = world
+
+        self._all_of_components: set[_ComponentKey[object]] = set()
+        self._none_of_components: set[_ComponentKey[object]] = set()
+        self._all_of_tags: set[object] = set()
+        self._none_of_tags: set[object] = set()
+        self._all_of_relations: set[tuple[Any, Entity | EllipsisType] | tuple[Entity | EllipsisType, Any, None]] = set()
+        self._none_of_relations: set[
+            tuple[Any, Entity | EllipsisType] | tuple[Entity | EllipsisType, Any, None]
+        ] = set()
+
+    def __iter_requires(self, extra_components: AbstractSet[_ComponentKey[object]]) -> Iterator[AbstractSet[Entity]]:
+        collect_components = self._all_of_components | extra_components
+        for component in collect_components:
+            yield self.world._components_by_type.get(component, {}).keys()
+        for tag in self._all_of_tags:
+            yield self.world._tags_by_key.get(tag, set())
+        for relation in self._all_of_relations:
+            yield self.world._relations_lookup.get(relation, set())
+
+    def __iter_excludes(self) -> Iterator[AbstractSet[Entity]]:
+        for component in self._none_of_components:
+            yield self.world._components_by_type.get(component, {}).keys()
+        for tag in self._none_of_tags:
+            yield self.world._tags_by_key.get(tag, set())
+        for relation in self._none_of_relations:
+            yield self.world._relations_lookup.get(relation, set())
+
+    def _get_entities(self, extra_components: AbstractSet[_ComponentKey[object]] = frozenset()) -> set[Entity]:
+        # Place the smallest sets first to speed up intersections.
+        requires = sorted(self.__iter_requires(extra_components), key=len)
+        excludes = list(self.__iter_excludes())
+
+        if not requires:
+            if excludes:
+                msg = "A Query can not function only excluding entities."
+            else:
+                msg = "This Query did not include any entities."
+            raise AssertionError(msg)
+
+        entities = set(requires[0])
+        for require in requires[1:]:
+            entities.intersection_update(require)
+        for exclude in excludes:
+            entities.difference_update(exclude)
+        return entities
+
+    def all_of(
+        self,
+        components: Iterable[_ComponentKey[object]] = (),
+        *,
+        tags: Iterable[object] = (),
+        relations: Iterable[tuple[object, Entity | EllipsisType] | tuple[Entity | EllipsisType, Any, None]] = (),
+    ) -> Self:
+        """Filter entities based on having all of the provided elements."""
+        self._all_of_components.update(components)
+        self._all_of_tags.update(tags)
+        self._all_of_relations.update(relations)
+        return self
+
+    def none_of(
+        self,
+        components: Iterable[_ComponentKey[object]] = (),
+        *,
+        tags: Iterable[object] = (),
+        relations: Iterable[tuple[object, Entity | EllipsisType] | tuple[Entity | EllipsisType, Any, None]] = (),
+    ) -> Self:
+        """Filter entities based on having none of the provided elements."""
+        self._none_of_components.update(components)
+        self._none_of_tags.update(tags)
+        self._none_of_relations.update(relations)
+        return self
+
+    def __iter__(self) -> Iterator[Entity]:
+        """Iterate over the matching entities."""
+        return iter(self._get_entities())
+
+    @overload
+    def __getitem__(self, key: tuple[_ComponentKey[_T1]]) -> Iterable[tuple[_T1]]:
+        ...
+
+    @overload
+    def __getitem__(self, key: tuple[_ComponentKey[_T1], _ComponentKey[_T2]]) -> Iterable[tuple[_T1, _T2]]:
+        ...
+
+    @overload
+    def __getitem__(
+        self, key: tuple[_ComponentKey[_T1], _ComponentKey[_T2], _ComponentKey[_T3]]
+    ) -> Iterable[tuple[_T1, _T2, _T3]]:
+        ...
+
+    @overload
+    def __getitem__(
+        self, key: tuple[_ComponentKey[_T1], _ComponentKey[_T2], _ComponentKey[_T3], _ComponentKey[_T4]]
+    ) -> Iterable[tuple[_T1, _T2, _T3, _T4]]:
+        ...
+
+    @overload
+    def __getitem__(
+        self,
+        key: tuple[_ComponentKey[_T1], _ComponentKey[_T2], _ComponentKey[_T3], _ComponentKey[_T4], _ComponentKey[_T5]],
+    ) -> Iterable[tuple[_T1, _T2, _T3, _T4, _T5]]:
+        ...
+
+    @overload
+    def __getitem__(self, key: tuple[_ComponentKey[object], ...]) -> Iterable[tuple[Any, ...]]:
+        ...
+
+    def __getitem__(self, key: tuple[_ComponentKey[object], ...]) -> Iterable[tuple[Any, ...]]:
+        """Collect components from a query."""
+        assert key is not None
+        assert isinstance(key, tuple)
+
+        entities = list(self._get_entities(set(key) - {Entity}))
+        entity_components = []
+        for component_key in key:
+            if component_key is Entity:
+                entity_components.append(entities)
+                continue
+            world_components = self.world._components_by_type[component_key]
+            entity_components.append([world_components[entity] for entity in entities])
+        return zip(*entity_components)
```

### Comparing `tcod-ecs-1.2.0/PKG-INFO` & `tcod_ecs-2.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tcod-ecs
-Version: 1.2.0
+Version: 2.0.0
 Summary: A type-hinted Entity Component System based on Python dictionaries and sets.
 Author-email: Kyle Benesch <4b796c65+github@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -64,32 +64,39 @@
 >>> import tcod.ecs
 >>> world = tcod.ecs.World()  # New empty world.
 
 ```
 
 ## Entity
 
-New entities can be created with `World.new_entity`.
+Each Entity is identified by its unique id (`uid`) which can be any hashable object and the `world` it belongs to.
+New unique entities can be created with `World.new_entity` which uses a new `object()` as the `uid`.
 An entity always knows about its assigned world.
 Worlds only know about their entities once the entity is assigned a name, component, tag, or relation.
-An entity is identified by its "Python identity" rather than with a low-level stand-in identifier.
 
 ```py
->>> entity = world.new_entity(name="MyEntity")  # Name is optional and can be any hashable, not just str.
+>>> entity = world.new_entity()  # Creates a unique entity using `object()` as the uid
 >>> entity
-<Entity name='MyEntity'>
->>> entity.world is world  # Worlds can always be accessed from their entity.
+<Entity(uid=object at ...)>
+>>> entity.world is world  # Worlds can always be accessed from their entity
 True
->>> world.named["MyEntity"]  # Named entities can be accessed with `World.named`.
-<Entity name='MyEntity'>
->>> world.named.get("Missing") is None  # `World.named` acts like a dictionary, including assignment and `.get()`.
+>>> world[entity.uid] is entity  # Entities with the same world/uid are compared using `is`
+True
+
+# Reference an entity with the given uid, can be any hashable object:
+>>> entity = world["MyEntity"]
+>>> entity
+<Entity(uid='MyEntity')>
+>>> world["MyEntity"] is entity
 True
 
 ```
 
+Use `World.new_entity` to create unique entities and use `World[x]` to reference a global entity or relation with an id.
+
 ## Serialization
 
 Worlds are normal Python objects and can be pickled as long as all stored components can be pickled.
 
 ```py
 >>> import pickle
 >>> pickled_data: bytes = pickle.dumps(world)
@@ -112,15 +119,15 @@
 42
 >>> int in entity.components
 True
 >>> del entity.components[int]
 >>> entity.components[int]  # Missing keys raise KeyError
 Traceback (most recent call last):
   ...
-KeyError: <Entity ...>
+KeyError: <Entity...>
 >>> entity.components.get(int, "default")  # Test keys with `.get()` like a dictionary.
 'default'
 >>> @attrs.define
 ... class Vector2:
 ...     x: int = 0
 ...     y: int = 0
 >>> entity.components[Vector2] = Vector2(1, 2)
@@ -146,15 +153,15 @@
 ...     print((pos, i))
 (Vector2(x=10, y=0), 11)
 
 # You can include `Entity` to iterate over entities with their components.
 # This always iterates over the entity itself instead of an Entity component.
 >>> for e, pos, i in world.Q[tcod.ecs.Entity, Vector2, int]:
 ...     print((e, pos, i))
-(<Entity ...>, Vector2(x=10, y=0), 11)
+(<Entity...>, Vector2(x=10, y=0), 11)
 
 ```
 
 ## Named Components
 
 Only one component can be assigned unless that component is given a unique name.
 You can name components with the key syntax `(name, type)` when assigning components.
```

