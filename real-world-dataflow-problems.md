# real world dataflow problems
Some problems I observed in real dataflow pipelines

## ETL
- quality controlling data prior to ingest from source systems
- actually knowing (responsibility for bought applications) where to find the data(base) and who knows about the format
- parameterize everything, most importantly the fileds

### SQL
SQL nowadays is so much more than SQL92 (which most people are familiar with). Arrays, json, xml ... can be handled. In case of distributed systems ordering (total ordering vs partial ordering within partitions) turn out to be important concepts to master as well:
- spark https://blog.deepsense.ai/optimize-spark-with-distribute-by-and-cluster-by/
- hive https://saurzcode.in/2015/01/hive-sort-order-distribute-cluster/

### dataflow
- understand the limits of your architecture / technology and dataflows regarding speed, capacity, latency, types of data handlable...
- define clear APIs (schemata) between different data sources and pipelines to allow building workflows on top of the ingested data streams

### security
- know the difference between masking field values on the fly i.e. in ranger vs actually not having the permissions to view a column which often (at lest for hive) disallows then to execute the `DESCRIBE TABLE` statement so any tool like tableau which relies on this will subsequently fail
- understand knox https://community.hortonworks.com/content/kbentry/113013/how-to-troubleshoot-and-application-behind-apache.html

## operations
- use HAproxy instead of mysql router for hive HA setups for metastore
- centos os for locally installed cluster
- make sure to really consider if the cluster is only meant for analytics or if it is not more reasonable to run the analytics cluster on kubernetes / openshift
- own the base and cloud the spike
- consider hybrid cloud (cross cloud provider)
- adhere to https://www.acm.org/binaries/content/assets/public-policy/2017_usacm_statement_algorithms.pdf and especially look out for any data provenance issues
- make sure to setup a file quota in HDFS per user

### llap
llap might not start (in case of a small development cluster) if not enough memory is available or a node is down. However, currently in HDP 2.6.4 no meaningful error message is displayed

### hardware
- use intel CPUs. Hdoop 3.0 will use erasure coding. ISA-L intel library can greatly speed up compressions https://issues.apache.org/jira/browse/HDFS-7285

## machine learning
- no proper strategy for holdout group and prevention of feedback
- model serving not scalable, no fully fledged ML solution available
- when woring on a machine learning prototype the chance is high - if the results look promising that the model needs to be deployed int oa production environment. Business stakeholders will expect a smooth & quick transition to production mode (results already look so great). Therefore, make sure to only use data sources which are actually available in a production setting, and make sure to get the data directly at the source
- understand the problem domain. Very often regular k-fold cross validation is not a perfect fit as there is a dependency on time. Use time series cross validation (possibly customized) to perform CV in a setting which resembles the actual business use case
- proper understanding of the data. Cehck for errors (too much / not ehough / wrong units / ...)
- work with and talk to the department to prevent data leakage into the model
- reproducibility is a problem (https://petewarden.com/2018/03/19/the-machine-learning-reproducibility-crisis/) and the overall pipeline E2E needs to be thought out very well
- model management is a big problem. This book https://mapr.com/ebooks/machine-learning-logistics/ describes it nicely

## hiring
- if in doubt hire a data engineer and not a data scientist (especially when starting out to bring data driven processes into the company) assuming the engineer also has a feeling for strategy
- but watch out that communication skills are great as well
- make sure to have enough *process* and engineering in the team to build a solid and *regular* IT software development lifecycle process accoring to current standards
- not any (great) developer is a great teamlead
- https://rework.withgoogle.com holds great resources regarding hiring & team building
- in case working for a small company read https://medium.com/apteo/what-makes-a-good-data-scientist-at-a-small-company-3f445d421dff
### teams & organization
great article: https://multithreaded.stitchfix.com/blog/2016/03/16/engineers-shouldnt-write-etl/ usually a problem
- either too many data engineers / site reliability engineers
- or a gap (no holistic approach) as separated into segregated teams in different parts of company hierarchy

## big data
**DO NOT do big data!** unless you really have big data and fully understand all the consequences of a distributed system.
Instead, invest a couple of $$ into beefier single node computers. High single thread performance + lots of RAM will make you so much more productive.

**scalability**
Sometimes extreme scalability is not required! Do not get stuck in thinking you actually need it. Think of a scenario of many events for each user but the number of users being alsmost constant. Such a scenario can warrant some different algorithms to optimally process the data.

**small files problem**
many small files (a lot smaller than HDFS block size) cause a performance degredation.
workarounds:
- combine input format (spark whole textfiles)
- use sequence files
- Hadoop archives HAR https://github.com/ZuInnoTe/hadoopoffice/wiki/Improve-performance-for-processing-a-lot-of-small-Office-files-with-Hadoop-Archives-(HAR)
- kafka

## java stuff
### containers
- java and containers still do not play nicely (java9) https://mesosphere.com/blog/java-container/
