---
title: 'Eiffel: Inferring Input Ranges of Significant Floating-point Errors via Polynomial Extrapolation'

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
  - Zuoyan Zhang
  - Bei Zhou
  - Jiangwei Hao
  - Hongru Yang
  - Mengqi Cui
  - Yuchang Zhou
  - Guanghui Song
  - Fei Li
  - Jinchen Xu
  - Jie Zhao
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
  - 'Corresponding author'
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
publication: In *Proceedings of the 38th IEEE/ACM International Conference on Automated Software Engineering*
publication_short: In *ASE 2023*
ccf_rank: A

abstract: Existing search heuristics used to find input values that result in significant floating-point (FP) errors or small ranges that cover them are accompanied by severe constraints, complicating their implementation and restricting their general applicability. This paper introduces an error analysis tool called Eiffel to infer error-inducing input ranges instead of searching them. Given an FP expression with its domain D , Eiffel first constructs an error data set by sampling values across a smaller domain R and assembles these data into clusters. If more than two clusters are formed, Eiffel derives polynomial curves that best fit the bound coordinates of the error-inducing ranges in R , extrapolating them to infer all target ranges of D and reporting the maximal error. Otherwise, Eiffel simply returns the largest error across R . Experimental results show that Eiffel exhibits a broader applicability than Atomu and S<sup>3</sup> FP by successfully detecting the errors of all 70 considered benchmarks while the two baselines only report errors for part of them. By taking as input the inferred ranges of Eiffel, Herbie obtains an average accuracy improvement of 3.35 bits and up to 53.3 bits.

# Summary. An optional shortened abstract.
summary: In *Proceedings of the 38th IEEE/ACM International Conference on Automated Software Engineering (ASE 2023)*

tags: []

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://www.computer.org/csdl/proceedings-article/ase/2023/299600b441/1SBGuFStnZ6'
url_code: 'https://github.com/zuoyanzhang/Maxfpeed'
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
