---
title: 'A Holistic Approach to Automatic Mixed-Precision Code Generation and Tuning for Affine Programs'

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
  - Jinchen Xu
  - Guanghui Song
  - Bei Zhou
  - Fei Li
  - Jiangwei Hao
  - Jie Zhao
# Author notes (optional)
author_notes:
  - 'Equal contribution'
  - 'Equal contribution'
  - ''
  - ''
  - ''
  - 'Corresponding author'

date: '2024-02-01T00:00:00Z'
doi: ''

# Schedule page publish date (NOT publication's date).
publishDate: '2024-02-20T00:00:00Z'

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ['paper-conference']

# Publication name and optional abbreviated publication name.
publication: In *Proceedings of the 29th ACM SIGPLAN Annual Symposium on Principles and Practice of Parallel Programming*
publication_short: In *PPoPP 2024*
ccf_rank: A

abstract: Reducing floating-point (FP) precision is used to trade the quality degradation of a numerical program's output for performance, but this optimization coincides with type casting, whose overhead is undisclosed until a mixed-precision code version is generated. This uncertainty enforces the decoupled implementation of mixed-precision code generation and autotuning in prior work. In this paper, we present a holistic approach called PrecTuner that consolidates the mixed-precision code generator and the autotuner by defining one parameter. This parameter is first initialized by some automatically sampled values and used to generate several code variants, with various loop transformations also taken into account. The generated code variants are next profiled to solve a performance model formulated using the aforementioned parameter, possibly under a pre-defined quality degradation budget. The best-performing value of the defined parameter is finally predicted without evaluating all code variants. Experimental results of the PolyBench benchmarks on CPU demonstrate that PrecTuner outperforms LuIs by 3.28× while achieving smaller errors, and we also validate its effectiveness in optimizing a real-life large-scale application. In addition, PrecTuner also obtains a mean speedup of 1.81× and 1.52×-1.73× over Pluto on single- and multi-core CPU, respectively, and 1.71× over PPCG on GPU.

# Summary. An optional shortened abstract.
summary: In *Proceedings of the 29th ACM SIGPLAN Annual Symposium on Principles and Practice of Parallel Programming (PPoPP 2024)*

tags: []

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://dl.acm.org/doi/10.1145/3627535.3638484'
url_code: 'https://github.com/sheenisme/lnlamp'
url_dataset: 'https://github.com/sheenisme?tab=repositories'
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
projects:
  - example

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: example
---

<!-- {{% callout note %}}
Click the _Cite_ button above to demo the feature to enable visitors to import publication metadata into their reference management software.
{{% /callout %}}

{{% callout note %}}
Create your slides in Markdown - click the _Slides_ button to check out the example.
{{% /callout %}}

Add the publication's **full text** or **supplementary notes** here. You can use rich formatting such as including [code, math, and images](https://docs.hugoblox.com/content/writing-markdown-latex/). -->
