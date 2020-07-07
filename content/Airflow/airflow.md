# Airflow

workflow orchestration, also able to monitoring them

use for repetitive tasks, don't change on daily basis, good for ETL job orchestration, trigger Spark

## How to use 
Concepts you need to know for sure:
- Scheduler / Executor
    - DAG: start_date / shedule_interval
    - Task Create → Queue
        - sequential: one by one, for debug and testing
        - local: concurrent, vertically, single point failure
        - celery: dispatch to woker, recommend: maintain infrastructure
        - kubernetes:L: allow run task using kubernetes - elastic to workload, avoid wasting resources
- Webserver: UI dashboard
    - DAGs View / DAG View /  Tree Biew / Task Dualation / Gantt View / Code View
    
- DAGs:
    - start_data/dag_id/schedule_interval/max_active_runs/catch_up

- Plugin:
- Operator / Hooks / sensors:
    - operator: excute work as a step in a workflow; sensor, when a creatia is met
    - hook: interface to external platforms and services, sensor, special type of operator, monitering events poke function
- XCom: cross-communication between tasks and operators to exchange info
    - push / pull to a database
- variables: key vaule store in airflow, query from database


## Resources 
- Everyone has to start somewhere, provide a short blurb for ANY turorials you found helpful, link to the tutorial, and any connected Codebases. 
- Youtube videos, Important documentation, etc.
- Please don't include out of date / bad resources.  This should be a best of list with

Example:
- [Some really awesome tutorial](https://towardsdatascience.com/getting-started-with-apache-airflow-df1aa77d7b1b)
    - This tutorial is about XYZ...


## Pain Points 
The worst part of Airflow
Example:
- **Something painful about this topic**
This is really annoying when it happens.  The reason for it is people need to write better code.  In order to get around it, write better code.



