---
title: 'Dual-Pronged Deep Learning Preprocessing on Heterogeneous Platforms With CPU, Accelerator and CSD'

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
  - Jia Wei
  - Xingjun Zhang
  - Witold Pedrycz
  - Longxiang Wang
  - Jie Zhao

# Author notes (optional)
author_notes:
  - ''
  - ''
  - ''
  - ''
  - ''


date: '2026-03-01T00:00:00Z'
doi: ''

# Schedule page publish date (NOT publication's date).
publishDate: '2026-03-01T00:00:00Z'
# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ["article-journal"]

# Publication name and optional abbreviated publication name.
publication: "IEEE Transactions on Computers"
publication_short: In *IEEE TC 2026*
ccf_rank: A

abstract: For image-related deep learning tasks, the first step often involves reading data from external storage and performing preprocessing on the CPU. As accelerator speed increases and the number of single compute node accelerators increases, the computing and data transfer capabilities gap between accelerators and CPUs gradually increases. Data reading and preprocessing become progressively the bottleneck of these tasks. Our work, DDLP, addresses the data computing and transfer bottleneck of deep learning preprocessing using Computable Storage Devices (CSDs). DDLP allows the CPU and CSD to efficiently parallelize preprocessing from both ends of the datasets, respectively. To this end, we propose two adaptive dynamic selection strategies to make DDLP control the accelerator to automatically read data from different sources. The two strategies trade-off between consistency and efficiency. DDLP achieves sufficient computational overlap between CSD data preprocessing and CPU preprocessing, accelerator computation, and accelerator data reading. In addition, DDLP leverages direct storage technology to enable efficient SSD-to-accelerator data transfer. In addition, DDLP reduces the use of expensive CPU and DRAM resources with more energy-efficient CSDs, alleviating preprocessing bottlenecks while significantly reducing power consumption. Extensive experimental results show that DDLP can improve learning speed by up to 23.5% on ImageNet Dataset while reducing energy consumption by 19.7% and CPU and DRAM usage by 37.6%. DDLP also improves the learning speed by up to 27.6% on the Cifar-10 dataset.

# Summary. An optional shortened abstract.
summary: "IEEE Transactions on Computers (TC 2026)"

tags:
- Source Themes
featured: false

# links:
# - name: ""
#   url: ""
url_pdf: 'https://ieeexplore.ieee.org/document/11318138'
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
