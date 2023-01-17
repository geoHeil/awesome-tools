# Data Management

## environment handling

- https://palm-cli.readthedocs.io/en/latest/introduction/examples.html

## choice of database

- cloud databases
  - https://towardsdatascience.com/datastore-choices-sql-vs-nosql-database-ebec24d56106 really great overview


## storage systems

### blob storage

- https://tech.preferred.jp/en/blog/a-year-with-apache-ozone/

## scheduler
- https://www.digdag.io


## permissions
- AWS policy generator https://github.com/salesforce/policy_sentry/blob/master/README.md
## ETL

### methodology

- https://de.wikipedia.org/wiki/Data_Vault
- metrics layer: https://www.sspaeti.com/blog/analytics-api-with-graphql-the-next-level-of-data-engineering/

### batch
- https://github.com/volcano-sh/volcano
- excel automation https://www.xlwings.org/
- spark
  - SQL tuning 
    - https://www.youtube.com/watch?v=_Ne27JcLnEc
  - lakehouse spark 3.x & delta: https://www.youtube.com/watch?v=iog5feADeXc
  - https://www.onehouse.ai/blog/apache-hudi-vs-delta-lake-vs-apache-iceberg-lakehouse-feature-comparison
  
- dagster tipps
  - https://github.com/sspaeti-com/awesome-dagster
  - https://github.com/sephib/dagster-graph-project
  - https://github.com/slamer59/dagster-mlflow
  - https://github.com/broadinstitute/dagster-utils
  - https://github.com/AntonFriberg/dagster-project-example
  - https://github.com/thedmi/dagster-celery-docker-example
  - https://github.com/kahnwong/dagster-demo
  - https://github.com/VladX09/dagster-celery-docker-bug/tree/non-zero-exit-example with https://github.com/dagster-io/dagster/issues/5008
    - https://github.com/astenuz/dagster-celery-test
  - https://github.com/xyzy-web/dagster-exchangerates
- airflow problems
    -  https://medium.com/bluecore-engineering/were-all-using-airflow-wrong-and-how-to-fix-it-a56f14cb0753


### schema

- dynamic schema https://www.youtube.com/watch?v=No55ImP-Jic

### streaming

- www.gentlydownthe.stream

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


### cachings

- redis tips: 
  -  https://developer.redis.com/howtos/antipatterns/

### ETL tools
- https://dataform.co/
- https://www.getdbt.com

### ETL in python
- https://github.com/petl-developers/petl
- https://github.com/python-bonobo/bonobo
- https://www.singer.io
- https://meltano.com/ (reference runner for singer)
- https://airbyte.io/

#### dbt and governance

- https://github.com/dbt-labs/dbt-project-evaluator
- https://github.com/tobymao/sqlglot
- https://github.com/Montreal-Analytics/dbt-gloss
- https://github.com/offbi/pre-commit-dbt
- team structure https://github.com/dbt-labs/dbt-core/discussions/5244 monorepo or not
- https://blog.montrealanalytics.com/blue-green-deployment-with-dbt-and-snowflake-922f1c658011
- https://www.getdbt.com/analytics-engineering/case-for-elt-workflow/
- https://montrealanalytics.notion.site/Coalesce-Workshop-Guide-6382db82046f41599e9ec39afb035bdb and https://github.com/Montreal-Analytics/poutineshop-public and video of the workshop https://www.youtube.com/watch?v=L6ixHejZX5A&list=PL0QYlrC86xQlj9UDGiEwhXQuSjuSyPJHl&index=42

#### unit testing data - validating assumptions

- https://bulwark.readthedocs.io/en/latest/index.html
-  https://github.com/datafold/data-diff

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

## self service tools

- https://www.gooddata.com/


## api design

- https://martinfowler.com/articles/cant-buy-integration.html



# end user productivity

- https://www.tadviewer.com/

# quality

## consistency

- https://github.com/IvorySQL/IvorySQL
