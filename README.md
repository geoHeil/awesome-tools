# awesome-tools
curated list of awesome tools and libraries for specific domains

## geospatial processing
- python
  - plotting raster https://github.com/fmaussion/salem
  - raster handling http://xarray.pydata.org/en/stable/
  - multi dimensional arrays http://xarray.pydata.org/en/stable/
  - spatial data including joins (works with dask) http://geopandas.org
- hadoop
  - http://www.geomesa.org
  - https://github.com/DataSystemsLab/GeoSpark
  - https://github.com/harsha2010/magellan
  - https://github.com/locationtech/geowave
  - https://github.com/locationtech/geotrellis
  - https://github.com/Esri/spatial-framework-for-hadoop and https://github.com/Esri/gis-tools-for-hadoop as well as their java api

## operations & monitoring
- general operations
  - logging
    - https://sentry.io/welcome/
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
- storage
  - http://www.chronix.io
## machine learning
**model metadata**
- https://www.comet.ml
- http://studio.ml (also hyper opt)

**model building**
- small
  - http://scikit-learn.org/stable/
  - R
- hadoop
  - https://spark.apache.org/mllib/
  - https://github.com/amidst/toolbox
  - https://github.com/tdunning/t-digest
  
  
 **model serving**
- own API wrapper around original model code
- http://clipper.ai
- http://vespa.ai
- https://github.com/RedisLabsModules/redis-ml
- https://github.com/Hydrospheredata/mist

**model serialization**
- PMML
- https://github.com/combust/mleap

**hyperparameter tuning**
- https://sigopt.com

**e2e**
- https://www.seldon.io
- http://pipeline.ai
- https://datmo.com

** ml solutions**
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

## cool videos
- telco hadoop geospatial
  - https://www.youtube.com/watch?v=VtvP54Xo3Ek&feature=youtu.be
  - streaming and declarative models: https://www.youtube.com/watch?v=Do7C4UJyWCM


## visualization
- python
  - https://python-graph-gallery.com for inspiration
  - seaborn
- R
  - ggplot2 + grest themes

**bi & dashboarding**
- https://metabase.com
- https://looker.com
