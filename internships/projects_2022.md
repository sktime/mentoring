## Summer project ideas 2022

Below is a list of ideas for longer summer projects 2022 with `sktime`.
For getting started or smaller projects, see our curated list of [good first issues and advice on getting started as an sktime developer](https://github.com/alan-turing-institute/sktime/issues/1147).

The below list is only an ideas starter - we welcome and actively encourage bringing your own ideas to the table!

For information on mentoring, summer programmes and application processes, see [here](https://github.com/sktime/mentoring) for the newest information.


### annotation & segmentation

* work with sktime core developers to design and create new module(s) for time series annotation
* annotation includes: segmentation, change point detection, outlier detection
* implementing base stock of estimators, interfacing popular specialist packages

Skills: design/architecture, methodology (annotation)
Getting started: segmentation wishlist
Stretch goal: "own" one of the modules!
Difficulty: challenging

### probabilistic & hierarchical/global forecasting

* help implement estimators and compositors from the wishlist
* examples: reconciliation, bootstrap prediction intervals, time series augmentation
* tuning, pipelines, ensembling

Skills: methodology (forecasting), "rolling your own estimator", sklearn internals
Getting started: reconciliation or augmentation
Stretch goal: probabilistic supervised learning package
Difficulty: average

### stream forecasting interfaces

* help refactor and consolidate stream forecasting interfaces
* integrate with stream supervised learning packages
* implement stream compositors, e.g., "re-fit every X periods" or "re-fit on condition"

Skills: design/architecture, methodology (stream/on-line)
Getting started: `update`, `update_predict` refactor
Stretch goal: benchmarking study, or "cross-module" stream functionality
Difficulty: average

### flexible pipelines and composition

* help design an build flexible building blocks for pipeline/composition
* create pipeline builders that cross modules and tasks
* ensuring performance: caching, vectorization

Skills: design/architecture, sklearn internals
Getting started: forecasting pipelines
Stretch goal: pipeline specification language
Difficulty: challenging

### benchmarking framework

* create and refactor `sktime` benchmarking framework
* conduct benchmarking studies in cutting edge areas, e.g., forecasting
* statistical evaluation, visualization, and reporting functionality

Skills: methodology (evaluation), design/architecture
Getting started: forecasting benchmarks
Stretch goal: run or replicate a major benchmarking study, publish paper
Difficulty: average

### deep learning!

* implement or integrate key deep learning methods for forecasting or classification
* refactor parts of legacy `sktime-dl` code
* create interface and flexible back-end layers

Skills: neural network packages (tensorflow, pytorch), methodology (deep learning)
Stretch goal: "own" deep learning module, or benchmarking study
Difficulty: challenging
