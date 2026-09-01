---
title: 'Arfa: an Agile Regime-based Floating-point Optimization Approach for Rounding Errors'

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
  - Jinchen Xu
  - Mengqi Cui
  - Fei Li
  - Zuoyan Zhang
  - Hongru Yang
  - Bei Zhou
  - Jie Zhao
# Author notes (optional)
author_notes:
  - 'Equal contribution'
  - 'Equal contribution'
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
publication: In *Proceedings of the 33rd ACM International Symposium on Software Testing and Analysis*
publication_short: In *ISSTA 2024*
ccf_rank: A

abstract: Recent approaches present the concept of regimes to partition the input domain D of a floating-point expression f_e, rewriting it in each regime where f_e shows larger errors such that the accuracy across D can be improved. These methods, however, fall short of both inferring regimes and searching rewrite substitutions.In this paper, we introduce a rewriting system called Arfa to address these issues. Given an f_e and its D, Arfa first seeks a rewrite substitution f_o that has lower errors across D and next plots the error distribution of f_o. The boundary line of this plot is then sketched, based on which an effective regime inference algorithm applicable to both numerically stable and unstable programs is implemented. For each regime where f_o should be rewritten, Arfa first normalizes f_o  by considering the regime’s properties and next generates an incomplete set of f_o ’s rewrite candidates, which are prioritized according to the number of floating-point operators. Finally, Arfa selects the best rewrite substitution by empirically inspecting the errors of several top ranked rewrite candidates, with enhancing precision also considered as a complementary strategy. This search heuristic avoids the need to establish a cost model used by prior work.We conduct experiments using 60 benchmarks, including 56 FPbench examples and four real-life programs. The results demonstrate that Arfa can reduce both maximum and average errors of the original expressions by 4.73 and 2.08 bits on average, and up to 33 and 16 bits, respectively; the experimental outcomes also show that Arfa exhibits lower errors, sometimes to a significant degree, than Herbie, PSAT (a global optimization framework that rewrites numerical programs via prioritized stochastic algebraic transformations), Daisy, and Regina.

# Summary. An optional shortened abstract.
summary: In *Proceedings of the 33rd ACM International Symposium on Software Testing and Analysis (ISSTA 2024)*

tags: []

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://papers.ssrn.com/sol3/papers.cfm?abstract_id=4511969'
url_code: 'https://github.com/yuanyuanxia/exprAuto'
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
<!-- 
{{% callout note %}}
Click the _Cite_ button above to demo the feature to enable visitors to import publication metadata into their reference management software.
{{% /callout %}}

{{% callout note %}}
Create your slides in Markdown - click the _Slides_ button to check out the example.
{{% /callout %}}

Add the publication's **full text** or **supplementary notes** here. You can use rich formatting such as including [code, math, and images](https://docs.hugoblox.com/content/writing-markdown-latex/). -->
