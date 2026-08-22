---
title: 'Memory-Safe Hierarchical Planning for Hybrid-Parallel Transformer Training'

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
  - Zuoyan Zhang
  - Zhiqiang Zhang
  - Nanqin Wang
  - Jinyi Wang
  - Jie Zhao

# Author notes (optional)
author_notes:
  - ''
  - ''
  - ''
  - ''
  - ''

date: '2026-08-22T00:00:00Z'
doi: '10.1145/3842760'

# Schedule page publish date (NOT publication's date).
publishDate: '2026-08-22T00:00:00Z'

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ['article-journal']

# Publication name and optional abbreviated publication name.
publication: 'ACM Transactions on Architecture and Code Optimization'
publication_short: 'In *TACO 2026*'

abstract: >-
  Training decoder-style Transformer models at scale requires composing data,
  tensor, pipeline, context, and, for sparse models, expert parallelism under
  tight device memory limits. Without a reliable pre-profiling admission model,
  algebraically legal but memory-infeasible configurations can consume
  profiling budget without yielding useful throughput measurements. Choosing a
  pipeline degree also leaves a structured layer-to-stage mapping problem
  unresolved. This paper presents Shockwave, a hierarchical planner that
  operates through the exposed launcher and partition interfaces of
  Megatron-style dense and sparse Transformer runtimes. Shockwave first builds
  a conservative memory-feasible region with an analytical model and
  backend-calibrated safety margins. It then profiles a balanced baseline and a
  few single-dimension anchors to learn which parallel degrees improve
  throughput most on the target runtime and uses that ranking to select a
  global strategy. Finally, it solves a mixed-integer program for stage-aware
  layer allocation under a fixed 1F1B pipeline schedule. Implemented as a thin
  control layer on top of Megatron-LM and MindSpeed, Shockwave matches or
  exceeds expert-curated plans, achieving geometric mean throughput gains of
  1.08x over expert-tuned Megatron hybrid configurations on GPUs and 1.04x over
  expert MindSpeed recipes on NPUs. Relative to the evaluated automatic
  baselines, it improves throughput by 1.33x on GPUs and 1.10x on NPUs while
  reducing configuration search time by 4.59x and 5.60x.

# Summary. An optional shortened abstract.
summary: 'ACM Transactions on Architecture and Code Optimization'

tags: []
featured: false

url_pdf: 'https://doi.org/10.1145/3842760'
url_code: ''
url_dataset: ''
url_poster: ''
url_project: ''
url_slides: ''
url_source: ''
url_video: ''

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects: []

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: ''
---
