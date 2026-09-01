---
title: 'Post-Link Outlining for Code Size Reduction'

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
  - Shaobai Yuan
  - Jihong He
  - Yihui Xie
  - Feng Wang
  - Jie Zhao

# Author notes (optional)
author_notes:
  - ''
  - ''
  - ''
  - 'Corresponding author'
  - ''

date: '2024-12-24T00:00:00Z'
doi: ''

# Schedule page publish date (NOT publication's date).
publishDate: '2024-12-24T00:00:00Z'

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ['paper-conference']

# Publication name and optional abbreviated publication name.
publication: In *Proceedings of the ACM SIGPLAN 2025 International Conference on Compiler Construction*
publication_short: In *CC 2025*
ccf_rank: B

abstract: "This paper introduces PLOS, a novel post-link outlining approach designed to enhance code size reduction for resource-constrained environments. Built on top of a post-link optimizer BOLT, PLOS maintains a holistic view of the whole-program structure and behavior, utilizing runtime information while preserving standard build system flows. The approach includes a granular outlining algorithm that matches and replaces repeated instruction sequences within across modules and outlined functions, along with careful stack frame management to ensure correct function call handling. By integrating profiling information, PLOS balances the trade-off between code size and execution efficiency. The evaluation using eight MiBench benchmarks on an ARM-based Phytium FCT662 core demonstrates that PLOS achieves a mean code size reduction of 10.88% (up to 43.53%) and 6.61% (up to 14.78%) compared to LLVM’s and GCC’s standard optimization, respectively, 1.76% (up to 4.75%) over LLVM’s aggressive code size reduction optimizations, and 2.88% (up to 8.56%) over a link-time outliner. The experimental results also show that PLOS can achieve a favorable balance between code size reduction and performance regression."

# Summary. An optional shortened abstract.
summary: In *Proceedings of the ACM SIGPLAN 2025 International Conference on Compiler Construction (CC 2025)*

tags: []

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://conf.researchr.org/details/CC-2025/CC-2025-main-conference/14/Post-Link-Outlining-for-Code-Size-Reduction'
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
