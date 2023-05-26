# Comparing `tmp/pyjej-0.1.6.tar.gz` & `tmp/pyjej-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjej-0.1.6.tar", max compression
+gzip compressed data, was "pyjej-0.1.7.tar", max compression
```

## Comparing `pyjej-0.1.6.tar` & `pyjej-0.1.7.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     9522 2023-05-25 11:06:33.644668 pyjej-0.1.6/README.md
--rw-r--r--   0        0        0      171 2023-05-24 19:43:16.382536 pyjej-0.1.6/pyjej/__main__.py
--rw-r--r--   0        0        0     1956 2023-05-24 19:19:54.926640 pyjej-0.1.6/pyjej/selflib.py
--rw-r--r--   0        0        0     3701 2023-05-25 11:12:00.060233 pyjej-0.1.6/pyjej/tasks.py
--rw-r--r--   0        0        0      400 2023-05-25 11:13:50.644074 pyjej-0.1.6/pyproject.toml
--rw-r--r--   0        0        0    10153 1970-01-01 00:00:00.000000 pyjej-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0    10796 2023-05-26 15:26:43.521571 pyjej-0.1.7/README.md
+-rw-r--r--   0        0        0      171 2023-05-24 19:43:16.382536 pyjej-0.1.7/pyjej/__main__.py
+-rw-r--r--   0        0        0      142 2023-05-26 14:31:45.812687 pyjej-0.1.7/pyjej/groovy/export_plugins.txt
+-rw-r--r--   0        0        0     1956 2023-05-24 19:19:54.926640 pyjej-0.1.7/pyjej/selflib.py
+-rw-r--r--   0        0        0     4213 2023-05-26 14:45:01.866921 pyjej-0.1.7/pyjej/tasks.py
+-rw-r--r--   0        0        0      400 2023-05-26 14:49:43.698251 pyjej-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0    11427 1970-01-01 00:00:00.000000 pyjej-0.1.7/PKG-INFO
```

### Comparing `pyjej-0.1.6/README.md` & `pyjej-0.1.7/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -32,35 +32,41 @@
     ```
     python -m pyjej job.export-all -s мой_сервер_jenkins
     ```
 
 1.  Создание задания на сервере Jenkins из XML файла:
 
     ```
-    python -m pyjej job.create -s мой_сервер_jenkins -j моё_задание -i входная_папка
+    python -m pyjej job.create -s мой_сервер_jenkins -j моё_задание -f входная_папка
     ```
 
 1.  Обновление задания на сервере Jenkins из XML файла:
 
     ```
-    python -m pyjej job.update -s мой_сервер_jenkins -j моё_задание -i входная_папка
+    python -m pyjej job.update -s мой_сервер_jenkins -j моё_задание -f входная_папка
     ```
 
-1.  Экспорт всех плагинов:
+1.  Экспорт всех плагинов в файл `plugins.txt`:
 
     ```
     python -m pyjej plugins.export-all -s мой_сервер_jenkins
     ```
 
 1.  Установка указного плагина в Jenkins:
 
     ```
     python -m pyjej plugins.install -s мой_сервер_jenkins -p имя_плагина
     ```
 
+1.  Установить все плагины Jenkins из указного файла `plugins.txt` на указанный сервер:
+
+    ```
+    python -m pyjej plugins.all-install -s my_server -f ./data/komtek/plugins.txt
+    ```
+
 1.  Скачать настройки из плагина Jenkins Configuration as Code:
 
     ```
     python -m pyjej jcasc.export -s мой_сервер_jenkins
     ```
 
 Убедитесь, что заменяете `мой_сервер_jenkins` на фактическое имя сервера, определенное в файле `inventory.yml`, `моё_задание` на желаемое имя задания и `входная_папка` на папку, содержащую файл XML для задания.
@@ -99,29 +105,29 @@
 #### Задача `job.create`
 
 Эта задача создает конкретное задание на сервере Jenkins с использованием файла XML.
 
 **Использование:**
 
 ```shell
-python -m pyjej job.create --server <имя_сервера> --jobname <имя_задания> --in_server <входная_папка>
+python -m pyjej job.create --server <имя_сервера> --jobname <имя_задания> --from_server <входная_папка>
 ```
 
 -   `<имя_сервера>`: Имя сервера Jenkins, определенное в файле `inventory.yml`.
 -   `<имя_задания>`: Имя задания для создания.
 -   `<входная_папка>`: Папка, содержащая файл XML для задания.
 
 #### Задача `job.update`
 
 Эта задача обновляет конкретное задание на сервере Jenkins с использованием файла XML.
 
 **Использование:**
 
 ```shell
-python -m pyjej job.update --server <имя_сервера> --jobname <имя_задания> --in_server <входная_папка>
+python -m pyjej job.update --server <имя_сервера> --jobname <имя_задания> --from_server <входная_папка>
 ```
 
 -   `<имя_сервера>`: Имя сервера Jenkins, определенное в файле `inventory.yml`.
 -   `<имя_задания>`: Имя задания для обновления.
 -   `<входная_папка>`: Папка, содержащая файл XML для задания.
 
 #### Задача `plugins.export-all`
@@ -149,14 +155,29 @@
 ```
 
 -   `<имя_сервера>`: Имя сервера Jenkins, определенное в файле `inventory.yml`.
 -   `<имя_плагина>`: Имя плагина, который нужно установить.
 
 Результат выполнения команды будет выведен на экран.
 
+#### Задача `plugins.all-install`
+
+Эта задача позволяет установить все плагин на сервере Jenkins из файла `plugins.txt`.
+
+**Использование:**
+
+```shell
+python -m pyjej plugins.all-install --server <имя_сервера> --from_file <путь_к_файлу>
+```
+
+-   `<имя_сервера>`: Имя сервера Jenkins, определенное в файле `inventory.yml` на который установить плагины.
+-   `<имя_плагина>`: Путь к файлу `plugins.txt`
+
+Результат выполнения команды будет выведен на экран.
+
 #### Задача `jcasc.export`
 
 Эта задача позволяет скачать конфигурации Jenkins которые формируются через плагин `Jenkins Configuration as Code (a.k.a. JCasC) Plugin`.
 https://github.com/jenkinsci/configuration-as-code-plugin
 
 **Использование:**
 
@@ -164,15 +185,15 @@
 python -m pyjej jcasc.export --server <имя_сервера>
 ```
 
 -   `<имя_сервера>`: Имя сервера Jenkins, определенное в файле `inventory.yml`.
 
 Результат выполнения команды будет выведен на экран и записан в файл `data/<имя_сервера>/jenkins.yaml`.
 
-# Пример создания файла inventory.yml
+## Пример создания файла inventory.yml
 
 Файл `inventory.yml` используется для настройки подключения к серверам Jenkins в коде. В этой главе мы предоставим пример создания файла `inventory.yml` с фиктивными значениями.
 
 Пример содержимого файла `inventory.yml`:
 
 ```yaml
 my_server:
@@ -192,7 +213,13 @@
 -   `BASE_COMMAND_CLI`: Базовая команда для выполнения операций через командную строку Jenkins CLI.
 
 Убедитесь, что заменяете фиктивные значения реальными данными серверов Jenkins, к которым вы хотите подключиться.
 
 Создайте файл `inventory.yml` в корневой папке проекта и добавьте соответствующую информацию для ваших серверов Jenkins. Этот файл будет использоваться кодом для установления связи с серверами Jenkins.
 
 В следующей главе мы рассмотрим пример использования задач из `tasks.py` для взаимодействия с серверами Jenkins, настроенными в файле `inventory.yml`.
+
+# Восстановление конфигураций Jenkins через плагин `Configuration as Code`
+
+1. Переместить файл `jenkins.yaml` в Jenkins по пути `/var/jenkins_home/`
+1. Перейти на URL: `https://ci.pkzdrav.ru/configuration-as-code/`
+1. Нажать `Apply new configuration`
```

### Comparing `pyjej-0.1.6/pyjej/selflib.py` & `pyjej-0.1.7/pyjej/selflib.py`

 * *Files identical despite different names*

### Comparing `pyjej-0.1.6/pyjej/tasks.py` & `pyjej-0.1.7/pyjej/tasks.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import requests
 from invoke import Runner, Collection, Result, task
 
 from .selflib import getInventory, os_exe_async
 
 
 INVENTORY = getInventory(os.getenv("INVENTORY_FILE"))
+PATH_TO_SCRIPTS = pathlib.Path(__file__).parent / "groovy"
 
 
 def get_base_command_cli(server):
     return INVENTORY[server]["BASE_COMMAND_CLI"].format(**INVENTORY[server])
 
 
 @task
@@ -42,44 +43,58 @@
         f"{get_base_command_cli(server)} get-job {jobname}", hide=True
     )
     if not res.stderr:
         pathlib.Path("data", server, "jobs", f"{jobname}.xml").write_text(res.stdout)
 
 
 @task
-def create_job(ctx: Runner, server: str, jobname: str, in_server: str):
+def create_job(ctx: Runner, server: str, jobname: str, from_server: str):
     """Создать указанную Job на Jenkins"""
     ctx.run(
-        f"{get_base_command_cli(server)} create-job {jobname} < {pathlib.Path('data', in_server,'jobs',f'{jobname}.xml')}",
+        f"{get_base_command_cli(server)} create-job {jobname} < {pathlib.Path('data', from_server,'jobs',f'{jobname}.xml')}",
     )
 
 
 @task
-def update_job(ctx: Runner, server: str, jobname: str, in_server: str):
+def update_job(ctx: Runner, server: str, jobname: str, from_server: str):
     """Обновить указанную Job в Jenkins"""
     ctx.run(
-        f"{get_base_command_cli(server)} update-job {jobname} < {pathlib.Path('data',in_server,'jobs',f'{jobname}.xml')}",
+        f"{get_base_command_cli(server)} update-job {jobname} < {pathlib.Path('data',from_server,'jobs',f'{jobname}.xml')}",
     )
 
 
 @task
 def export_all_plugins(ctx: Runner, server: str):
     """Получить список всех плагинов"""
 
-    res: Result = ctx.run(f"{get_base_command_cli(server)} list-plugins", hide=True)
+    path_to_script = (PATH_TO_SCRIPTS / "export_plugins.txt").resolve()
+
+    res: Result = ctx.run(
+        f"{get_base_command_cli(server)} groovy = < {path_to_script}", hide=False
+    )
+
     if not res.stderr:
         pathlib.Path("data", server, "plugins.txt").write_text(res.stdout)
 
 
 @task
-def install_plugins(ctx: Runner, server: str, plugin: str):
+def install_plugin(ctx: Runner, server: str, plugin: str):
     """Установить указанный плагин"""
     ctx.run(
         f"{get_base_command_cli(server)} install-plugin {plugin}",
     )
+    print(f":> {plugin}")
+
+
+@task
+def install_all_plugin(ctx: Runner, server: str, from_file: str):
+    """Установить все плагины"""
+    for plugin in pathlib.Path(from_file).read_text().split("\n"):
+        if plugin:
+            install_plugin(ctx, server, plugin)
 
 
 @task
 def export_JCasC(ctx: Runner, server: str):
     """Загрузить настройки из плагина 'Jenkins Configuration as Code'"""
     i = INVENTORY[server]
     res: requests.Response = requests.post(
@@ -93,15 +108,16 @@
 job_nsp.add_task(export_all_jobs, "export-all")
 job_nsp.add_task(export_job, "export")
 job_nsp.add_task(create_job, "create")
 job_nsp.add_task(update_job, "update")
 
 plugins_nsp = Collection()
 plugins_nsp.add_task(export_all_plugins, "export-all")
-plugins_nsp.add_task(install_plugins, "install")
+plugins_nsp.add_task(install_plugin, "install")
+plugins_nsp.add_task(install_all_plugin, "all-install")
 
 jcasc_nsp = Collection()
 jcasc_nsp.add_task(export_JCasC, "export")
 
 namespace = Collection()
 namespace.add_collection(job_nsp, "job")
 namespace.add_collection(plugins_nsp, "plugins")
```

### Comparing `pyjej-0.1.6/PKG-INFO` & `pyjej-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjej
-Version: 0.1.6
+Version: 0.1.7
 Summary: Проект для взаимодействия с Jenkins через CLI
 Author: Кустов Денис
 Author-email: kudv@pkzdrav.ru
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -49,35 +49,41 @@
     ```
     python -m pyjej job.export-all -s мой_сервер_jenkins
     ```
 
 1.  Создание задания на сервере Jenkins из XML файла:
 
     ```
-    python -m pyjej job.create -s мой_сервер_jenkins -j моё_задание -i входная_папка
+    python -m pyjej job.create -s мой_сервер_jenkins -j моё_задание -f входная_папка
     ```
 
 1.  Обновление задания на сервере Jenkins из XML файла:
 
     ```
-    python -m pyjej job.update -s мой_сервер_jenkins -j моё_задание -i входная_папка
+    python -m pyjej job.update -s мой_сервер_jenkins -j моё_задание -f входная_папка
     ```
 
-1.  Экспорт всех плагинов:
+1.  Экспорт всех плагинов в файл `plugins.txt`:
 
     ```
     python -m pyjej plugins.export-all -s мой_сервер_jenkins
     ```
 
 1.  Установка указного плагина в Jenkins:
 
     ```
     python -m pyjej plugins.install -s мой_сервер_jenkins -p имя_плагина
     ```
 
+1.  Установить все плагины Jenkins из указного файла `plugins.txt` на указанный сервер:
+
+    ```
+    python -m pyjej plugins.all-install -s my_server -f ./data/komtek/plugins.txt
+    ```
+
 1.  Скачать настройки из плагина Jenkins Configuration as Code:
 
     ```
     python -m pyjej jcasc.export -s мой_сервер_jenkins
     ```
 
 Убедитесь, что заменяете `мой_сервер_jenkins` на фактическое имя сервера, определенное в файле `inventory.yml`, `моё_задание` на желаемое имя задания и `входная_папка` на папку, содержащую файл XML для задания.
@@ -116,29 +122,29 @@
 #### Задача `job.create`
 
 Эта задача создает конкретное задание на сервере Jenkins с использованием файла XML.
 
 **Использование:**
 
 ```shell
-python -m pyjej job.create --server <имя_сервера> --jobname <имя_задания> --in_server <входная_папка>
+python -m pyjej job.create --server <имя_сервера> --jobname <имя_задания> --from_server <входная_папка>
 ```
 
 -   `<имя_сервера>`: Имя сервера Jenkins, определенное в файле `inventory.yml`.
 -   `<имя_задания>`: Имя задания для создания.
 -   `<входная_папка>`: Папка, содержащая файл XML для задания.
 
 #### Задача `job.update`
 
 Эта задача обновляет конкретное задание на сервере Jenkins с использованием файла XML.
 
 **Использование:**
 
 ```shell
-python -m pyjej job.update --server <имя_сервера> --jobname <имя_задания> --in_server <входная_папка>
+python -m pyjej job.update --server <имя_сервера> --jobname <имя_задания> --from_server <входная_папка>
 ```
 
 -   `<имя_сервера>`: Имя сервера Jenkins, определенное в файле `inventory.yml`.
 -   `<имя_задания>`: Имя задания для обновления.
 -   `<входная_папка>`: Папка, содержащая файл XML для задания.
 
 #### Задача `plugins.export-all`
@@ -166,14 +172,29 @@
 ```
 
 -   `<имя_сервера>`: Имя сервера Jenkins, определенное в файле `inventory.yml`.
 -   `<имя_плагина>`: Имя плагина, который нужно установить.
 
 Результат выполнения команды будет выведен на экран.
 
+#### Задача `plugins.all-install`
+
+Эта задача позволяет установить все плагин на сервере Jenkins из файла `plugins.txt`.
+
+**Использование:**
+
+```shell
+python -m pyjej plugins.all-install --server <имя_сервера> --from_file <путь_к_файлу>
+```
+
+-   `<имя_сервера>`: Имя сервера Jenkins, определенное в файле `inventory.yml` на который установить плагины.
+-   `<имя_плагина>`: Путь к файлу `plugins.txt`
+
+Результат выполнения команды будет выведен на экран.
+
 #### Задача `jcasc.export`
 
 Эта задача позволяет скачать конфигурации Jenkins которые формируются через плагин `Jenkins Configuration as Code (a.k.a. JCasC) Plugin`.
 https://github.com/jenkinsci/configuration-as-code-plugin
 
 **Использование:**
 
@@ -181,15 +202,15 @@
 python -m pyjej jcasc.export --server <имя_сервера>
 ```
 
 -   `<имя_сервера>`: Имя сервера Jenkins, определенное в файле `inventory.yml`.
 
 Результат выполнения команды будет выведен на экран и записан в файл `data/<имя_сервера>/jenkins.yaml`.
 
-# Пример создания файла inventory.yml
+## Пример создания файла inventory.yml
 
 Файл `inventory.yml` используется для настройки подключения к серверам Jenkins в коде. В этой главе мы предоставим пример создания файла `inventory.yml` с фиктивными значениями.
 
 Пример содержимого файла `inventory.yml`:
 
 ```yaml
 my_server:
@@ -210,7 +231,13 @@
 
 Убедитесь, что заменяете фиктивные значения реальными данными серверов Jenkins, к которым вы хотите подключиться.
 
 Создайте файл `inventory.yml` в корневой папке проекта и добавьте соответствующую информацию для ваших серверов Jenkins. Этот файл будет использоваться кодом для установления связи с серверами Jenkins.
 
 В следующей главе мы рассмотрим пример использования задач из `tasks.py` для взаимодействия с серверами Jenkins, настроенными в файле `inventory.yml`.
 
+# Восстановление конфигураций Jenkins через плагин `Configuration as Code`
+
+1. Переместить файл `jenkins.yaml` в Jenkins по пути `/var/jenkins_home/`
+1. Перейти на URL: `https://ci.pkzdrav.ru/configuration-as-code/`
+1. Нажать `Apply new configuration`
+
```

