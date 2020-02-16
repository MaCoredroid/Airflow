Airflow

- Apache Airflow (or simply Airflow) is a platform to programmatically author, schedule, and monitor workflows.

  When workflows are defined as code, they become more maintainable, versionable, testable, and collaborative.

  Use Airflow to author workflows as directed acyclic graphs (DAGs) of tasks. The Airflow scheduler executes your tasks on an array of workers while following the specified dependencies. Rich command line utilities make performing complex surgeries on DAGs a snap. The rich user interface makes it easy to visualize pipelines running in production, monitor progress, and troubleshoot issues when needed.

  Airflow是一个以代码定义工作流的工具，可以可视化的显示流程的执行

- Install airflow with `pip install apache-airflow `. It is recommended to install airflow on ubuntu 18.04 or higher.

- Use the following code to get started with example

  ```bash
  # initialize the database
  airflow initdb
  
  # start the web server, default port is 8080
  airflow webserver -p 8080
  
  # start the scheduler
  airflow scheduler
  ```

- Workflows are expected to be mostly static or slowly changing. You can think of the structure of the tasks in your workflow as slightly more dynamic than a database structure would be. Airflow workflows are expected to look similar from a run to the next, this allows for clarity around unit of work and continuity.

  工作流一旦定义后则成为静态的，不会在执行时改变。

- 