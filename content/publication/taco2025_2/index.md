---
title: 'ASSG: Enhanced Workload Balancing via Adaptive State Scheduling Granularity Approach for Stateful Distributed Stream Processing'

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
  - Jiawei Tan
  - Jiapeng Zhang
  - Zhuo Tang
  - Xiong Xiao
  - Bingting Jiang
  - Jie Zhao
  - Kenli Li

# Author notes (optional)
author_notes:
  - ''
  - ''
  - ''
  - ''
  - ''
  - ''
  - ''


date: '2025-12-13T00:00:00Z'
doi: ''

# Schedule page publish date (NOT publication's date).
publishDate: '2025-12-13T00:00:00Z'
# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ["article-journal"]

# Publication name and optional abbreviated publication name.
publication: "ACM Transactions on Architecture and Code Optimization "
publication_short: In *TACO 2025*
ccf_rank: A

abstract: The dynamic changes in the distribution of data attributes within the data stream lead to unbalanced workloads in stream processing operators, often necessitating state migration in these operators. However, significant time overhead associated with state migration results in latency peaks and interruptions in stream applications. Ignoring the impact of state scheduling granularity exacerbates the time overhead during migration. Focusing on state migration efficiency, this article presents the Adaptive State Scheduling Granularity (ASSG) approach for stateful distributed stream processing. The ASSG conducts dynamic workload balancing at the granularity of state subgroups, where the number and size of any subgroup can be adaptively adjusted to reduce the time of collecting workloads and generating balancing plans. Moreover, since the idle instances may experience higher workloads than average due to receiving the migrated states, we propose a parallel migration strategy. They are enabled to post low states to other instances while receiving the high ones, alleviating the workload imbalance without extending migration duration. ASSG has been fully implemented on Apache Flink, which demonstrates a 23.84% reduction in average latency compared to state-of-the-art workload balancing schemes and achieves at least a 10.91% reduction in the time required for state migration through adaptive granularity adjustment..

# Summary. An optional shortened abstract.
summary: "ACM Transactions on Architecture and Code Optimization "

tags:
- Source Themes
featured: false

# links:
# - name: ""
#   url: ""
url_pdf: 'https://dl.acm.org/doi/10.1145/3776583'
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
