# data science

## great content

- https://www.youtube.com/watch?v=xC-c7E5PK0Y

## ethics

- https://book.the-turing-way.org/


## nice overview courseware

- https://mlip-cmu.github.io/s2025/
- vis teaching
  - https://github.com/stefmolin/data-morph

## list of useful tools

- https://landscape.lfai.foundation/
- https://github.com/fmind/mlops-python-package
- https://github.com/callmesora/llmops-python-package

## references to further similar lists

- https://github.com/r0f1/datascience

## basics

- https://missing.csail.mit.edu/

## exploratory data analysis (EDA)

- automated EDA
  - python
    - https://sci-analysis.readthedocs.io/en/latest/
    - https://github.com/pandas-profiling/pandas-profiling
    - https://amueller.github.io/dabl/dev/
    - https://www.visidata.org/
    - https://github.com/microsoft/vscode-data-wrangler
  - R
    - https://boxuancui.github.io/DataExplorer/
  
## anomaly detection

- https://pyod.readthedocs.io/en/latest/index.html

## visualization

- https://charticulator.com/
- https://www.datawrapper.de/
- https://flourish.studio/
- https://rawgraphs.io/
- high dimensional data https://github.com/facebookresearch/hiplot

## scaling pandas

- https://github.com/ibis-project/ibis
- elasticsearch: https://github.com/elastic/eland
- dask
- ray/modin
- RAPIDS
- vaex
- https://ibis-project.org/
- https://github.com/pola-rs/polars
  - https://talkpython.fm/episodes/show/510/10-polars-tools-and-techniques-to-level-up-your-data-science
    - https://github.com/ddotta/awesome-polars
    - https://github.com/quantco/dataframely
    - https://github.com/JakobGM/patito
    - https://github.com/foxcroftjn/polars-strsim
    - https://github.com/zlobendog/polars_encryption
    - https://github.com/pola-rs/polars-xdt
    - https://github.com/TomBurdge/harley
    - https://github.com/azmyrajab/polars_ols
    - https://github.com/erichutchins/polars_iptools

## experiment design

- http://docs.pyro.ai/en/stable/contrib.oed.html

## experiment tracking

MLops overview: https://github.com/visenger/awesome-mlops

- mlFlow
- https://docs.bentoml.org
- https://neptune.ai/blog/experiment-management
- https://neptune.ai/blog/mlops-what-it-is-why-it-matters-and-how-to-implement-it-from-a-data-scientist-perspective
- https://towardsdatascience.com/machine-learning-experiment-tracking-93b796e501b0
- https://neptune.ai/blog/machine-learning-model-management

## bayesian analyses

- frameworks
  - stand
  - pymc
  - pyro https://arviz-devs.github.io/arviz/
- https://botorch.org/
- https://arviz-devs.github.io/arviz/
- https://bayesiancomputationbook.com/welcome.html

## deep learning

- books
  - https://github.com/fastai/fastbook
- a really useful link collection on my blog: https://georgheiler.com/2020/12/03/intersting-links-about-deep-learning/
- automated/easy DL
  - https://github.com/geekjr/quickai
  - https://pythonawesome.com/a-framework-that-implements-automl-algorithms-for-model-architecture-search-at-scale/
- tabular deeplearning:
  - https://github.com/dreamquark-ai/tabnet

- https://lets-unify.ai/
  
## neighbor search

- https://ai.googleblog.com/2020/07/announcing-scann-efficient-vector.html
- https://github.com/spotify/annoy
### subgroup discovery

- https://github.com/flemmerich/pysubgroup
- https://github.com/imoscovitz/wittgenstein
- https://github.com/scikit-learn-contrib/skope-rules

## NLP

- https://pythonawesome.com/attention-based-grapheme-to-phoneme-with-python/

### rules
- https://github.com/adaamko/POTATO

## reprodrucibility

### population drift monitoring

- https://github.com/ing-bank/popmon

### exploration of models

- exploration in a nice HTML UI by the end user to get a feel for the model or feedback: https://github.com/gradio-app/gradio

### fairness

- https://www.youtube.com/watch?v=WfcCXlxkBb0, https://github.com/koaning/scikit-lego
- https://koaning.io/posts/the-future-is-past/
- https://github.com/linkedin/LiFT


### explainable AI

- https://github.com/interpretml/interpret

### version control
- improve jupyter git integration http://timstaley.co.uk/posts/making-git-and-jupyter-notebooks-play-nice/
- https://elyra.readthedocs.io/en/latest/

## streaming data science
### libraries
- https://github.com/alibaba/alink
- https://github.com/scikit-multiflow/scikit-multiflow
- https://riverml.xyz/latest/


## data

### audio

- feature calculation
  - https://github.com/jcvasquezc/DisVoice

### streams

- jupyter
  - bokeh on streams in jupyter https://medium.com/swlh/streaming-time-series-with-jupyter-and-influxdb-fec33803c460


### feature store

- hopsworks
- Behaviors compose better than states
  -  perhaps a simple python library with some transformations & DBT & Dagster will do the job very well and https://metriql.com/ for metrics
- https://feast.dev/

## forecasting (time series)

- https://www.youtube.com/watch?v=jo12CWZ00Lo
- https://github.com/linkedin/greykite
- https://facebook.github.io/prophet/
- https://github.com/winedarksea/AutoTS
- https://github.com/timeseriesAI/tsai
- https://github.com/AIStream-Peelout/flow-forecast

### generic timeseries operations
- https://khiva.readthedocs.io/en/latest/
- cleaning https://towardsdatascience.com/a-common-mistake-to-avoid-when-working-with-time-series-data-eedf60a8b4c1



## website tracking

### google analytics

- schema overview http://storage.googleapis.com/e-nor/visualizations/bigquery/ga360-schema.html

### CDM/CDP customer data management & customer data platform

basically SQL-based sync & incremental updates of data to many systems and reports without sending a lot of CSV files around

- https://www.hightouch.io/
- https://www.getcensus.com/


## deployment

- https://github.com/whylabs/whylogs
- clean machine learning code https://leanpub.com/cleanmachinelearningcode
    - code refactoring example https://github.com/moutai/tdml-example/tree/master/with_tests/tests

### cloud instance handling

- cheap training using spot instances https://www.spotml.io/


# use cases

## marketing

- https://facebookexperimental.github.io/Robyn/


# text processing

## ocr

- https://github.com/VikParuchuri/surya


# labeling

- prodigy
- https://github.com/TutteInstitute/thisnotthat
 
## clustering

- https://github.com/TutteInstitute
- https://www.tute.com/


## matching data

entity/identity resolution

- https://linktransformer.github.io/

## LLM resources

- https://github.com/SylphAI-Inc/LLM-engineer-handbook
  - https://github.com/stanfordnlp/dspy
  - https://github.com/SylphAI-Inc/AdalFlow
  - https://github.com/Eladlev/AutoPrompt
  - https://github.com/comet-ml/opik
  - https://github.com/huggingface/lighteval
  - https://github.com/explodinggradients/ragas
  - https://github.com/unslothai/unsloth
  - https://github.com/Lightning-AI/litgpt 
- embeddings
  - https://raw.githubusercontent.com/veekaybee/what_are_embeddings/main/embeddings.pdf

## cleaning

- https://github.com/cleanlab/cleanlab

## vision

- object detection
  - object tracking https://github.com/roboflow/trackers


## interactive computing

notebooks

- https://marimo.io/


## similarity search

### semantic hashing

- https://github.com/MinishLab/semhash
- https://colab.research.google.com/drive/1o1nzwXWAa8kdkEJljbJFW1VuI-3VZLUn?usp=sharing
### minhash

- https://github.com/beowolx/rensa
