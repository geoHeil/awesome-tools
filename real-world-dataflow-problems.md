# real world dataflow problems
Some problems I observed in real dataflow pipelines

## ETL
- quality controlling data prior to ingest from source systems
- actually knowing (responsibility for bought applications) where to find the data(base) and who knows about the format
- parameterize everything, most importantly the fileds
### security
- know the difference between masking field values on the fly i.e. in ranger vs actually not having the permissions to view a column which often (at lest for hive) disallows then to execute the `DESCRIBE TABLE` statement so any tool like tableau which relies on this will subsequently fail
- understand knox https://community.hortonworks.com/content/kbentry/113013/how-to-troubleshoot-and-application-behind-apache.html

## operations
- use HAproxy instead of mysql router for hive HA setups for metastore
- centos os for locally installed cluster
- make sure to really consider if the cluster is only meant for analytics or if it is not more reasonable to run the analytics cluster on kubernetes / openshift
### hardware
- use intel CPUs. Hdoop 3.0 will use erasure coding. ISA-L intel library can greatly speed up compressions https://issues.apache.org/jira/browse/HDFS-7285

## machine learning
- no proper strategy for holdout group and prevention of feedback
- model serving not scalable, no fully fledged ML solution available
- when woring on a machine learning prototype the chance is high - if the results look promising that the model needs to be deployed int oa production environment. Business stakeholders will expect a smooth & quick transition to production mode (results already look so great). Therefore, make sure to only use data sources which are actually available in a production setting, and make sure to get the data directly at the source
- understand the problem domain. Very often regular k-fold cross validation is not a perfect fit as there is a dependency on time. Use time series cross validation (possibly customized) to perform CV in a setting which resembles the actual business use case


## hiring
- if in doubt hire a data engineer and not a data scientist (especially when starting out to bring data driven processes into the company) assuming the engineer also has a feeling for strategy
- but watch out that communication skills are great as well
- make sure to have enough *process* and engineering in the team to build a solid and *regular* IT software development lifecycle process accoring to current standards
- not any (great) developer is a great teamlead

## big data
**DO NOT do big data!** unless you really have big data and fully understand all the consequences of a distributed system.
Instead, invest a couple of $$ into beefier single node computers. High single thread performance + lots of RAM will make you so much more productive.