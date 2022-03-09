# Welcome to sktime's Google Summer of Code program 2021! 

sktime is participating in Google Summer of Code (GSoC) part of INCF (https://www.incf.org/activities/gsoc). Join the sktime team for a summer full of coding, learning and fun. Be part of our diverse community and join our efforts to advance machine learning and time series analysis capabilities!

We explicitly would like to encourage applications by female and non-binary students, or of minority/underrepresented groups in the tech sector.

If you have questions, please feel free to reach out to us on Gitter (https://gitter.im/sktime/community) or GitHub (https://github.com/alan-turing-institute/sktime/discussions). 

## Why sktime?
Time series data is ubiquitous in many applications. Examples include sensor readings from industrial processes, spectroscopy wave length data from chemical samples, or bed-side monitor medical data from patients. Developing advanced time series analysis capabilities for researchers and practitioners is one of the major challenges of contemporary machine learning. 

sktime is a new Python toolbox for machine learning with time series and, to the best of our knowledge, the first unified toolbox for time series. Our ambition is to provide for time series what scikit-learn provides for tabular data. This involves extending scikit-learn to the different time series learning tasks, such as time series classification, clustering, forecasting and anomaly detection. To find out more, check out our [paper](http://learningsys.org/neurips19/assets/papers/sktime_ml_systems_neurips2019.pdf) published at the [Workshop on Systems for ML at NeurIPS 2019](http://learningsys.org/neurips19/). 

## How to apply?
1. Solve an entrance task by making a pull request (PR) to sktime. Find out more about how to contribute in our guide (https://www.sktime.org/en/latest/contributing.html).
This means opening a sensible PR, but your PR does not need to be merged yet. 
Alternatively, if you are already experienced in using git and GitHub in a collaborative environment, you can skip this step. In this case, please provide a link to publicly visible evidence for your experience in the application form in step 2 below.
2. Fill in and submit the application form at: https://forms.gle/1mS6AWGSAnGh4hNM7. You should have completed your entrance task (point 1 above) before submitting the form, since you need to provide a link to it in the form.
3. Submit a proposal on the GSoC platform (https://summerofcode.withgoogle.com). You can base this on the list of proposed projects (see below), your entrance task, or your own independent idea - whichever you choose, we aim to evaluate fairly and primarily on quality. If you submit a draft proposal, we are happy to provide feedback before the final submission. For general advice on how to write the proposal, have a look at the official guide: https://google.github.io/gsocguides/student/writing-a-proposal.

The application deadline for completing all three steps above is April 13, 19:00 (WEST). 

If you get stuck or have questions, please feel free to reach out to us on Gitter (https://gitter.im/sktime/community) or GitHub (https://github.com/alan-turing-institute/sktime/discussions). 

## What we expect
GSoC is a marathon, not a sprint, and we expect good performance over the whole project. This means that you are in daily contact with your mentors and wider community and that you work full time on the project. 

In addition to the individual project work, all students will be required (and have the opportunity) to:

 * peer-review a fellow student's work in the middle and at the end of GSoC,
 * write weekly blog posts about your contribution and a final summary post at the end of the project,
 * have a good time web-socializing with the other students.

## What you can expect to get out of your participation

The stipend will allow you to aquire cutting edge skills and participate in intensive mentoring sessions, in highly sought-after areas of data science (time series, toolboxes, healthcare & industry applications). 

Ultimately, one of our key goals is to onboard new *long-term* developers who are willing to step up and become next generation leaders in open source toolbox development.

## Candidate selection process
A pre-selection will be carried out for applications submitted by April 13 based on the submitted application form and linked material. You will receive notification of the pre-selection outcome no later than April 20.

The outcome of the pre-selection can be either progression to the next stage, or a rejection. In the latter case, we would still very much welcome collaboration and contribution outside GSoC. For example, you may be eligible for (unpaid) mentoring.

If successful in the pre-selection, we will invite you to a structured interview (ca. 60 minutes length) with core community members of sktime, in the weeks of April 19 or 26.
Preferred dates are April 23 and 30. Please keep these dates free if possible.

During the interview, you will be expected to give a 10-minute presentation on a piece of Python code that you wrote. The interview will also focus on your motivation to join sktime, prior work experience, suitability for the specified project, and general technical background in data science and Python software development. 

The interview can have the following three outcomes:
* Conditional fast-track acceptance to the sktime GSoC 2021. This means you are put on-track by the sktime project, and in a project dedicated slot for the GSoC program, and accepted subject to subsequent confirmation by INCF/GSoC. This means highly likely - but not guaranteed - acceptance to the GSoC program, but can still result in a rejection (see below)
* Conditional acceptance to the sktime GSoC 2021. This means you are put on-track by the sktime project, but in one of the pooled slots for the INCF/GSoC program. This means possible - but not guaranteed - acceptance to the GSoc program, but can still result in a rejection (see below).
* A rejection for GSoC 2021. This means you are not put forward to any of the GSoC 2021 slots by the sktime team - but we would still very much welcome collaboration and contribution, outside of GSoC 2021, if you are interested.

The interview outcome will be communicated to you no later than one week after the interview itself. You will receive full confirmation of acceptance or rejection (from sktime and INCF/GSoC) on May 17.

## What we are looking for
We're actively looking for contributors and your help is extremely welcome. Therefore, if
 * you are interested in time series, machine learning (ML), statistics, API design and software architecture,
 * you like coding in Python,
 * you are familiar with the basic data science ecosystem in Python, including numpy, pandas and scikit-learn, 
 * you enjoy working with a vibrant team of experienced ML scientists and software engineers,
 * you always wanted to join an open-source community,

then GSoC with sktime is for you! You'll spend the summer working with our enthusiastic and open-minded team of developers who are creating one of the first comprehensive time series ML toolboxes out there.

## Projects
Please find below a list topics to help you get started. But please don't hesitate to propose your own topic to work on. Please check out our [development roadmap](https://github.com/alan-turing-institute/sktime/issues/228) and [good first issues](https://github.com/alan-turing-institute/sktime/labels/good%20first%20issue) to get an idea of the topics we're working on. 

You can find an overview of the project ideas [here](https://docs.google.com/document/d/14wnNV-cIqTIF3eE9QJXtkwyW7lQomUiCLVVPFafX6Js/edit?ts=5ffda09e).

### Software engineering projects 
| Title | Mentors | Short Description  | Difficulty | What you need to know |
|---|---|---|---|---|
| **Time series regression** |  @mloning | Refactoring classifiers into regressor | beginner | Regression with scikit-learn |
| **Time series clustering** | @TonyBagnall | Implementing time series clustering algorithm using time series distances | beginner | Clustering with scikit-learn |
| **Forecasting** | @mloning  | Implementing algorithms for model selection, composition and reduction | medium |
| **Develop a framework** | @fkiraly | Annotation tasks, multi-sample forecasting tasks, event modelling tasks, probabilistic tasks; check out our [enhancement proposal](https://github.com/sktime/enhancement-proposals) to find out more about the design process  | ambitious :-) | 

### Applied neuroscience projects
#### Project 1: Classification using EEG 
Mentor: @TonyBagnall

Electroencephalograms (EEG) and magnetoencephalography (MEG) are techniques for measuring, directly or indirectly, actual or relative changes in voltage throughout the body. This type of time series data is often related to classification problems. EEG and MEG are also central to human computer interface research. The question we wish to address on this project is, what is the best way to make predictions from ECG/EEG and MEG? We will treat the problem as time series classification. We have an existing database of publicly available labelled EEG/MEG datasets, tools in both Python for time series classification and collaborators who are expert in traditional techniques for analysing EEG/MEG. Our ultimate goal is an effective automated end-to-end pipeline for EEG/MEG classification using open source software such as sktime. This would encourage reproducible research in the field and facilitate more widespread analysis. This ten week project will contribute to this goal and will involve three phases. The first will involve implementation of a pipeline benchmark approach of feature extraction and standard classification. This will require standard toolkits for features such as wavelets as soft dependencies in sktime and the evaluation of existing techniques with a range of transformation/scikit-learn  classifier combinations. The second phase will involve the development of existing time series classification algorithms to work directly with EEG data. The final phase will be to help construct and manage an experimental scheme to compare the performance of a range of algorithms on problems of this kind.   
 
#### Project 2: Detecting Early Onset Dementia
Mentor: @TonyBagnall

Sea Hero Quest (SHQ) is a citizen science project which uses gamification as a means to collect large scale data for future use in preclinical dementia diagnosis. SHQ has to date collected data from 4.5 million healthy people worldwide. In addition, our collaborator Prof. Hornberger has patient cohort data on the game. The game itself collects basic demographic and level outcome measures, and trajectory data (position, heading direction) for each player in each level is collected every 500ms. This fully anonymised data can potentially be used to predict the risk of early onset of dementia through trajectory information. This project will involve developing a direct interface the SHQ game so that we can develop tools to process data and ultimately, attempt to make predictions. 

## Mentors

| Name  | GitHub | Website |
|---|---|---|
| Franz Király | [@fkiraly](https://github.com/fkiraly) | [website](https://www.ucl.ac.uk/statistics/people/franz-kiraly) |
| Markus Löning   | [@mloning](https://github.com/mloning) | | 
| Martina Vilas | [@martinagvilas](https://github.com/martinagvilas) | [website](https://martinagvilas.github.io) | 
| Nina Miolane | [@ninamiolane](https://github.com/ninamiolane/) | [website](https://www.ninamiolane.com) |
| Tony Bagnall | [@TonyBagnall](https://github.com/TonyBagnall) | [website](http://www.timeseriesclassification.com/index.php)  |
