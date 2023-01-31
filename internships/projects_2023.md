
## Summer project ideas 2023

Below is a list of ideas for longer summer projects 2023 with `sktime`.
For getting started or smaller projects, see our curated list of [good first issues and advice on getting started as an sktime developer](https://github.com/sktime/sktime/issues/1147).

The below list is only an ideas starter - we welcome and actively encourage bringing your own ideas to the table!

For information on mentoring, summer programmes and application processes, see [here](https://github.com/sktime/mentoring) for the newest information.


### various easy tasks - "easy" project or for 1st weeks

* "good first issues" for getting started
* suitable for 1st couple weeks and/or contributors new to open source
* https://github.com/alan-turing-institute/sktime/issues/1147

Skills: only the basics

Getting started: https://www.sktime.org/en/stable/developer_guide.html

Expected outcomes: multiple small improvements to sktime documentation, existing mature modules, bugfixes

Stretch goal: move on quickly to a medium or hard difficulty project :-)

Mentors:

Difficulty: easy

Length: 175 hours (or less)

### annotation & segmentation

* work with sktime core developers to design and create new module(s) for time series annotation
* annotation includes: segmentation, change point detection, outlier detection
* implementing base stock of estimators, interfacing popular specialist packages

Skills: design/architecture, methodology (annotation)

Getting started: segmentation wishlist

Expected outcomes: functioning experimental module "annotation" and/or "segmentation"

Stretch goal: "own" one of the modules!

Mentors: 

Difficulty: hard

Length: 350 hours

### probabilistic forecasting and supervised learning

* help implement estimators and compositors from the wishlists: [proba forecasting list](https://github.com/alan-turing-institute/sktime/issues/1742), [proba for compositors list](https://github.com/alan-turing-institute/sktime/issues/2088), [hierarchical reconciliation](https://github.com/alan-turing-institute/sktime/issues/2157)
* examples: model-based prediction intervals, probabilistic ensembles
* tuning, pipelines, composition

Skills: methodology (forecasting), "rolling your own estimator", sklearn internals

Getting started: adding `predict_interval` and `predict_proba` for estimators

Expected outcomes: implemented 3-5 interesting estimators in the area

Stretch goal: probabilistic supervised learning package

Mentors:

Difficulty: medium

Length: 175 or 350 hours

### develop skbase - base class package

* help integrate `skbase` with `sktime`
* build advanced base class functionality - pipelines, meta-estimators
* co-develop new sub-module of `sktime`: e.g., specialized forecasting tasks

Skills: design/architecture, sklearn development

Getting started: write a new `sktime` module using `skbase`

Expected outcomes: `skbase` feature, e.g., pipelines building blocks or meta-estimators

Stretch goal: new package in `sktime` ecosystem

Mentors:

Difficulty: medium

Length: 175 or 350 hours

### graphical pipelines, integration with `pywatts`

* help design an build flexible building blocks for pipeline/composition
* graphical pipelines, [integration with pywatts package](https://github.com/sktime/sktime/issues/2653)
* create pipeline builders that cross modules and tasks
* ensuring performance: caching, vectorization

Skills: design/architecture, sklearn internals

Getting started: polymorphic pipeline

Expected outcomes: advanced pipeline module, cross-package

Stretch goal: pipeline specification language

Mentors:

Difficulty: hard

Length: 175 or 350 hours

### benchmarking framework, integration with `kotsu`

* create and refactor `sktime` benchmarking framework using `kotsu`
* statistical evaluation, visualization, and reporting functionality
* conduct benchmarking studies in cutting edge areas, e.g., forecasting

Skills: methodology (evaluation), design/architecture

Getting started: forecasting benchmarks

Expected outcomes: professional benchmarking framework module

Stretch goal: run or replicate a major benchmarking study, publish paper

Mentors:

Difficulty: medium

Length: 175 or 350 hours

### deep learning for forecasting

* implement or integrate key deep learning methods for forecasting
* contribute to design forecasting sub-base class for deep learning back-ends
* create interface and flexible back-end layers

Skills: neural network packages (tensorflow, pytorch), methodology (deep learning)

Getting started: interface pytorch-forecast or darts

Expected outcomes: a few deep learning forecasters integrated

Stretch goal: "own" deep learning module, or benchmarking study

Mentors:

Difficulty: hard

Length: 350 hours
