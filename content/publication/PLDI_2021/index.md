---
title: 'AKG: automatic kernel generation for neural processing units using polyhedral transformations'

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
  - Jie Zhao
  - Bojie Li
  - Wang Nie
  - Zhen Geng
  - Renwei Zhang
  - Xiong Gao
  - Bin Cheng
  - Chen Wu
  - Yun Cheng
  - Zheng Li
  - Peng Di
  - Kun Zhang
  - Xuefeng Jin
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
  - '' 
  - '' 
  - '' 

date: '2021-06-18T00:00:00Z'
doi: ''

# Schedule page publish date (NOT publication's date).
publishDate: '2021-06-18T00:00:00Z'

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ['paper-conference']

# Publication name and optional abbreviated publication name.
publication: In *Proceedings of the 42nd ACM SIGPLAN International Conference on Programming Language Design and Implementation*
publication_short: In *PLDI 2021*
ccf_rank: A

abstract: Existing tensor compilers have proven their effectiveness in deploying deep neural networks on general-purpose hardware like CPU and GPU, but optimizing for neural processing units (NPUs) is still challenging due to the heterogeneous compute units and complicated memory hierarchy.In this paper, we present AKG, a tensor compiler for NPUs. AKG first lowers the tensor expression language to a polyhedral representation, which is used to automate the memory management of NPUs. Unlike existing approaches that resort to manually written schedules, AKG leverages polyhedral schedulers to perform a much wider class of transformations, and extends the semantics of the polyhedral representation to combine complex tiling techniques and hierarchical fusion strategies. We also implement the domain-specific optimization of convolution in AKG. Moreover, to achieve the optimal performance, we introduce complementary optimizations in code generation, which is followed by an auto-tuner.We conduct extensive experiments on benchmarks ranging from single operators to end-to-end networks. The experimental results show that AKG can obtain superior performance to both manual scheduling approaches and vendor provided libraries. We believe AKG will cast a light on the follow-up compiler works on NPUs.

# Summary. An optional shortened abstract.
summary: In *Proceedings of the 42nd ACM SIGPLAN International Conference on Programming Language Design and Implementation (PLDI 2021)*

tags: []

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://dl.acm.org/doi/10.1145/3453483.3454106'
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
