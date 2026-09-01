# Climate Module

<!-- EDIT with your badge link -->
[![Reproducibility Check](https://github.com/espm-157/climate-python-template/actions/workflows/main.yml/badge.svg)](https://github.com/espm-157/climate-python-template/actions/workflows/main.yml)

## Team Members

🦸
🦹

## 🎓 Learning Objectives

:octocat: Use of GitHub  
:snake: Use of Jupyter Notebooks  
:abcd: Accessing tabular data  
📈 Data visualization  
🔍 Verifying code you did not write  
🗄 Working with data larger than memory  
🌡️ Become familiar with data on global climate change  

## 📖 Content Overview

[💻 Assignment template](climate.ipynb)  
[💯 Assignment rubric](rubric.md)  
[📊 Session 2 benchmarking exercise](benchmark.md)  

Individuals or teams will work through and adapt the questions presented in the climate
notebook to reproduce key indicators of climate change, similar to NASA's
<https://climate.nasa.gov/vital-signs>.  Our primary objective is to reproduce the famous
'hockey-stick' curve first reported in _Nature_ ([Mann et al 1998](https://doi.org/10.1038/33859 "Mann, M., Bradley, R. & Hughes, M. Global-scale temperature patterns and climate forcing over the past six centuries. Nature 392, 779–787 (1998). https://doi.org/10.1038/33859"))
using the most recent observations and most extensive ice core data.  Along the way we
will encounter many other datasets and learn about wrangling the diverse conventions in
tabular data.

A second thread runs through the module. You have a language model that will write the
parsing code for you, and it is good at it. It is also wrong in specific, recurring ways
that produce code which runs cleanly and gives the wrong answer. Each part of the notebook
pairs a climate data set with one of those failure modes. The notebook does not tell you
which; finding out is the assignment. The recurring question is the one scientists have
always had to answer about code they did not write:

> How do I know these numbers are right?

Every previous advance that made computing dramatically easier — screens over punchcards,
compilers over assembly, Python over C — led to more programming by more people, not less.
Efficiency gets spent on attempting more. That is why this module does not ask you to
memorize library syntax, and equally why it cannot be completed by pasting the assignment
into a model and typing "go". The work moves up a level rather than disappearing.

We work in plan mode throughout this module: you review and approve what the model
proposes before it runs.

## Data sources

- NOAA Mauna Loa CO2 record — <https://gml.noaa.gov/webdata/ccgg/trends/co2/co2_mm_mlo.txt>
- NSIDC Arctic sea ice extent (G02135) — <https://nsidc.org/data/G02135>
- EXIOBASE 3, cloud-optimized Parquet — <https://source.coop/youssef-harby/exiobase-3>
- Our World in Data CO2 — <https://github.com/owid/co2-data>
- Vostok ice core — <https://doi.org/10.3334/CDIAC/ATG.009>

## Setup

Environment setup, GitHub authentication, and language model configuration are covered on
the [course website](https://espm-157.carlboettiger.info/) rather than here, since those
mechanics are shared across all four modules and change faster than the assignments do.

We use GitHub Actions to run automated reproducibility checks — click the badge up top for
details.

## Links

[🌐 Course Website](https://espm-157.carlboettiger.info/)
