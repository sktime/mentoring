# sktime - Google Season of Docs 2024 proposal

This is the full proposal for sktime at GSoD 2024.

For the [applicant info page, see here](https://github.com/sktime/mentoring/blob/main/internships/gsod2024.md).

## improving the user journey for finding information on ML/AI algorithms, tags, metadata

## About sktime

[``sktime``](https://www.sktime.net/en/stable/) is a unified framework for machine learning and AI with time series.

sktime - the software - is used as a commodity component in AI systems worldwide.

sktime is openly governed, by the user and developer community, and provides
software interfaces and governance mechanisms for second and third party developers
to contribute, or list, algorithms ("estimators") in sktime compatible interfaces, e.g., forecasters.

``sktime``'s mission:

* an easy-to-use, easy-to-extend, comprehensive **python framework for ML and AI with time series**
* **open source**, permissive license, free to use
* **openly and transparently governed** by the user and developer community, with a charitable core
* a **friendly, responsive, kind and inclusive community**,with an active commitment to fairness and equal opportunity
* an academically, commercially **neutral space**, with an **ecosystem integration** ambition and neutral point of view
* an **educational platform**, providing mentoring and upskilling for all career stages, especially early career

## About the project

### The problem

`sktime` is a library in a quite literal sense of the word - it provides unified interfaces to hundreds of objects (at time of writing: 392),
among them ML/AI algorithms, and other objects such as performance metrics. The objects can be contributed and maintained by anyone in the world.

The full list of objects is presented on the [searchable estimator table, on the sktime webpage](https://www.sktime.net/en/latest/estimator_overview.html),
and can be also retrieved and searched via python, in the library, e.g.,

```python
from sktime.registry import all_estimators

res = all_estimators()
```

Each estimator has tags, e.g., forecasters can be inspected regarding their capabilities, such as being able to make in-sample predictions, probabilistic forecasts, etc.

```python
from sktime.forecasting.arima import ARIMA

ARIMA.get_class_tags()
```

The user journey in the `sktime` documentation has not been too great in providing the user with access to this information.
For instance, the tags are not displayed in the web documentation at all.

While it is possible to retrieve everything in python, the ambition is to make it as easy as possible to obtain the same in our online documentation, in static and interactive elements.

Further, basic information on the taxonomic primitives, e.g., basic estimator types, data types, tags, is missing from the on-line documentation. Examples: what is forecaster, what does it mean to forecast in-sample.
Pages with such information should be created, and cross-linked from the top and mid level API documentation.

### Scope

* user journey design and implementation of improvements to the online documentation, for presentation, lookup, and interlinkage of estimators, algorithms, and other first-class objects in `sktime`
* added technical documentation on taxonomic primitives, e.g., estimator types, data types, tags, in the web documentation
* extensions of `python` code in the package, estimator taxonomy, or web logic that make it easier for the user to search, retrieve, and understand algorithms by their capabilities
* bonus: improvements to formal algorithm taxonomies and core interfaces of the python objects, motivated by improved user journeys, categories, or common user taxonomies not currently mirrored in the `python` design

### Measures of success

* positive user feedback through existing feedback channels (user feedback thread, discord)
* increase in references using new structure/taxonomy made by developers on the help desk
* increase of meaningful user journeys through the estimator tables and potential tag-specific cross-links

### Useful skills

* technical writing with some background in ML, AI, data science, statistics or mathematics
* entry level familiarity with the python data science ecosystem, optimally scikit-learn or comparable packages (not strictly needed)
* basic understanding of data base schemas or object taxonomies
* familiarity with basic contribution workflows using git, GitHub
* nice to have: familiarity with sphinx, reStructuredText, markdown


### Timeline


## Budget

| Budget item     | Amount in USD          | Running total   | Justification   |
|-----------------|-----------------|-----------------|-----------------|
| Technical writer salaries | 10.500 | 10.500 | technical writer |
| Documentation sprint | 2.500 | 13.000 | 1-week sprint for colocation - travel/lodging support, venue |
| Mentor/supervision | 1.950 | 14.950 | 2-3 mentors/supervisors, 1wk FTE |
| Giant inflatable unicorn | 50 | 15.000 | as required by Google |


## Previous experience

### Technical writing

The mentoring programme lead, FK, has created technical documentation (e.g.,``sktime``), and also supervised and mentored technical writers before, in open source context, in an academic context, and in industry projects (15 years experience overall in mentoring/advising/supervising).

``sktime`` has also hosted small documentation projects and a documentation sprint, in 2022 and 2023.

### Google programmes, mentoring

``sktime`` has yearly internships and stipends, and mentoring on a rolling basis,
see the [mentoring programme GitHub](https://github.com/sktime/mentoring/)

We have participated in GSoC in 2021 and 2022, and are participating again in 2024. 

This year, 5 ``sktime`` core community members are active as mentors; over the years, dozens of junior developers have successfully moved through one of our mentoring programmes.

Our experience and continued participation will benefit GSoD, for instance:

* more junior technical writers will receive simultaneous mentoring, on documentation, or on a technical topic in line with their personal learning goals
* we will use established practices and communication patterns for the project, e.g., sprints, project boards, social community channels (discord)
* the technical writers will be embedded in the summer programme, with mentees, recipients of GSoC stipends, core developers, industry contributors
