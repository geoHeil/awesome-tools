# awesome-tools
curated list of awesome tools and libraries for specific domains

## Excel in python
- pandas
- editing data in jupyter notebooks: https://github.com/quantopian/qgrid

## geospatial processing
- python
  - plotting raster https://github.com/fmaussion/salem
  - raster handling http://xarray.pydata.org/en/stable/
  - multi dimensional arrays http://xarray.pydata.org/en/stable/
  - spatial data including joins (works with dask) http://geopandas.org
  - cleaning of addresses: https://github.com/openvenues/libpostal
- postgis
  - multi dimensional
    - http://www.nearimprov.com/nd-spatial-index-in-postgis/
- hadoop
  - http://www.geomesa.org
    - https://github.com/spatialcurrent/ansible-geomesa-accumulo-ubuntu
  - https://github.com/DataSystemsLab/GeoSpark
  - https://github.com/harsha2010/magellan
  - https://github.com/locationtech/geowave
  - https://github.com/locationtech/geotrellis
    - http://rasterframes.io
  - https://github.com/Esri/spatial-framework-for-hadoop and https://github.com/Esri/gis-tools-for-hadoop as well as their java api https://github.com/Esri/geometry-api-java
  - https://github.com/ngageoint/mrgeo
  
 ### indexing
 - https://github.com/riskaware-ltd/open-eaggr
 - https://github.com/uber/h3
  

## nlp
- http://www.nltk.org/book/
- https://github.com/keon/awesome-nlp
- https://github.com/JohnSnowLabs/spark-nlp
- https://github.com/databricks/spark-corenlp (check license extra carefully for commercial setup)
- pyspark with https://spacy.io
- https://explosion.ai
- https://github.com/clulab/processors
- https://github.com/google/sling
- https://github.com/facebookresearch/faiss
- https://github.com/bplank/bilstm-aux
- https://github.com/facebookresearch/fastText
- https://github.com/facebookresearch/InferSent
- https://github.com/google/sentencepiece
- https://github.com/zalandoresearch/flair
- https://github.com/Microsoft/BlingFire

### chatbots
- https://rasa.com

## clustering & distances
- https://github.com/nmslib/nmslib
- T-SNE interactive https://js.tensorflow.org
- UMAP (faster alternative to T-SNE) https://github.com/lmcinnes/umap
- fast DBSCAN. https://github.com/scikit-learn-contrib/hdbscan

### textual preprocessing
- parsing HTML
  - https://github.com/GravityLabs/goose
  - https://github.com/ruippeixotog/scala-scraper
- clustering
  - https://github.com/derrickburns/generalized-kmeans-clustering

## operations & monitoring
- general operations
  - logging & alerting
    - https://sentry.io/welcome/
    - https://bosun.org
    - https://www.datadoghq.com/product/
    - https://opencensus.io
 - certificates
    - https://certbot.eff.org and https://letsencrypt.org for free and automated https/ssl certificates
- hadoop monitoring
  - https://github.com/linkedin/dr-elephant
  - https://github.com/qubole/sparklens
  - https://sites.google.com/site/sparkbigdebug/home
  - https://github.com/SparkMonitor/varOne (not maintained)
  - performance test https://github.com/databricks/spark-perf
  - https://github.com/conversant/spark-profiler
- testing
  - https://www.slideshare.net/hkarau/testing-and-validating-distributed-systems-with-apache-spark-and-apache-beam-fosdem-2018-1?trk=v-feed
- data quality
  - hadoop
    - https://github.com/FRosner/drunken-data-quality
- packer base images
  - http://chef.github.io/bento/

## time series
**small**
- [sktime](https://github.com/alan-turing-institute/sktime) and [sktime-dl](https://github.com/sktime/sktime-dl)
- prediction
  - https://www.youtube.com/watch?v=0zpg9ODE6Ww
  - https://www.youtube.com/watch?v=68ABAU_V8qI
  - https://cran.r-project.org/web/packages/forecast/index.html
  - https://github.com/facebook/prophet
  - https://pythonawesome.com/probabilistic-time-series-modeling-in-python/
  - bayesian structural https://cran.r-project.org/web/packages/bsts/index.html
  - multi prediction
    - https://cran.r-project.org/web/packages/forecastHybrid/index.html
    - https://cran.r-project.org/web/packages/opera/index.html https://github.com/Dralliag/opera
  - https://github.com/ellisp/forecastxgb-r-package
  - https://github.com/dmbee/seglearn
  - https://pytorch-forecasting.readthedocs.io/en/latest/index.html
- feature extration
  - https://github.com/blue-yonder/tsfresh
  - https://robjhyndman.com/hyndsight/tspackages/
  - https://www.featuretools.com (but also worth in general)
- anomalies
  - https://github.com/Yelp/elastalert

**hadoop**
- handling & prediction
  - https://github.com/sryza/spark-timeseries
  - https://spark-summit.org/2016/events/huohua-a-distributed-time-series-analysis-framework-for-spark/
  - https://github.com/twosigma/flint
  - https://databricks.gitbooks.io/databricks-spark-reference-applications/content/timeseries/index.html
  - correlation https://github.com/Sotera/correlation-approximation
  - https://github.com/sryza/spark-timeseries
- anomaly detection
  - https://github.com/numenta/htm.java
  - https://github.com/YuhaoCheng/PyAnomaly
- examples
  - streaming
    - https://github.com/confluentinc/demo-scene/blob/master/ksql-atm-fraud-detection/ksql-atm-fraud-detection-README.adoc
- storage
  - http://www.chronix.io
## machine learning
**model metadata**
- https://github.com/IDSIA/sacred
- http://studio.ml (also hyper opt)
- https://github.com/mitdbg/modeldb
- https://dataversioncontrol.com
- https://www.comet.ml
- https://aetros.com
- https://github.com/ModelChimp/modelchimp
- https://flyte.org/

**model building**
- feature engineering
  - https://www.featuretools.com
- small
  - http://scikit-learn.org/stable/
  - production processes https://github.com/quantumblacklabs/kedro
  - R
    - preprocessing
      - https://cran.r-project.org/web/packages/vtreat/index.html
  - python
    - automl
      - teapot
      - http://automl.github.io/auto-sklearn/stable/
    - https://github.com/kingfengji/gcForest
    - lambda https://www.youtube.com/watch?v=eF-4CrS_j_4
    - improved python https://software.intel.com/en-us/articles/using-intel-distribution-for-python-with-anaconda
    - https://github.com/mthh/jenkspy breaks
    - https://github.com/NeerajSarwan/CPT
- hadoop
  - https://spark.apache.org/mllib/
  - https://github.com/amidst/toolbox
  - fast aggregation in spark https://github.com/tdunning/t-digest
- ensembling
  - http://ml-ensemble.com
  - https://github.com/viisar/brew
  - https://github.com/civisanalytics/civisml-extensions
- specific great models
  - gradient boosted trees
    - xgboost
    - lightgbm
      - https://github.com/Azure/mmlspark
    - catboost https://github.com/catboost/catboost
- visualization of results
  - https://github.com/DistrictDataLabs/yellowbrick
  
  
 **model serving**
- own API wrapper around original model code
- http://clipper.ai
- https://mlflow.org
- https://www.acumos.org
- https://polyaxon.com
- http://vespa.ai
- https://github.com/RedisLabsModules/redis-ml
- https://riseml.com
- https://github.com/Hydrospheredata/mist
- https://github.com/Azure/ai-toolkit-iot-edge
- https://www.dominodatalab.com and various other cloud data science work benches
- https://datmo.com
- https://aws.amazon.com/de/sagemaker/

**model serialization**
- PMML
- https://github.com/combust/mleap

**hyperparameter tuning**
- https://github.com/kubeflow/katib
- https://sigopt.com
- https://github.com/scikit-optimize/scikit-optimize
- https://github.com/Yelp/MOE

**e2e**
- https://www.seldon.io
- http://pipeline.ai
- https://datmo.com

**ml solutions**
- https://predictionio.incubator.apache.org
- https://www.dominodatalab.com

**bridiging python / r and big data**
- http://blog.madhukaraphatak.com/pipe-in-spark/
- sparklyR
- https://github.com/apple/turicreate out of core models on medium sized data

**graph processing**
- hadoop
  - https://tinkerpop.apache.org
  - https://github.com/dbs-leipzig/gradoop
  - https://github.com/gchq/Gaffer
  - https://graphframes.github.io/index.html
  - connector to neo4j https://github.com/neo4j-contrib/neo4j-spark-connector
  - communities
    - https://github.com/Sotera/distributed-graph-analytics/tree/master/dga-graphx
- non hadoop
  - https://neo4j.com (single master, multi slave cluster possible)
- tutorial
  - paradise papers https://github.com/johnymontana/pp-viz/blob/master/jupyter/PP_Viz.ipynb

## cool videos
- telco hadoop geospatial
  - https://www.youtube.com/watch?v=VtvP54Xo3Ek&feature=youtu.be
  - streaming and declarative models: https://www.youtube.com/watch?v=Do7C4UJyWCM
- ml
  - ml pipelines https://www.youtube.com/watch?v=cpR6Vkp7ImA
  - shingles and pipelines https://www.youtube.com/watch?v=qkrh35IF2SU, https://github.com/PacktPublishing/Mastering-Spark-for-Data-Science
  - gradient boosting comparision: https://www.youtube.com/watch?v=5CWwwtEM2TA
- streaming
  - kafka https://www.youtube.com/watch?v=MNPI925PFD0
  - spark streaming in depth https://www.youtube.com/watch?v=hyZU_bw1-ow
  - python https://github.com/mrocklin/streamz
- SQL hadoop & BI https://www.youtube.com/watch?v=v40HWIlsE_w&t=0s&list=PLSAiKuajRe2kGgi-GhMVE8IXzr5Pb3b5y&index=13
- BMW self driving car & spark https://www.youtube.com/watch?v=ub2ufKrrAIs&t=0s&list=PLSAiKuajRe2kGgi-GhMVE8IXzr5Pb3b5y&index=27

## visualization
- python
  - https://python-graph-gallery.com for inspiration
  - seaborn
- R
  - ggplot2 + grest themes
- javascript
  - https://uber.github.io/deck.gl/#/
  - https://dc-js.github.io/dc.js/

**bi & dashboarding**
- https://metabase.com
- https://looker.com
- python
  - https://github.com/stitchfix/pyxley
**notebooks**
- jupyter
  - http://beakerx.com
  - https://medium.com/netflix-techblog/notebook-innovation-591ee3221233
- zeppelin

**type safety**
- https://github.com/typelevel/frameless

## probabilistic programming
- stan
- pymc3
- https://github.com/uber/pyro

## databases
- https://www.cockroachlabs.com (spanner)
- https://www.snowflake.net/de/
- https://snowplowanalytics.com/products/snowplow-open-source/
- hbase-spark
  - via phenix spark
  - https://github.com/hortonworks/shc-release/tree/HDP-2.6.3.0-235-tag
- postgres on GPUs http://www.brytlyt.com
- improved cassandra scylla http://www.scylladb.com
- https://www.mapd.com/platform/
- https://clickhouse.yandex
- https://github.com/biokoda/actordb
- https://clemenswinter.com/2018/07/09/how-to-analyze-billions-of-records-per-second-on-a-single-desktop-pc/amp/
### graph dbs
- streaming graphs https://github.com/NationalSecurityAgency/lemongraph

**time series DBs**
- https://timescale.com

**big real time analytics and data integration**
- https://medium.com/@leventov/comparison-of-the-open-source-olap-systems-for-big-data-clickhouse-druid-and-pinot-8e042a5ed1c7
- https://www.quora.com/Should-I-use-Gobblin-or-Spark-Streaming-to-injest-data-from-Kafka-to-HDFS/answer/Prithiviraj-Damodaran

## scala
### configuration
- typesafe configuration
- https://cir.is/docs/validation
- https://github.com/pureconfig/pureconfig

## bio-informatics
- https://github.com/MG-RAST/AWE

## startup
- founding / payments https://stripe.com/atlas
- errors
  - https://www.youtube.com/watch?v=zFYcXvOrwDE
- analytics
  - https://thinkgrowth.org/the-startup-founders-guide-to-analytics-1d2176f20ac1
  - https://retina.ai/blog/dataops-principles/
- data selling company (data as a service DSSV) https://blog.safegraph.com/data-as-a-service-bible-everything-you-wanted-to-know-about-running-daas-companies-d4cf4c15c038

## recommender
- https://github.com/actionml/universal-recommender
- https://github.com/DataSystemsLab/recdb-postgresql


## governance
- apache atlas
- cloudera navigator
- https://www.waterlinedata.com (hadoop only)
- https://alation.com (all)
- https://www.privitar.com

## blockchain
- data mining
  - https://www.openmined.org

## next gen big data tools
- https://www.weld.rs
- https://datafusion.rs
- http://pachyderm.io
- https://github.com/frankmcsherry/differential-dataflow
