---
title: 'A Decoupled Analytical Model for Tile Size Selection in Affine Programs'

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
  - Shihan Yuan
  - Zuoyan Zhang
  - Guanghui Song
  - Junhui Peng
  - Feng Wang
  - Zhuo Tang
  - Kenli Li
  - Jie Zhao

# Author notes (optional)
author_notes:
  - ''
  - ''
  - ''
  - ''
  - ''
  - ''
  - ''
  - ''

date: '2026-04-01T00:00:00Z'
doi: '10.1145/3806056'

# Schedule page publish date (NOT publication's date).
publishDate: '2026-04-01T00:00:00Z'

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ['article-journal']

# Publication name and optional abbreviated publication name.
publication: 'ACM Transactions on Architecture and Code Optimization'
publication_short: 'In *TACO 2026*'
ccf_rank: A

abstract: >-
  Existing tile size selection approaches are tightly coupled with compiler
  transformation pipelines, often leading to inaccurate modeling of cache
  behavior and limited effectiveness for non-rectangular tile shapes. This
  paper presents TileMind, a decoupled analytical model that combines
  compile-time and runtime information for tile size selection in affine
  programs. It introduces a transformation-aware pre-tiling step that enables
  the decoupled selector to remain consistent with compiler transformations
  while extracting compile-time metadata. The extracted metadata is then
  combined with profiled runtime characteristics to construct a richer yet
  tractable feasible domain, within which a nonlinear objective for tile size
  selection is formulated. This objective is subsequently transformed into a
  binary product linearization problem, with its nonlinear constraints also
  linearized for efficient optimization. Finally, an intra-tile optimization
  aligns computation with data layout to enhance data reuse within tiles.
  Across two multi-core Intel CPUs, TileMind achieves 1.49x (sequential) and
  1.33x (parallel) mean speedups on twenty PolyBench kernels, and 2.08--3.54x
  speedups on three deep learning workloads over the state-of-the-art
  analytical model Pluto-tss. Compared with TVM's latest autotuner
  MetaSchedule, TileMind delivers 1.35--1.46x mean speedups while reducing
  tuning overhead by 2--4 orders of magnitude. While demonstrating
  effectiveness on selecting tile sizes for non-rectangular tile shapes and
  compatibility with PPCG, Pluto, and TVM, we further provide proof-of-concept
  results on GPUs, illustrating the potential portability of TileMind across
  architectures.

# Summary. An optional shortened abstract.
summary: 'ACM Transactions on Architecture and Code Optimization (Just Accepted)'

tags: []
featured: false

url_pdf: 'https://doi.org/10.1145/3806056'
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
