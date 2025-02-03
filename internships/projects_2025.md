## Mid-year project ideas 2025

Below is a list of ideas for longer mid-year projects 2025 with `sktime`.
For getting started or smaller projects, see our curated list of [good first issues and advice on getting started as an sktime developer](https://github.com/sktime/sktime/issues/1147).

The below list is only an ideas starter - we welcome and actively encourage bringing your own ideas to the table!

A useful reference is also the [2025 project roadmap](https://github.com/sktime/sktime/issues/7707) for `sktime`, `pytorch-forecasting`, `dsipts`, `skpro`, `skchange`, and adjacent packages.

For information on mentoring, summer programmes and application processes, see [here](https://github.com/sktime/mentoring) for the newest information.


### pytorch-forecasting & dsipts - redesign, sktime integration

* rework of `pytorch-forecasting` & `dsipts` interfaces towards version 2.0
* uniformization of `torch` `dataset` and `dataloader`-s across projects
* short: migrate one or two research grade deep learning models to `pytorch-forecasting`
* advanced: pre-trained models and serialization interfaces - design, implementation
* advanced: rework of `sktime` `torch` backend, move to `pytorch-forecasting`

Skills: `torch`, methodology (deep learning), familiarity with training, checkpointing, interence, hubs

Getting started: rework one `pytorch-forecasting` model

Expected outcomes: `pytorch-forecasting` rearchitecture & integration to 2.0

Stretch goal: foundation model integration, research benchmark study

Mentors: agobbifbk, fnhirwa, fkiraly, (benheid)

Difficulty: easy (basic, short), hard (advanced)

Length: 90 hours (short), 175 hours (basic), 350 hours (advanced)

Max projects: 3


### foundations models - development, interfaces, research

* mature and complete integrations of pre-trained models and foundation models in `sktime`
* layer integration with `pytorch-forecasting` and `scikit-base`
* short: interfacing a 3rd party foundation model from the [umbrella issue](https://github.com/sktime/sktime/issues/6177)
* advanced: re-design of foundation model API elements - pre-training, fine-tuning
* advanced: rearchitecture of existing foundation models in `sktime`, integration with `pytorch-forecasting`

Skills: `torch`, `huggingface`, `transformers`, methodology (DL, LLM), familiarity with training, checkpointing, interence, hubs

Getting started: interface a 3rd party foundation model

Expected outcomes: consolidated interfaces for pre-trained model, forecasting

Stretch goal: other learning tasks, research benchmark study

Mentors: geetu040, fnhirwa, (benheid)

Difficulty: easy (basic, short), hard (advanced)

Length: 90 hours (short), 175 hours (basic), 350 hours (advanced)

Max projects: 3


### hyperparameter tuning engines, auto-ML and model optimization

* integration of `sktime` with `hyperactive` package, abstract tuners
* integration of `hyperactive` with `optuna`, `hyperopt`
* refactor implementation of basic tuning strategies
* `optuna` based tuning for various learning tasks: detection, classification, time-to-event
* advanced: API refactor

Skills: optimization, automl, `optuna` and similar tuning packages;

Getting started: interface pytorch-forecast or darts

Expected outcomes: a few deep learning forecasters integrated

Stretch goal: public foundation model for forecasting, "own" deep learning module, or benchmarking study

Mentors: simonblanke, fkiraly

Difficulty: medium (175), hard (advanced)

Length: 175 (basic) or 350 hours (advanced)

Max projects: 1


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

Mentors: felipeangelimvieira, fkiraly

Difficulty: medium (basic), hard (advanced)

Length: 175 (basic) or 350 hours (advanced)

Max projects: 2


### stream and online support for forecasting and detection tasks

* help expanding efficient stream/online update for existing forecasting models in `sktime`
* stream/update compositors for forecasting models and transformation models
* advanced: stream/update API architecture for transformations
* advanced: stream/update API architecture for anomaly and changepoint detection, predictive monitoring
* short: add `update` method for one or two existing, widely used estimators

Skills: methodology (forecasting, stream/online), "rolling your own estimator"; advanced: sklearn and sktime internals

Getting started: adding dedicated `update` to `statsmodels` estimators, or `NaiveForecaster`

Expected outcomes: implemented update feature for 3-5 forecasters

Stretch goal: stream and online API for forecasting, transformations, and/or detection

Mentors: fkiraly, felipeangelimvieira

Difficulty: easy (basic, short), hard (advanced)

Length: 90 (short), 175 (basic) or 350 hours (advanced)

Max projects: 2


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

Length: 175 (basic) or 350 hours (advanced)

Max projects: 3


### detection framework with sktime and skchange

* expand the detection framework in sktime - segmentation, change point detection, anomaly detection
* short project: implementing and interfacing new algorithms and metrics
* advanced: multi-channel detection
* advanced: tuning, auto-ml, ensembles
* optional: application in affiliated real-world projects

Skills: sklearn and sklearn-like extensions, "rolling your own estimator"; helpful: familiarity with detection tasks

Getting started: detection algorithms and metrics wishlist

Expected outcomes: algorithms implemented; advanced compositors (if advanced)

Stretch goal: become maintainer or join an application project

Mentors: tveten, alex-jb3, robot-psychologist

Difficulty: easy (basic, short), medium (advanced)

Length: 90 hours (short), 175 hours (basic), or 350 hours (advanced items)

Max projects: 3


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

Max projects: 1

Length: 175 or 350 hours
