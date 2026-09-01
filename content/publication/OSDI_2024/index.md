---
title: 'Enabling Tensor Language Model to Assist in Generating High-Performance Tensor Programs for Deep Learning'

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
  - Yi Zhai
  - Sijia Yang
  - Keyu Pan
  - Renwei Zhang
  - Shuo Liu
  - Chao Liu 
  - Zichun Ye
  - Jianmin Ji
  - Jie Zhao
  - Yu Zhang
  - Yanyong Zhang
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
  - 'Corresponding author'
  - 'Corresponding author' 

date: '2024-07-01T00:00:00Z'
doi: ''

# Schedule page publish date (NOT publication's date).
publishDate: '2024-07-01T00:00:00Z'

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ['paper-conference']

# Publication name and optional abbreviated publication name.
publication: In *Proceedings of the 18th USENIX Symposium on Operating Systems Design and Implementation*
publication_short: In *OSDI 2024*
ccf_rank: A

abstract: Obtaining high-performance tensor programs with high efficiency continues to be a substantial challenge. Approaches that favor efficiency typically limit their exploration space through heuristic constraints, which often lack generalizability. Conversely, approaches targeting high performance tend to create an expansive exploration space but employ ineffective exploration strategies.We propose a tensor program generation framework for deep learning applications. Its core idea involves maintaining an expansive space to ensure high performance while performing powerful exploration with the help of language models to generate tensor programs efficiently. We thus transform the tensor program exploration task into a language model generation task. To facilitate this, we explicitly design the language model-friendly tensor language that records decision information to represent tensor programs. During the compilation of target workloads, the tensor language model (TLM) combines knowledge from offline learning and previously made decisions to probabilistically sample the best decision in the current decision space. This approach allows more informed space exploration than random sampling commonly used in previously proposed approaches.Experimental results indicate that TLM excels in delivering both efficiency and performance. Compared to fully tuned Ansor/MetaSchedule, TLM matches their performance with a compilation speedup of 61×. Furthermore, when evaluated against Roller, with the same compilation time, TLM improves the performance by 2.25×.

# Summary. An optional shortened abstract.
summary: In *Proceedings of the 18th USENIX Symposium on Operating Systems Design and Implementation (OSDI 2024)*

tags: []

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://www.usenix.org/conference/osdi24/presentation/zhai'
url_code: 'https://github.com/zhaiyi000/tlm'
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
