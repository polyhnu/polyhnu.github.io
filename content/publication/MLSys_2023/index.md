---
title: 'SIRIUS: Harvesting Whole-Program Optimization Opportunities for DNNs'

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
  - Yijin Li
  - Jiacheng Zhao
  - Qianqi Sun
  - Haohui Mai
  - Lei Chen
  - Wanlu Cao
  - Yanfan Chen
  - Zhicheng Li
  - Ying Liu
  - Xinyuan Zhang
  - Xiyu Shi
  - Jie Zhao
  - Jingling Xue
  - Huimin Cui
  - Xiaobing Feng
# Author notes (optional)
author_notes:
  - 'Equal contribution'
  - 'Equal contribution'
  - ''
  - ''
  - ''
  - ''
  - ''
  - ''
  - 'Corresponding author'
  - ''
  - ''
  - ''
  - ''
  - ''
  - ''

date: '2023-11-01T00:00:00Z'
doi: ''

# Schedule page publish date (NOT publication's date).
publishDate: '2023-11-01T00:00:00Z'

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ['paper-conference']

# Publication name and optional abbreviated publication name.
publication: In *Proceedings of Machine Learning and Systems*
publication_short: In *MLSys 2023*
ccf_rank: Non-CCF

abstract: As emerging applications are rapidly moving to accelerators, a greatdeal of research has been proposed to improve the performance of the accelerators. For the AI applications, fruitful software-driven research has been focused on proposing new programming languages, new kernel fusion heuristics,new optimization tuning approaches, and new software execution engines. However, how to leverage classical compiler optimizations to generate efficient code is an overlooked aspect of performance. In this paper, we propose a whole-program analysis and optimization compiler framework, SIRIUS, to uniformly model the host and kernel computations in a unified polyhedral representation and,further, seek maximal fusion opportunities from the global view so that the fused kernel can benefit from classical optimizations. Evaluations over representative DNN models demonstrate that SIRIUS can achieve up to 11.98x speedup over TensorRT, and 154.84x speedup over TensorFlow. In particular, for BERT, SIRIUS can achieve 1.46x speedup over TensorRT.

# Summary. An optional shortened abstract.
summary: In *Proceedings of Machine Learning and Systems (MLSys 2023)*

tags: []

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://proceedings.mlsys.org/paper_files/paper/2023/file/3e4e24f7e055320fa54c03f6e816775f-Paper-mlsys2023.pdf'
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
