---
title: 'Flextended Tiles: A Flexible Extension of Overlapped Tiles for Polyhedral Compilation'

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
  - Jie Zhao
  - Albert Cohen

# Author notes (optional)
author_notes:
  - 'INRIA 8 DI, École Normale Supérieure'
  - 'Google'


date: '2019-12-17T00:00:00Z'
doi: ''

# Schedule page publish date (NOT publication's date).
publishDate: '2019-12-17T00:00:00Z'

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ["article-journal"]

# Publication name and optional abbreviated publication name.
publication: "ACM Transactions on Architecture and Code Optimization "
publication_short: In *TACO 2019*
ccf_rank: A

abstract: Loop tiling to exploit data locality and parallelism plays an essential role in a variety of general-purpose and domain-specific compilers. Affine transformations in polyhedral frameworks implement classical forms of rectangular and parallelogram tiling, but these lead to pipelined start with rather inefficient wavefront parallelism. Multiple extensions to polyhedral compilers evaluated sophisticated shapes such as trapezoid or diamond tiles, enabling concurrent start along the axes of the iteration space; yet these resort to custom schedulers and code generators insufficiently integrated within the general framework. One of these modified shapes referred to as overlapped tiling also lacks a unifying framework to reason about its composition with affine transformations; this prevents its application in general-purpose loop-nest optimizers and the fair comparison with other techniques. We revisit overlapped tiling, recasting it as an affine transformation on schedule trees composable with any affine scheduling algorithm. We demonstrate how to derive tighter tile shapes with less redundant computations. Our method models the traditional “scalene trapezoid” shapes and novel “right-rectangle” variants. It goes beyond the state of the art by avoiding the restriction to a domain-specific language or introducing post-pass rescheduling and custom code generation. We conduct experiments on the PolyMage benchmarks and iterated stencils, validating the effectiveness and applicability of our technique on both general-purpose multicores and GPU accelerators.

# Summary. An optional shortened abstract.
summary: "ACM Transactions on Architecture and Code Optimization "

tags:
- Source Themes
featured: false

# links:
# - name: ""
#   url: ""
url_pdf: 'https://dl.acm.org/doi/10.1145/3369382'
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
