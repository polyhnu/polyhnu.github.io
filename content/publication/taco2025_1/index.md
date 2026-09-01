---
title: 'Accelerating Parallel Structures in DNNs via Parallel Fusion and Operator Co-Optimization'

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
  - Zhanyuan Di
  - Leping Wang
  - Zhaojia Ma
  - En Shao
  - Jie Zhao
  - Ziyi Ren
  - Siyuan Feng
  - Dingwen Tao
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


date: '2025-09-18T00:00:00Z'
doi: ''

# Schedule page publish date (NOT publication's date).
publishDate: '2025-09-18T00:00:00Z'
# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ["article-journal"]

# Publication name and optional abbreviated publication name.
publication: "ACM Transactions on Architecture and Code Optimization "
publication_short: In *TACO 2025*
ccf_rank: A

abstract: Parallel structures have become a key pattern in deep neural networks (DNNs), offering improved efficiency and scalability. However, existing machine learning compilers (MLCs) face challenges in optimizing these structures due to limited parallel fusion scope and insufficient analysis of intra-operator characteristics. This article introduces Magneto, a framework designed to accelerate DNN inference by co-optimizing parallel operators. Magneto broadens the fusion scope and incorporates a specialized co-tuning algorithm to optimize operators jointly. Our approach addresses the unique challenges inherent in optimizing parallel structures, enabling significant performance improvements across various hardware platforms. Experimental results show that Magneto outperforms state-of-the-art NVIDIA TensorRT and AMD MIGraphX, achieving geometric mean speedups of 2.27× and 2.88×, respectively.

# Summary. An optional shortened abstract.
summary: "ACM Transactions on Architecture and Code Optimization "

tags:
- Source Themes
featured: false

# links:
# - name: ""
#   url: ""
url_pdf: 'https://dl.acm.org/doi/10.1145/3744906'
url_code: ''
url_dataset: ''
url_poster: ''
url_project: ''
url_slides: ''
url_source: ''
url_video: ''

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 

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
slides: example
---

<!-- {{% callout note %}}
Click the *Cite* button above to demo the feature to enable visitors to import publication metadata into their reference management software.
{{% /callout %}}

{{% callout note %}}
Create your slides in Markdown - click the *Slides* button to check out the example.
{{% /callout %}}

Add the publication's **full text** or **supplementary notes** here. You can use rich formatting such as including [code, math, and images](https://docs.hugoblox.com/content/writing-markdown-latex/). -->
