# Zeppelin topics:
---
## Configuring zeppelin for spark and pyspark on windows.

### Steps:

* Download zeppelin : https://zeppelin.apache.org/download.html
* Extract the zeppelin on to harddrive.
* Broswe to the folder _**<your_zeppelin_folder>**_\conf\
* Rename the file or copy zeppelin-env.cmd.template to zeppelin-env.cmd
* Open the file zeppelin-env.cmd for a editing.
* Add the following line in the file:
  * <sub><sup>set PYTHONPATH=_**<your_zeppelin_folder>**_\interpreter\spark\pyspark;_**<your_zeppelin_folder>**_\interpreter\spark\python;_**<your_zeppelin_folder>**_\interpreter\python;_**<your_zeppelin_folder>**_\interpreter\python\python;</sup></sub>
  * Save the file.
* Run the zeppelin zepplin.cmd
* Goto http://localhost:8080
* Create new notebook.
* Try the spark paragraph:
  ```
  %spark
  sc.version
  ```
* Try the pysprak paragraph:
  ```
  %pyspark
  sc.version
  ```
* Both paragraphs should run without error and print the spark version. For eg:
  ```
  2.2.0
  ```
---
