
## Summer project ideas 2022

Below is a list of ideas for longer summer projects 2022 with `sktime`.
For getting started or smaller projects, see our curated list of [good first issues and advice on getting started as an sktime developer](https://github.com/alan-turing-institute/sktime/issues/1147).

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

Mentors: @fkiraly, @GuzalBulatova, @Lovkush-A , @lmmentel

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

Mentors: @lmmentel, @Lovkush-A

Difficulty: hard

Length: 350 hours

### probabilistic & hierarchical/global forecasting

* help implement estimators and compositors from the wishlists: [proba forecasting list](https://github.com/alan-turing-institute/sktime/issues/1742), [proba for compositors list](https://github.com/alan-turing-institute/sktime/issues/2088), [hierarchical reconciliation](https://github.com/alan-turing-institute/sktime/issues/2157)
* examples: reconciliation (matrix based e.g. min trace and other methods), bootstrap prediction intervals, time series augmentation
* tuning, pipelines, ensembling

Skills: methodology (forecasting), "rolling your own estimator", sklearn internals

Getting started: reconciliation or augmentation

Expected outcomes: implemented 3-5 interesting estimators in the area

Stretch goal: probabilistic supervised learning package

Mentors: @fkiraly, @GuzalBulatova; support: @danbartl, @ltsaprounis

Difficulty: medium

Length: 175 or 350 hours

### stream forecasting interfaces

* help refactor and consolidate stream forecasting interfaces
* integrate with stream supervised learning packages
* implement stream compositors, e.g., "re-fit every X periods" or "re-fit on condition"

Skills: design/architecture, methodology (stream/on-line)

Getting started: refactor `update` and `update_predict`

Expected outcomes: upgraded stream interface for all modules

Stretch goal: benchmarking study, or "cross-module" stream functionality

Mentors: @lmmentel, @fkiraly, @GuzalBulatova

Difficulty: medium

Length: 175 or 350 hours

### flexible pipelines and composition

* help design an build flexible building blocks for pipeline/composition
* create pipeline builders that cross modules and tasks
* ensuring performance: caching, vectorization

Skills: design/architecture, sklearn internals

Getting started: forecasting pipelines

Expected outcomes: advanced pipeline module, cross-package

Stretch goal: pipeline specification language

Mentors: @fkiraly, @GuzalBulatova; support: @aiwalter

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

Mentors: @fkiraly, @Lovkush-A

Difficulty: medium

Length: 175 or 350 hours

### deep learning for time series

* implement or integrate key deep learning methods for forecasting or classification
* refactor parts of legacy `sktime-dl` code
* create interface and flexible back-end layers

Skills: neural network packages (tensorflow, pytorch), methodology (deep learning)

Getting started: port sktime-dl to sktime

Expected outcomes: sktime deep learning functionality up-to-date with current main package

Stretch goal: "own" deep learning module, or benchmarking study

Mentors: @lmmentel, @fkiraly; support: @tonybagnall, @chrisholder

Difficulty: hard

Length: 350 hours
