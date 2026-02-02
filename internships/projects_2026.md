# Project Ideas for 2026


Below is a list of ideas for longer mid-year projects 2025 with `sktime`.
For getting started or smaller projects, see our curated list of [good first issues and advice on getting started as an sktime developer](https://github.com/sktime/sktime/issues/1147).

The below list is only an ideas starter - we welcome and actively encourage bringing your own ideas to the table!

For information on mentoring, summer programmes and application processes, see [here](https://github.com/sktime/mentoring) for the newest information.

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

### Foundation Models

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


### pytorch-forecasting & dsipts - redesign, sktime integration

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

