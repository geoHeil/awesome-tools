# Data Management

## choice of database

- cloud databases
  - https://towardsdatascience.com/datastore-choices-sql-vs-nosql-database-ebec24d56106 really great overview

## scheduler
- https://www.digdag.io


## permissions
- AWS policy generator https://github.com/salesforce/policy_sentry/blob/master/README.md
## ETL

### methodology

- https://de.wikipedia.org/wiki/Data_Vault

### batch
- https://github.com/volcano-sh/volcano
- excel automation https://www.xlwings.org/
- spark
  - SQL tuning 
    - https://www.youtube.com/watch?v=_Ne27JcLnEc
  - lakehouse spark 3.x & delta: https://www.youtube.com/watch?v=iog5feADeXc
  
- dagster tipps
  - https://github.com/sspaeti-com/awesome-dagster
  
### schema

- dynamic schema https://www.youtube.com/watch?v=No55ImP-Jic

### streaming

#### flink deployments

- k8s operator for blue green deployment
  - https://github.com/lyft/flinkk8soperator

### unit testing
- hive sql unit testing with code coverage https://github.com/HotelsDotCom/mutant-swarm
- pyspark
  - https://medium.com/@gu.martinm/pyspark-unit-integration-and-end-to-end-tests-c2ba71467d85

### native code

- wrapping native code
  - https://github.com/bytedeco/javacpp
  - https://www.youtube.com/watch?v=5GvfPGcdhqI PCAP example

#### spark
- https://github.com/swoop-inc/spark-records
- https://github.com/swoop-inc/spark-alchemy
- framework ETL
  - https://github.com/CoxAutomotiveDataSolutions/waimak
  - https://arc.tripl.ai/
- fine tuning catalyst optimizer
  - https://www.youtube.com/watch?v=IjqC2Y2Hd5k
- streaming optimization
  - https://medium.com/@Iqbalkhattra85/optimize-spark-structured-streaming-for-scale-d5dc5dee0622

### classical DB
- https://pgdash.io/blog/postgres-features.html

### ETL tools
- https://dataform.co/
- https://www.getdbt.com

### ETL in python
- https://github.com/petl-developers/petl
- https://github.com/python-bonobo/bonobo
- https://www.singer.io
- https://meltano.com/ (reference runner for singer)
- https://airbyte.io/

#### unit testing data - validating assumptions

- https://bulwark.readthedocs.io/en/latest/index.html

### orchestration
- Airflow
- prefect
- https://dagster.readthedocs.io

### monitoring
- health dashbboard https://github.com/criteo/slab

## k8s
### failures
- - https://github.com/hjacobs/kubernetes-failure-stories

## load tests
- stress testing https://github.com/open-chaos/experiment-catalog

### unified batch & streaming
- https://www.youtube.com/watch?v=4qSlsYogALo


### hybrid cloud

#### data sync
- NiFi https://medium.com/@abdelkrim.hadjidj/hub-and-spoke-architectures-with-nifi-site-to-site-communications-at-any-level-a-nifi-1-10-a8702f77c66e
