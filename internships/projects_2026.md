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

* Complete migration to `torch` for Deep learning based models.
* Move the current implementation of DL models from `tensorflow` to `torch`.
* Create a unified workflow with base `dataset` and `model` class. See issue [sktime#7598](https://github.com/sktime/sktime/issues/7598)
* Add new models with `torch` implementation.
* See `sktime` [issue](https://github.com/sktime/sktime/issues/8699) for more details.

Skills: `torch`, methodology (deep learning), familiarity with training, checkpointing, interence, hubs.

Getting started: migrate one `tensorflow` based model to `torch` in `sktime`. You can find some models [here](https://github.com/sktime/sktime/tree/main/sktime/classification/deep_learning).

Expected Outcomes: Complete migration of all `tensorflow` based model to `torch` in `sktime`

Difficulty: 

Mentors:

Length: 

Max projects:


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

Mentors: geetu040, fnhirwa, (benheid)

Difficulty: easy (basic, short), hard (advanced)

Length: 90 hours (short), 175 hours (basic), 350 hours (advanced)

Max projects: 3


### hyperparameter tuning engines, auto-ML and model optimization

* integration of `sktime` with `hyperactive` package, abstract tuners - see [design discussion](https://github.com/SimonBlanke/Hyperactive/issues/93)
* integration of `hyperactive` with `optuna`, `hyperopt`
* refactor implementation of basic tuning strategies - `sktime` forecasting grid search, random search, `skopt` and `optuna` search
* `optuna` based tuning for various learning tasks: detection, classification, time-to-event
* advanced: API refactor
* advanced: implementation of the hyperband algorithm

Skills: python, optimization, automl, `optuna` and similar tuning packages; `sktime` basics

Getting started: implement one new hyperparameter tuning strategy for `sktime` forecasters: https://github.com/sktime/sktime/issues/4188

Expected outcomes: abstract hyperparameter tuning backends available in `sktime` via `hyperactive`

Stretch goal: `hyperactive` complete API design and library for tuning strategies

Mentors: simonblanke, fkiraly

Difficulty: medium (175), hard (advanced)

Length: 175 (basic) or 350 hours (advanced)

Max projects: 1


### gradient-free-optimization algorithms for tuning

`hyperactive` and `gradient-free-optimizers`- new implementation of:

* the harmonic search algorithm
* advanced: the ant-colony optimization algorithm
* space-filling curves (Hilbert-curve, Z-Order curve) for grid-search
* advanced: add new acquisition functions for bayesian optimization
* advanced: autoML module in `sktime` supporting GFO tuners

Skills: python, mathematical optimization;

Getting started: add one new optimization algorithm to [`Gradient-Free-Optimizers`-package](https://github.com/SimonBlanke/Gradient-Free-Optimizers)

Expected outcomes: new optimization algorithms

Stretch goal: performance benchmarking of new algorithm against other optimization algorithms

Mentors: simonblanke, fkiraly

Difficulty: medium (175), hard (advanced)

Length: 175 (basic) or 350 hours (advanced)

Max projects: 1


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

Mentors: geetu040, recreationalmath, fkiraly

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

