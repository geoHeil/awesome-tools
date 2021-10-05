# data science

## basics

- https://missing.csail.mit.edu/

## exploratory data analysis (EDA)

- automated EDA
  - python
    - https://sci-analysis.readthedocs.io/en/latest/
    - https://github.com/pandas-profiling/pandas-profiling
    - https://amueller.github.io/dabl/dev/
  - R
    - https://boxuancui.github.io/DataExplorer/
    
## scaling pandas

- elasticsearch: https://github.com/elastic/eland
- dask
- ray/modin
- RAPIDS
- vaex
- https://ibis-project.org/

## experiment design

- http://docs.pyro.ai/en/stable/contrib.oed.html

## bayesian analyses

- frameworks
  - stand
  - pymc
  - pyro https://arviz-devs.github.io/arviz/
- https://botorch.org/
- https://arviz-devs.github.io/arviz/

## deep learning

- books
  - https://github.com/fastai/fastbook
- a really useful link collection on my blog: https://georgheiler.com/2020/12/03/intersting-links-about-deep-learning/
- automated/easy DL
  - https://github.com/geekjr/quickai
  - https://pythonawesome.com/a-framework-that-implements-automl-algorithms-for-model-architecture-search-at-scale/
  
## neighbor search

- https://ai.googleblog.com/2020/07/announcing-scann-efficient-vector.html
- https://github.com/spotify/annoy
### subgroup discovery

- https://github.com/flemmerich/pysubgroup
- https://github.com/imoscovitz/wittgenstein
- https://github.com/scikit-learn-contrib/skope-rules

## NLP

- https://pythonawesome.com/attention-based-grapheme-to-phoneme-with-python/

## reprodrucibility

### population drift monitoring

- https://github.com/ing-bank/popmon

### exploration of models

- exploration in a nice HTML UI by the end user to get a feel for the model or feedback: https://github.com/gradio-app/gradio

### fairness

- https://www.youtube.com/watch?v=WfcCXlxkBb0, https://github.com/koaning/scikit-lego
- https://koaning.io/posts/the-future-is-past/


### explainable AI

- https://github.com/interpretml/interpret

### version control
- improve jupyter git integration http://timstaley.co.uk/posts/making-git-and-jupyter-notebooks-play-nice/
- https://elyra.readthedocs.io/en/latest/

## streaming data science
### libraries
- https://github.com/alibaba/alink


## data

### audio

- feature calculation
  - https://github.com/jcvasquezc/DisVoice

### streams

- jupyter
  - bokeh on streams in jupyter https://medium.com/swlh/streaming-time-series-with-jupyter-and-influxdb-fec33803c460


## forecasting (time series)

- https://www.youtube.com/watch?v=jo12CWZ00Lo
- https://github.com/linkedin/greykite
- https://facebook.github.io/prophet/

### generic timeseries operations
- https://khiva.readthedocs.io/en/latest/
- cleaning https://towardsdatascience.com/a-common-mistake-to-avoid-when-working-with-time-series-data-eedf60a8b4c1



## website tracking

### google analytics

- schema overview http://storage.googleapis.com/e-nor/visualizations/bigquery/ga360-schema.html

### CDH customer data management

basically SQL-based sync & incremental updates of data to many systems and reports without sending a lot of CSV files around

- https://www.hightouch.io/
- https://www.getcensus.com/


## deployment

- https://github.com/whylabs/whylogs

### cloud instance handling

- cheap training using spot instances https://www.spotml.io/
