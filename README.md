# awesome-tools
curated list of awesome tools and libraries for specific domains

## geospatial processing
- python
  - plotting raster https://github.com/fmaussion/salem
  - raster handling http://xarray.pydata.org/en/stable/
  - multi dimensional arrays http://xarray.pydata.org/en/stable/
  - spatial data including joins (works with dask) http://geopandas.org
  - cleaning of addresses: https://github.com/openvenues/libpostal
- hadoop
  - http://www.geomesa.org
  - https://github.com/DataSystemsLab/GeoSpark
  - https://github.com/harsha2010/magellan
  - https://github.com/locationtech/geowave
  - https://github.com/locationtech/geotrellis
  - https://github.com/Esri/spatial-framework-for-hadoop and https://github.com/Esri/gis-tools-for-hadoop as well as their java api

## nlp
- https://github.com/JohnSnowLabs/spark-nlp
- https://github.com/databricks/spark-corenlp (check license extra carefully for commercial setup)
- pyspark with https://spacy.io
- https://github.com/clulab/processors
- https://github.com/google/sling

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
 - certificates
    - https://certbot.eff.org and https://letsencrypt.org for free and automated https/ssl certificates
- hadoop monitoring
  - https://github.com/linkedin/dr-elephant
  - https://sites.google.com/site/sparkbigdebug/home
  - https://github.com/SparkMonitor/varOne (not maintained)
  - performance test https://github.com/databricks/spark-perf
- data quality
  - hadoop
    - https://github.com/FRosner/drunken-data-quality

## time series
**small**
- prediction
  - https://cran.r-project.org/web/packages/forecast/index.html
  - https://github.com/facebook/prophet
  - multi prediction
    - https://cran.r-project.org/web/packages/forecastHybrid/index.html
    - https://cran.r-project.org/web/packages/opera/index.html
  - https://github.com/ellisp/forecastxgb-r-package
- feature extration
  - https://github.com/blue-yonder/tsfresh

**hadoop**
- handling & prediction
  - https://github.com/sryza/spark-timeseries
  - https://spark-summit.org/2016/events/huohua-a-distributed-time-series-analysis-framework-for-spark/
  - https://github.com/twosigma/flint
  - https://databricks.gitbooks.io/databricks-spark-reference-applications/content/timeseries/index.html
  - correlation https://github.com/Sotera/correlation-approximation
  - https://github.com/sryza/spark-timeseries
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

**model building**
- small
  - http://scikit-learn.org/stable/
  - R
- hadoop
  - https://spark.apache.org/mllib/
  - https://github.com/amidst/toolbox
  - https://github.com/tdunning/t-digest
- ensembling
  - http://ml-ensemble.com
  - https://github.com/viisar/brew
- specific great models
  - gradient boosted trees
    - xgboost
    - lightgbm
      - https://github.com/Azure/mmlspark
  
  
 **model serving**
- own API wrapper around original model code
- http://clipper.ai
- http://vespa.ai
- https://github.com/RedisLabsModules/redis-ml
- https://github.com/Hydrospheredata/mist
- https://github.com/Azure/ai-toolkit-iot-edge
- https://www.dominodatalab.com and various other cloud data science work benches

**model serialization**
- PMML
- https://github.com/combust/mleap

**hyperparameter tuning**
- https://sigopt.com
- https://github.com/scikit-optimize/scikit-optimize

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

**graph processing**
- hadoop
  - https://tinkerpop.apache.org
  - https://github.com/dbs-leipzig/gradoop
  - https://github.com/gchq/Gaffer
  - https://graphframes.github.io/index.html
  - communities
    - https://github.com/Sotera/distributed-graph-analytics/tree/master/dga-graphx
- non hadoop
  - https://neo4j.com (single master, multi slave cluster possible)

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

**type safety**
- https://github.com/typelevel/frameless

## probabilistic programming
- stan
- pymc3
- https://github.com/uber/pyro

## databases
- https://www.cockroachlabs.com
- https://www.snowflake.net/de/
- https://snowplowanalytics.com/products/snowplow-open-source/
- hbase-spark
  - via phenix spark
  - https://github.com/hortonworks/shc-release/tree/HDP-2.6.3.0-235-tag
