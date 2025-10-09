# Data Management

## learning

- https://www.reddit.com/r/dataengineering/comments/1491swe/a_mustread_data_engineering_collection/
- stack overview https://motherduck.com/blog/data-engineering-toolkit-essential-tools/
- https://github.com/rewrite-bigdata-in-rust/RBIR


## stack example

- data
 - https://github.com/cnstlungu/portable-data-stack-dagster/tree/main
 - https://github.com/dagster-io/dagster-open-platform
   - https://medium.com/@edsoncezar16/asset-level-concurrency-limits-via-declarative-scheduling-c4da3a875cf4
   - observability in dagster with grafana/prometheus
     - https://metaops.solutions/blog/dagster-monitoring-prometheus-dbt-assets-sql-transformations-part-2
     - https://metaops.solutions/blog/dagster-monitoring-prometheus-system-metrics-custom-assets-part-1

### editor tooling

databases

- https://studio.outerbase.com/

## environment handling

- https://palm-cli.readthedocs.io/en/latest/introduction/examples.html

## choice of database

- cloud databases
  - https://towardsdatascience.com/datastore-choices-sql-vs-nosql-database-ebec24d56106 really great overview
  
- postgres based
  - https://github.com/paradedb/paradedb****


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

### input validation

- https://github.com/JakobGM/patito
- 
### batch
- https://github.com/volcano-sh/volcano
- excel automation https://www.xlwings.org/
- spark
  - SQL tuning 
    - https://www.youtube.com/watch?v=_Ne27JcLnEc
  - lakehouse spark 3.x & delta: https://www.youtube.com/watch?v=iog5feADeXc
  - https://www.onehouse.ai/blog/apache-hudi-vs-delta-lake-vs-apache-iceberg-lakehouse-feature-comparison
  - optimizing delta https://www.youtube.com/watch?v=o2k9PICWdx0
  - auto optimization https://github.com/dataflint/spark
  
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
- examples
  - https://github.com/dagster-io/mdsfest-opensource-mds
 
#### DBT

- dbt-loom with dagster https://github.com/cnolanminich/dbt-loom-example/tree/demo-with-dagster
- https://github.com/borjavb/dbt-iceberg-poc

#### data frames

- https://github.com/xorq-labs/xorq

### schema

- dynamic schema https://www.youtube.com/watch?v=No55ImP-Jic

#### schema changes

- https://github.com/datafold/data-diff

### streaming

- www.gentlydownthe.stream
- https://gazette.readthedocs.io/en/latest/
- https://github.com/drasi-project/drasi-platform

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
- delta merge optimization
  - https://www.youtube.com/watch?v=o2k9PICWdx0&t=50s

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
- iceberg
  - https://github.com/datazip-inc/olake

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

### ingestion

#### convenience

- https://slingdata.io/
- https://airbyte.com/
- https://docs.dagster.io/integrations/embedded-elt
- https://www.prequel.co/

#### big data

- https://inlong.apache.org/
- https://seatunnel.apache.org/

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

# BI

- https://evidence.dev/
- 

- https://github.com/IvorySQL/IvorySQL

## scaling DBT

-  Unlocking model governance and multi-project deployments with dbt-meshify - Coalesce 2023  https://www.youtube.com/watch?v=FAsY0Qx8EyU https://dbt-labs.github.io/dbt-meshify/0.5/
-  datafold demo https://www.youtube.com/watch?v=5Xxm6cYRmFg
-  JSON schema https://www.youtube.com/watch?v=z8y7mvOUFsY https://github.com/GClunies/Reflekt

## web automation

- https://playwright.dev/ (apparently good for scraping)


## modern data startups

- https://localfirstweb.dev/
- https://www.5x.co/
- https://www.propeldata.com/
- https://www.tinybird.co/


## interesting databases

- Postgres
- DuckDB
  - https://www.youtube.com/watch?v=PoHfh6O43uE
- Starrocks
- https://github.com/datafuselabs/databend
- https://cratedb.com/
- https://www.hydra.so/
- https://neon.tech/
- https://github.com/TFMV/featherman
- https://kuzudb.com/

### streaming

- https://github.com/infinyon/fluvio
- https://risingwave.com/
- https://materialize.com/
- https://www.decodable.co/

### multimodal

- https://www.lancedb.com/
### graph

- https://www.youtube.com/watch?v=X_RFo616M_U
- https://kuzudb.com/

### vector

- https://turbopuffer.com/
### timeseries

- timescale https://www.timescale.com/
- https://www.timeplus.com/
- https://questdb.io/
- https://tembo.io/blog/pg-timeseries
- https://github.com/GreptimeTeam/greptimedb
- duckdb inspired
  - https://github.com/Basekick-Labs/arc

### key-value (like)

- Redis
- https://github.com/valkey-io/valkey
- https://aws.amazon.com/de/elasticache/
- https://aws.amazon.com/de/memorydb/
- https://www.memcached.org
- https://www.bauplanlabs.com/
- https://hazelcast.com
- https://www.dragonflydb.io/redis-alternative

### log structured data structures and brokers

- https://github.com/microsoft/FASTER and https://github.com/faster-rs/faster-rs
- https://redpanda.com/
- https://kafka.apache.org/

### text search

- https://github.com/paradedb/paradedb https://blog.paradedb.com/pages/elasticsearch_vs_postgres
  - https://github.com/quickwit-oss/tantivy
- https://gitlab.science.ru.nl/informagus/zoekeend/
#### observability

- https://www.scopedb.io/

### PG addons

- approximate
  - https://github.com/citusdata/postgresql-hll

## interesting message queues

- https://zeromq.org/
- 
### on basis of PostgreSQL
- https://github.com/tembo-io/pgmq
- https://github.com/hatchet-dev/hatchet

## visualization and admin

- https://trailbase.io/

## self service pipelines

- https://github.com/n8n-io/n8n

## end user onboarding

### web based code editors

- https://devpod.sh/

# remote workspaces gitlab airgapped

# rust speed tools

## storage

- https://developmentseed.org/obstore/latest/

- https://gitlab.com/vtak/gitlab-workspaces-kubernetes-webhook
- https://gitlab.com/groups/gitlab-org/-/epics/14001#top


## data linkeage

- https://github.com/moj-analytical-services/splink https://realworlddatascience.net/case-studies/posts/2023/11/22/splink.html

## template
- https://copier.readthedocs.io/en/stable/
- https://github.com/sixfeetup/scaf

## model

### modeling tools

- https://www.drawdb.app/
### quality

- https://practicaldatamodeling.substack.com/p/data-model-smells

## record linkeage

books
- https://link.springer.com/book/10.1007/978-3-642-31164-2

probabilistic
- https://moj-analytical-services.github.io/splink/#__tabbed_1_2

neat utilities
- https://github.com/dell-research-harvard/linktransformer


## AI BI apps

- https://www.rilldata.com/
- https://www.sigmacomputing.com/

## BI 

- https://github.com/djbarnwal/rill-developer
- https://github.com/visivo-io/visivo


## duckdb addons

- https://github.com/TFMV/arrowport
- https://omni.co/
- https://www.zenlytic.com/


## semantic layer

- https://www.youtube.com/watch?v=DZkXvdzYlVs https://www.malloydata.dev/


# HPC

## parallel computing

- https://parsl.readthedocs.io/en/stable/


# ducklake
## sqlmesh

- https://www.linkedin.com/pulse/build-open-lakehouse-your-laptop-ducklake-sqlmesh-madson-msc-mba-kjuzc/?trackingId=ys2obi8yJyaftwCY1vg0Gw%3D%3D
