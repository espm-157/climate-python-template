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

This year the module has a second thread running through it. You have a language model
that will write the parsing code for you, and it is good at it. It is also wrong in
specific, recurring ways that produce code which runs cleanly and gives the wrong answer.
Each part of the notebook pairs a climate data set with one of those failure modes:
mislabeled columns, sentinel values read as real measurements, one file loaded out of
twelve, a variable chosen by string match rather than by meaning, and a default library
that cannot handle the size of the data. The recurring question is the one scientists have
always had to answer about code they did not write:

> How do I know these numbers are right?

## Data sources

- NOAA Mauna Loa CO2 record — <https://gml.noaa.gov/webdata/ccgg/trends/co2/co2_mm_mlo.txt>
- NSIDC Arctic sea ice extent (G02135) — <https://nsidc.org/data/G02135>
- EXIOBASE 3, cloud-optimized Parquet — <https://source.coop/youssef-harby/exiobase-3>
- Our World in Data CO2 — <https://github.com/owid/co2-data>
- Vostok ice core — <https://doi.org/10.3334/CDIAC/ATG.009>

## Language models

We use open-weight models hosted by the [National Research Platform](https://nrp.ai).
Register your own account and generate a token at <https://nrp.ai/llmtoken>, then set:

```bash
export OPENAI_BASE_URL="https://ellm.nrp-nautilus.io/v1"
export OPENAI_API_KEY="your-nrp-token"
export OPENAI_MODEL="deepseek-v4-flash"
```

Reading the endpoint from the environment rather than hardcoding it is deliberate. These
are OpenAI-compatible APIs, so the same code runs against a different provider by changing
these three values and nothing else. That portability is a property of open infrastructure,
and it is worth noticing that closed systems generally do not offer it.

**We work in plan mode this module.** You review and approve what the model proposes before
it runs. Autonomous modes come later in the course.

## Setup

- Use the [github-login.ipynb](github-login.ipynb) notebook in JupyterLab to authenticate each session with GitHub.  This provides a short-lived and appropriately scoped token for secure access using `gh-scoped-creds`.
- We use GitHub Actions to run automated reproducibility checks, click the badge up top for details.

## Links

[🌐 Course Website](https://espm-157.carlboettiger.info/)
