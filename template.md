Mentorship Programme Notes: SINEM KILICDERE MOSCHOS
===

###### tags: `mentorship`

This is a collaborative document to keep track of progress during the mentorship programme.

:::info
- **Call time**: 30min time slot, day of week
- **Project name**: SKTIME	
- **Mentees**: SINEM KILICDERE MOSCHOS
- **Mentor(s)**: FRANZ KIRALY, DAMIR TEMIR
- **Call joining link**: Discord Channel
:::


## References
The sktime mentorship programme is inspired by the [The Turing Way](https://book.the-turing-way.org/) project and [Open Life Science](https://openlifesci.org) programme under a CC BY 4.0, Open Life Science (OLS-2), 2020 license.


**Contents**

[TOC]

## Week 0

- For reference: sktime's [mentorship programme call for applications](https://www.sktime.net/en/latest/get_involved/mentoring.html)
- Get started with HackMD using this short guide: https://hackmd.io/@openlifescience/OLS-HackMD-guide
- Please read our [Code of Conduct](https://www.sktime.net/en/latest/get_involved/code_of_conduct.html)
- [guide for getting started as an sktime contributor](https://www.sktime.net/en/latest/get_involved/contributing.html#contributing)
- [current list of project ideas](https://github.com/sktime/mentoring/blob/main/internships/projects_2023.md)
- Check out sktime's [development roadmap](https://github.com/sktime/sktime/issues/228)

**Preferred time and days provided by the mentor and mentee**

Please indicate your preferred day/time for your regular call:

Monday to Friday 13:00 to 20:00 UTC

### Prep work for week 1

**Mentees will:**

1. Read https://ideas.ted.com/are-you-mentorable/
2. Set 1-2 personal development goals for yourself:
Improve open-source contribution skills, especially through testing and documentation.
Learning more about time series forecasting and ML workflows.
3. State how your mentors can best support you in your contribution to sktime (e.g., providing code reviews, share useful resources, explain ML concepts):
I would definitely benefit from regular code reviews, pointers to useful parts of the codebase, and help understanding technical decisions in sktime issues

4. Open an issue on the [sktime/mentoring](https://github.com/sktime/mentoring/issues) repo. This can be updated during the mentorship program.



## Week 1 - 07/14/2025

### Agenda
* discussing aim of mentoring
* how sktime mentoring programme works
* discussing project to work on & next steps
* developer set-up

### Notes
We introduced ourselves and went over the sktime mentorship goals
Franz and Damir explained the structure of sktime and possible contribution areas
### development goals
Understand how sktime organizes, finding beginnner friendly issues and sending PR and rest

### project goals
Set up dev environment and run local tests. Contribute with mentors. Being part of open source project

## Week 2 - 07/21/2025

### work done
Changelog Generator= created a script to fetch merged PRs, group by label. Tested on sktime’s repo and added options for label grouping.
FCNClassifier=Understood why it was in EXCLUDED_TESTS. Updated tags and ran the estimator test suite. All tests pass locally ready for removal from EXCLUDED_TESTS.

### Agenda
Reviewing changelog output and label handling.
Confirm FCNClassifier is ready to include in standard tests.
Also planning to work on new issue #4303.

### Questions
Group by date or version?
Do I need to test GPU/CPU separately?

### Notes
Mentors said the changelog labels should follow a clear order.
The FCNClassifier tests are passing and look good to include.

### Actions, short-term goals
Hopefully, All PRs will be merged
Started a new issue for the next contribution.
Meet with mentors to decide what the new task will be and understand sktime better

## Week 3 - MMM DD

### work done
Changelog Generator = Finalized cleaning formatting and section order.Cleaned PR from unrelated files and commits.
FCNClassifier = Removed from EXCLUDED_TESTS after confirming all local tests pass. Submitted a PR to finalize.
Issue #4303 docstring= Working on completing docstrings. Added formulas, clarified multioutput behavior, and formatted descriptions.
### Agenda
Final review for changelog generator PR.
emaining metrics for issue #4303.
### Questions
Can I propose new labels for changelog categories?
### Notes
advised not to shorten mathematical explanations unless needed.
Learned to differentiate between evaluate and evaluate_by_index in docstring descriptions
### Actions, short-term goals
Wrap up issue #4303 and get it reviewed
Attend upcoming mentor sync to pick next issue
