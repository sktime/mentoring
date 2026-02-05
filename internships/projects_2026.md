# Project Ideas for 2026


Below is a list of ideas for longer mid-year projects 2025 with `sktime`.
For getting started or smaller projects, see our curated list of [good first issues and advice on getting started as an sktime developer](https://github.com/sktime/sktime/issues/1147).

The below list is only an ideas starter - we welcome and actively encourage bringing your own ideas to the table!

For information on mentoring, summer programmes and application processes, see [here](https://github.com/sktime/mentoring) for the newest information.


## `sktime`

`sktime` is a Python library that makes it easy to analyze and forecast time series data using a scikit-learn-like interface.

Github: https://github.com/sktime/sktime

Website: https://www.sktime.net/

Organisation: [GC.OS](https://gcos.ai/)

Contributor Guide: https://github.com/sktime/sktime/blob/main/CONTRIBUTING.md

### Migration of `tensorflow` based models to `torch`. 

* Complete the migration of deep learning models from tensorflow to torch. See issue [sktime/#8699](https://github.com/sktime/sktime/issues/8699) for more details. The comment section of linked issue contains already migrated models, which can be used as a template. For example, [RNN classifier from sktime/#8842](https://github.com/sktime/sktime/pull/8842) and [RNN regressor from sktime/#9013](https://github.com/sktime/sktime/pull/9013)
* Create a unified workflow with base `dataset` and `model` class. See issue [sktime#7598](https://github.com/sktime/sktime/issues/7598)
* Issue [sktime/#8928](https://github.com/sktime/sktime/issues/8928) has more ideas that can be incorporated as part of advanced projects.
* Add new models with `torch` implementation.
* Project 1 (advanced):
  * task 1: migrate 2 to 4 models (of your choice) from [sktime/#8699](https://github.com/sktime/sktime/issues/8699). Template for migration will be provided. This will give you familiarity of the codebase and an entry point to think about task 2.
  * task 2: implement some enhancements (of your choice) from issues: [sktime#7598](https://github.com/sktime/sktime/issues/7598) and [sktime/#8928](https://github.com/sktime/sktime/issues/8928). 
* Project 2 (advanced):
  * task 1: migrate 2 to 4 models (of your choice) from [sktime/#8699](https://github.com/sktime/sktime/issues/8699). Template for migration will be provided. This will give you familiarity of the codebase and an entry point to think about task 2.
  * task 2: implement some enhancements (of your choice) from issues: [sktime#7598](https://github.com/sktime/sktime/issues/7598) and [sktime/#8928](https://github.com/sktime/sktime/issues/8928)

Skills: `torch`, some parts may require knowledge of torch ecosystem libraries (such as lightning, torchmetrics), methodology (deep learning), familiarity with training, checkpointing, interence, hubs.

Getting started: migrate one `tensorflow` based model to `torch` in `sktime`. See issue [sktime/#8699](https://github.com/sktime/sktime/issues/8699) for more details.

Expected Outcomes: Complete migration of all `tensorflow` based models to `torch` in `sktime`

Difficulty: moderate

Mentors: RecreationalMath

Length: 350 hours (advanced)

Max projects: 2


### foundations models - development, interfaces, research

* mature and complete integrations of pre-trained models and foundation models in `sktime`: [umbrella issue](https://github.com/sktime/sktime/issues/6177)
* layer integration with `pytorch-forecasting` and `scikit-base`
* short: interfacing a 3rd party foundation model from the [umbrella issue](https://github.com/sktime/sktime/issues/6177)
* advanced: re-design of foundation model API elements - pre-training, fine-tuning
* advanced: rearchitecture of existing foundation models in `sktime`, integration with `pytorch-forecasting`

Skills: `torch`, `huggingface`, `transformers`, methodology (DL, LLM), familiarity with training, checkpointing, interence, hubs

Getting started: interface a 3rd party foundation model

Expected outcomes: consolidated interfaces for pre-trained model, forecasting

Stretch goal: other learning tasks, research benchmark study

Mentors: geetu040, fkiraly, RecreationalMath

Difficulty: easy (basic, short), hard (advanced)

Length: 90 hours (short), 175 hours (basic), 350 hours (advanced)

Max projects: 3

### hierarchical models and hierarchical distributions

* extend hierarchical model features in sktime, skpro, prophetverse
* help implement hierarchical estimators, see [hierarchical reconciliation](https://github.com/sktime/sktime/issues/2157)
* API extension to hierarchical predictive distributions: https://github.com/sktime/skpro/issues/212
* advanced: prophetverse - improvements to effects abstractions
* advanced: hierarchical and multi-factor models for proba regression and survival analysis

Skills: pandas/index handling, methodology (hierarchical models), probability, "rolling your own estimator", sklearn internals

Getting started: implement a new hierarchical reconciliation algorithm in `sktime`: https://github.com/sktime/sktime/issues/7609

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

Stretch goal: stream or point process modelling functionality (option 1); Bayesian modelling framework integration (option 2)

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

Getting started: [detection algorithms and metrics wishlist](https://github.com/sktime/sktime/issues/6481)

Expected outcomes: algorithms implemented; advanced compositors (if advanced)

Stretch goal: become maintainer or join an application project

Mentors: tveten, alex-jg3, robot-psychologist

Difficulty: easy (basic, short), medium (advanced)

Length: 90 hours (short), 175 hours (basic), or 350 hours (advanced items)

Max projects: 3


### Foundation Models - `pytorch-forecasting` integration

* mature and complete integrations of pre-trained models and foundation models in `sktime` and `pytorch-forecasting`: See issue [sktime#7598](https://github.com/sktime/sktime/issues/6177) and [pytorch-forecasting#1959](https://github.com/sktime/pytorch-forecasting/issues/1959)
* layer integration with `pytorch-forecasting` and `scikit-base`.
* interfacing a 3rd party foundation model from the umbrella issue
* Create new `DataModule`, `Model` and `pkg` layer specifically for foundation models for `pytorch-forecasting-v2`.
* Creating `pytorch-forecasting` a reliable provider of Foundation models to `sktime` with complete integration

Skills: `torch`, `huggingface`, `transformers`, methodology (DL, LLM), familiarity with training, checkpointing, interence, hubs

Getting started: interface a 3rd party foundation model

Expected outcomes: consolidated interfaces for pre-trained model, forecasting

Stretch goal: other learning tasks, research benchmark study

Difficulty: 

Mentors:

Length: 

Max projects:

## `pytorch-forecasting` and `DSIPTS`

`pytorch-forecasting` is a high-level library for neural network–based time series forecasting.

Github: https://github.com/sktime/pytorch-forecasting

Website: https://pytorch-forecasting.readthedocs.io/

Organisation: [GC.OS](https://gcos.ai/)

Contributor Guide: https://github.com/sktime/pytorch-forecasting/blob/main/CONTRIBUTING.md

### 1. Foundation Models

* mature and complete integrations of pre-trained models and foundation models in `sktime` and `pytorch-forecasting`: See issue [sktime#7598](https://github.com/sktime/sktime/issues/6177) and [pytorch-forecasting#1959](https://github.com/sktime/pytorch-forecasting/issues/1959)
* layer integration with `pytorch-forecasting` and `scikit-base`.
* interfacing a 3rd party foundation model from the umbrella issue
* Create new `DataModule`, `Model` and `pkg` layer specifically for foundation models for `pytorch-forecasting-v2`.
* Creating `pytorch-forecasting` a reliable provider of Foundation models to `sktime` with complete integration

Skills: `torch`, `huggingface`, `transformers`, methodology (DL, LLM), familiarity with training, checkpointing, interence, hubs

Getting started: interface a 3rd party foundation model

Expected outcomes: consolidated interfaces for pre-trained model, forecasting

Stretch goal: other learning tasks, research benchmark study

Difficulty: 

Mentors:

Length: 

Max projects:


### 2. pytorch-forecasting & dsipts - redesign, sktime integration

* Improving D1/D2 layer and `pkg` layer to complete the v2 version
* Complete migration of v1  model implementations to v2 (preferably with minimal changes to the source code).
* Complete integration with `DSIPTS` and `sktime`
* Improve the test framework to include more scenarios and edge cases
* Addition of new models from `tslib` and related packages.
* Addition of `polars` backend to v2 (preferably v2.x)
* See Roadmap issue [here](https://github.com/sktime/pytorch-forecasting/issues/1993)

Getting started: rework one `pytorch-forecasting` model

Expected outcomes: `pytorch-forecasting` rearchitecture & integration to 2.0

Stretch goal: foundation model integration, research benchmark study

Difficulty: 

Mentors:

Length: 

Max projects:

