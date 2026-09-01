---
title: 'Apollo: Automatic Partition-based Operator Fusion through Layer by Layer Optimization'

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
  - Jie Zhao
  - Xiong Gao
  - Ruijie Xia
  - Zhaochuang Zhang
  - Deshi Chen
  - Lei Chen
  - Renwei Zhang
  - Zhen Geng
  - Bin Cheng
  - Xuefeng Jin
# Author notes (optional)
author_notes:
  - 'Corresponding author'
  - ''
  - ''
  - ''
  - ''
  - 'Corresponding author'
  - ''
  - ''
  - ''
  - 'Corresponding author'

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
publication_short: In *MLSys 2022*
ccf_rank: Non-CCF

abstract: We study fusion for deep neural networks (DNNs) in a just-in-time (JIT) compilation framework Apollo. It considers both memory- and compute-bound tensor operators for fusion, and integrates graph-level node grouping and operator-level loop fusion closely, widening the fusion search space. Apollo enables the upward feedback from the downstream loop optimizer, enforcing the graph engine to regenerate partition patterns amenable to the downstream pass and thus resolving the scalability issue. Besides data locality, Apollo also exploits the parallelism between independent tensor operators, further improving the performance of DNN workloads. Experimental results on training workloads show that Apollo outperforms TensorFlow and XLA by 1.86× and 1.37× on a single GPU, and 1.96× and 1.18× on multiple GPUs. Apollo also improves the performance of a vendor-provided DNN framework by 19.7% on a domain-specific accelerator. In addition, the results of inference workloads demonstrate the general applicability of our fusion framework.

# Summary. An optional shortened abstract.
summary: In *Proceedings of Machine Learning and Systems (MLSys 2022)*

tags: []

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://proceedings.mlsys.org/paper_files/paper/2022/hash/e175e8a86d28d935be4f43719651f86d-Abstract.html'
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
