
## Summer project ideas 2024

Below is a list of ideas for longer summer projects 2024 with `sktime`.
For getting started or smaller projects, see our curated list of [good first issues and advice on getting started as an sktime developer](https://github.com/sktime/sktime/issues/1147).

The below list is only an ideas starter - we welcome and actively encourage bringing your own ideas to the table!

For information on mentoring, summer programmes and application processes, see [here](https://github.com/sktime/mentoring) for the newest information.


### various easy tasks - "easy" project or for 1st weeks

* "good first issues" for getting started
* suitable for 1st couple weeks and/or contributors new to open source
* https://github.com/alan-turing-institute/sktime/issues/1147

Skills: only the basics

Getting started: https://www.sktime.net/en/stable/developer_guide.html

Expected outcomes: multiple small improvements to sktime documentation, existing mature modules, bugfixes

Stretch goal: move on quickly to a medium or hard difficulty project :-)

Mentors: any

Difficulty: easy

Length: 175 hours (or less)


### global forecasting and reduction forecasting

* addition of global forecasting capability (with `fit` specific instances) to base class
    * https://github.com/sktime/sktime/issues/4651
* rework and extensions to direct, recursive forecasting
    * flexible model specification interface for exogenous variables and features
    * meta-strategies for global forecasting with `fit` specific instances
* integration of third party algorithms with global forecasting capability, e.g., `pytorch-forecast`

Skills: statistical and ML approaches to forecasting, 

Getting started: implement a new global forecaster based on `sklearn` ML methods

Expected outcomes: global forecasting API, extended selection of global forecasters

Stretch goal: benchmarking study of global forecasters, or building deep learning model

Mentors: benheid, fkiraly

Difficulty: medium

Length: 350 hours


### time-to-event modelling, probabilistic forecasting, probabilistic supervised learning

* help developing the [`skpro`](https://github.com/sktime/skpro/issues) package - distributions, time-to-event models, reductions
* help implement estimators and compositors from the wishlists:
   * skpro: [estimators](https://github.com/sktime/skpro/issues/7), [distributions](https://github.com/sktime/skpro/issues/22)
   * sktime: [proba forecasting list](https://github.com/sktime/sktime/issues/1742), [proba for compositors list](https://github.com/sktime/sktime/issues/2088), [hierarchical reconciliation](https://github.com/sktime/sktime/issues/2157)
* examples: model-based prediction intervals, probabilistic ensembles
* tuning, pipelines, composition

Skills: methodology (forecasting), probability, "rolling your own estimator", sklearn internals

Getting started: adding `predict_interval` and `predict_proba` for estimators

Expected outcomes: implemented 3-5 interesting estimators in the area

Stretch goal: stream or point process modelling functionality

Mentors: fkiraly, frthjf

Difficulty: medium

Length: 175 or 350 hours


### bootstrapping, simulation & ensemble models

* develop modules for boostrapping, simulation and probability objects, eg distributions over time series
* work towards integration with `tsbootstrap` package
* implement ensemble and tuning models based on bootstrap/simulation strategies

Skills: methodology (probability)

Getting started: implement a splitter

Expected outcomes: integration with `tsbootstrap`, `sktime` coverage and discoverability

Stretch goal: integration with sampling/distributions, `skpro`, advanced roadmap items

Mentors: astrogilda, fkiraly, benheid

Difficulty: Medium

Length: 350 hours


### categorical and time-constant features in forecasting

* extend framework for full support of categorical features and time-constant features
* implement transformers and feature extractors, or interface 3rd party
* ensure pipelines, tuning, composites, hierarchical support work end-to-end

Skills: sklearn and sklearn extensions with categorical features, framework/python, helpful: familiarity with finance or retail use cases

Getting started: interface a categorical feature encoder

Expected outcomes: basic support for categorical features in sktime

Stretch goal: full end-to-end support, noteobook/tutorials

Mentors: yarnabrina, fkiraly

Difficulty: Medium

Length: 350 hours


### annotation & segmentation

* work with sktime core developers to design and create new module(s) for time series annotation
* annotation includes: segmentation, change point detection, outlier detection
* implementing base stock of estimators, interfacing popular specialist packages

Skills: design/architecture, methodology (annotation)

Getting started: segmentation wishlist

Expected outcomes: functioning experimental module "annotation" and/or "segmentation"

Stretch goal: "own" one of the modules!

Mentors: fkiraly, achieveordie

Difficulty: hard

Length: 350 hours


### graphical pipelines

* help design an build flexible building blocks for pipeline/composition
* graphical pipelines
* create pipeline builders that cross modules and tasks
* ensuring performance: caching, vectorization

Skills: design/architecture, sklearn internals

Getting started: polymorphic pipeline

Expected outcomes: advanced pipeline module, cross-package

Stretch goal: pipeline specification language

Mentors: benheid, fkiraly

Difficulty: hard

Length: 175 or 350 hours


### benchmarking framework

* create and refactor `sktime` benchmarking framework
* statistical evaluation, visualization, and reporting functionality
* conduct benchmarking studies in cutting edge areas, e.g., forecasting

Skills: methodology (evaluation), design/architecture

Getting started: forecasting benchmarks

Expected outcomes: professional benchmarking framework module

Stretch goal: run or replicate a major benchmarking study, publish paper

Mentors: tbd

Difficulty: medium

Length: 175 or 350 hours


### scaling, backends, foundation models - `polars`, `pytorch`, `huggingface`

* integration with distributed and parallel backends - `polars`, `ray`, etc
* integration with deep learning backends - `pytorch`, `pytorch-forecast`
* integration with huggingface
  design forecasting sub-base class for deep learning back-ends
* create interface and flexible back-end layers

Skills: DL/LLM (pytorch, huggingface), methodology (deep learning), familiarity with distributed/parallel back-ends

Getting started: interface pytorch-forecast or darts

Expected outcomes: a few deep learning forecasters integrated

Stretch goal: public foundation model for forecasting, "own" deep learning module, or benchmarking study

Mentors: benheid, fkiraly

Difficulty: hard

Length: 350 hours
