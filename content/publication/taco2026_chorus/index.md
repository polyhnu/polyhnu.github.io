---
title: 'Global Scheduling of Transient Parameter Materialization for Sharded Training'

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
  - Zuoyan Zhang
  - Jinyi Wang
  - Zhuo Tang
  - Jie Zhao

# Author notes (optional)
author_notes:
  - ''
  - ''
  - ''
  - ''

date: '2026-08-06T00:00:00Z'
doi: '10.1145/3838601'

# Schedule page publish date (NOT publication's date).
publishDate: '2026-08-06T00:00:00Z'

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ['article-journal']

# Publication name and optional abbreviated publication name.
publication: 'ACM Transactions on Architecture and Code Optimization'
publication_short: 'In *TACO 2026*'

abstract: >-
  Parameter-sharded training reduces device-memory use by storing model
  parameters as shards and reconstructing full parameters only before the
  computations that consume them. This materialization is implemented through
  frequent all-gathers, which can become exposed waits in each forward-backward
  training iteration. Hiding these waits is not only a communication-volume
  problem. It requires deciding where to launch each all-gather and how long
  the materialized full-parameter buffer should remain live. All-gather
  prefetching can overlap communication with earlier computation but extends
  buffer lifetime. Retaining a buffer after its forward-pass use can eliminate
  a re-gather before backward-pass reuse, but consumes transient memory
  headroom needed by other materialization decisions. We present Chorus, a
  compiler-runtime framework for transient parameter materialization in
  memory-constrained sharded training. Chorus addresses a limitation of local
  runtime policies that make decisions at hooks, module boundaries, or
  configuration thresholds. They can issue individual prefetches or suppress
  individual releases, but they do not jointly compare future all-gather
  opportunities, buffer lifetimes, and memory-headroom conflicts across the
  iteration. Chorus lowers the forward and backward passes into a
  whole-iteration graph that makes all-gathers, use-site waits, and releases
  explicit. It then builds a profile-guided block model and solves a
  mixed-integer scheduling problem that jointly chooses all-gather launch
  positions and iteration-local retention decisions under time-varying memory
  headroom. The selected schedule is realized by graph rewriting, which moves
  communication while preserving use-site waits, fuses compatible prefetch
  operations, and removes redundant releases and re-gathers. Cross-iteration
  persistent retention is finalized during warmup using measured runtime
  memory behavior. We implement Chorus on top of torch.compile and evaluate it
  on 7B to 13B dense Transformer models and one MoE model across 4 to 16 A100
  GPUs. In the ZeRO-style stack, Chorus improves throughput by 1.10x over
  DeepCompile across the primary workloads. In the FSDP-style stack, the Chorus
  implementation on SimpleFSDP improves throughput by 1.14x over SimpleFSDP
  across the corresponding dense-model workloads. The benefits are greatest
  in network-constrained settings, where all-gather stalls are more exposed.
  Chorus stays within the configured memory budget and achieves a 1.35x
  compilation-time speedup over DeepCompile.

# Summary. An optional shortened abstract.
summary: 'ACM Transactions on Architecture and Code Optimization'

tags: []
featured: false

url_pdf: 'https://doi.org/10.1145/3838601'
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
