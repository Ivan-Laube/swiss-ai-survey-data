# swiss-ai-survey-data

Anonymized aggregate results from the [Swiss AI Deployment Resource](https://aicompliant.ch) adoption survey.

`survey-aggregates.json` is written automatically by a weekly Cloudflare
Worker cron job (see [`workers/survey`](https://github.com/Ivan-Laube/swiss-ai-resource/tree/main/workers/survey)
in the main repo). It contains only counts aggregated across respondents,
with any cell below 5 responses suppressed — never individual answers.

This repo is separate from the main site repo so the Worker's write
credential is scoped to just this data file, not the whole site.
Read at [aicompliant.ch/de/benchmark/](https://aicompliant.ch/de/benchmark/).
