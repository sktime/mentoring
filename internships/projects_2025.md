## Mid-year project ideas 2025

Below is a list of ideas for longer mid-year projects 2025 with `sktime`.
For getting started or smaller projects, see our curated list of [good first issues and advice on getting started as an sktime developer](https://github.com/sktime/sktime/issues/1147).

The below list is only an ideas starter - we welcome and actively encourage bringing your own ideas to the table!

For information on mentoring, summer programmes and application processes, see [here](https://github.com/sktime/mentoring) for the newest information.



### hierarchical models and hierarchical distributions

* extend hierarchical model features in sktime, skpro, prophetverse
* help implement hierarchical estimators, see [hierarchical reconciliation](https://github.com/sktime/sktime/issues/2157)
* API extension to hierarchical predictive distributions
* advanced: prophetverse - improvements to effects abstractions
* advanced: hierarchical and multi-factor models for proba regression and survival analysis

Skills: pandas/index handling, methodology (hierarchical models), probability, "rolling your own estimator", sklearn internals

Getting started: implement a hierarchical reconciliation algorithm

Expected outcomes: improved support for probabilistic models - API extension or more estimators implemented

Stretch goal: improved integration between sktime, skpro, prophetverse for hierarchical indices

Mentors: felipeangelimvieira, meraldoantonio, SaiRevanth25

Difficulty: medium (basic), hard (advanced)

Length: 175 or 350 hours


### probabilistic forecasting, survival models, Bayesian interfaces

* help developing the [`skpro`](https://github.com/sktime/skpro/issues) package - distributions, time-to-event models, reductions
* help implement estimators and compositors from the wishlists:
   * skpro: [estimators](https://github.com/sktime/skpro/issues/7), [distributions](https://github.com/sktime/skpro/issues/22)
   * sktime: [proba forecasting list](https://github.com/sktime/sktime/issues/1742), [proba for compositors list](https://github.com/sktime/sktime/issues/2088)
* examples: model-based prediction intervals, probabilistic ensembles
* advanced: develop Bayesian modelling API for regression and forecasting - prior/posterior handling, update
* advanced: on-line, stream/update functionality for regression

Skills: methodology (forecasting), probability, "rolling your own estimator", sklearn internals; advanced: methodology (Bayesian, online)

Getting started: adding `predict_interval` and `predict_proba` for estimators

Expected outcomes: implemented 3-5 interesting estimators in the area

Stretch goal: stream or point process modelling functionality

Mentors: felipeangelimvieira, meraldoantonio, SaiRevanth25

Difficulty: medium (basic), hard (advanced)

Length: 175 or 350 hours


### detection framework with sktime and skchange

* work with sktime core developers to expand the detection framework
* segmentation, change point detection, anomaly detection
* implementing and interfacing new algorithms and metrics
* advanced: multi-channel detection
* advanced: tuning, auto-ml, ensembles
* optional: application in affiliated real-world projects

Skills: sklearn and sklearn-like extensions, "rolling your own estimator"; helpful: familiarity with detection tasks

Getting started: detection algorithms and metrics wishlist

Expected outcomes: algorithms implemented; advanced compositors (if advanced)

Stretch goal: become maintainer or join an application project

Mentors: tveten, alex-jb3, robot-psychologist

Difficulty: easy (basic), medium (advanced)

Length: 175 hours (basic), or 350 hours (advanced items)


### benchmarking framework

* create and refactor `sktime` benchmarking framework
* statistical evaluation, visualization, and reporting functionality
* conduct benchmarking studies in cutting edge areas, e.g., forecasting

Skills: methodology (evaluation), design/architecture

Getting started: forecasting benchmarks

Expected outcomes: professional benchmarking framework module

Stretch goal: run or replicate a major benchmarking study, publish paper

Mentors: fkiraly, benheid

Difficulty: medium

Length: 175 or 350 hours
