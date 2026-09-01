---
title: 'Parallelizing Neural Network Models Effectively on GPU by Implementing Reductions Atomically'

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
  - Jie Zhao
  - Cédric Bastoul
  - Yanzhi Yi
  - Jiahui Hu
  - Wang Nie
  - Renwei Zhang
  - Zhen Geng
  - Chong Li
  - Thibaut Tachon
  - Zhiliang Gan
# Author notes (optional)
author_notes:
  - 'Corresponding author'
  - ''
  - ''
  - ''
  - ''
  - ''
  - ''
  - ''
  - ''
  - ''

date: '2022-09-01T00:00:00Z'
doi: ''

# Schedule page publish date (NOT publication's date).
publishDate: '2022-09-01T00:00:00Z'

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ['paper-conference']

# Publication name and optional abbreviated publication name.
publication: In *Proceedings of 31st International Conference on Parallel Architectures and Compilation Techniques*
publication_short: In *PACT 2022*
ccf_rank: B

abstract: Due to the missing of a good orchestration of loop transformations, existing optimizing compilers for deploying neural networks on GPU either parallelize reductions ineffectively or miss the fusion opportunities with other operators. Neural network models thus exhibit sub-optimal performance on GPU. We present a practical approach called Panamera for the effective parallelization of reductions in neural networks on GPU. Panamera first leverages loop coalescing to flatten the loop dimensions of reductions, converting all reduction operators into canonical forms eligible for the polyhedral model. Next, Panamera uses polyhedral transformations to reduce the data movements caused by unfused reductions and perform multi-block hardware binding not considered by many compilers. Finally, Panamera embeds a highly optimized routine implemented using GPU atomic instructions, further improving the performance of neural network models while guaranteeing the correctness of parallel reductions. The experimental results demonstrate the effectiveness of our approach：for single operators our code obtains a mean speedup of 33.7×, 3.5×, 5.4× and 9.6× over cuDNN, CUB, TVM and Ansor, for sub-graphs our approach outperforms cuDNN, TVM and Ansor by 9.5×, 2.6× and 2.7×, and for end-to-end workloads, a tensor compiler integrated with our approach outperforms them by 122.5%, 19.3% and 15.2%.

# Summary. An optional shortened abstract.
summary: In *Proceedings of 31st International Conference on Parallel Architectures and Compilation Techniques (PACT 2022)*

tags: []

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://dl.acm.org/doi/10.1145/3559009.3569656'
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
