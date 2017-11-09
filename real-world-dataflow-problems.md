# real world dataflow problems
Some problems I observed in real dataflow pipelines

## ETL
- quality controlling data prior to ingest from source systems
- actually knowing (responsibility for bought applications) where to find the data(base) and who knows about the format 


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
