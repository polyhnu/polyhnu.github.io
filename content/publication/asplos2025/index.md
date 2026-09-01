---
title: 'Optimizing Deep Learning Inference Efficiency through Block Dependency Analysis'

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
  - Zhanyuan Di
  - Leping Wang
  - En Shao
  - Zhaojia Ma
  - Ziyi Ren
  - Feng Hua
  - Lixian Ma
  - Jie Zhao
  - Guangming Tan
  - Ninghui Sun

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
  - ''
  - ''

date: '2025-03-30T00:00:00Z'
doi: ''

# Schedule page publish date (NOT publication's date).
publishDate: '2025-03-30T00:00:00Z'

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ['paper-conference']

# Publication name and optional abbreviated publication name.
publication: In *Proceedings of the 30th ACM International Conference on Architectural Support for Programming Languages and Operating Systems*
publication_short: In *ASPLOS 2025*
ccf_rank: A

abstract: "Inter-operator optimization in deep neural networks (DNNs) relies on accurate data dependency analysis. Traditional machine learning compilers (MLCs) perform static data dependency analysis at the element and operator levels, leading to two key limitations: complex dependencies that hinder efficient inter-operator optimizations, and overlooked parallelizable computations that underutilize GPU resources. We introduce BlockDepend, a novel MLC framework that addresses these issues through block-level dependency analysis. By examining the lower-level phases of compilation, BlockDepend extracts crucial block-level dependency information, simplifying complex relationships between operators and uncovering hidden parallelization opportunities. This allows for targeted optimization strategies that enhance memory access efficiency and improve GPU utilization. Our experiments demonstrate BlockDepend's effectiveness, achieving speedups of 1.71× and 2.88× compared to NVIDIA TensorRT and AMD MIGraphX, respectively, across various workloads."

# Summary. An optional shortened abstract.
summary: In *Proceedings of the 30th ACM International Conference on Architectural Support for Programming Languages and Operating Systems (ASPLOS 2025)*

tags: []

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://dl.acm.org/doi/10.1145/3676641.3716264'
url_code: ''
url_dataset: ''
url_poster: ''
url_project: ''
# url_slides: 'https://yaozhujia.github.io/assets/pdf/cc2018-presentation.pdf'
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
