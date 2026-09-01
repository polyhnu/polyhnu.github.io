---
title: 'Modeling the Interplay between Loop Tiling and Fusion in Optimizing Compilers Using Affine Relations'

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
  - Jie Zhao
  - Jinchen Xu
  - Peng Di
  - Wang Nie
  - Jiahui Hu
  - Yanzhi Yi
  - Sijia Yang
  - Zhen Geng
  - Renwei Zhang
  - Bojie Li
  - Zhiliang Gan
  - Xuefeng Jin
# Author notes (optional)
author_notes:
  - 'First author'
  - 'Corresponding author'
  - 'Corresponding author'
  - ''
  - ''
  - ''
  - ''
  - ''
  - ''
  - ''
  - ''
  - 'Corresponding author'
  
date: '2024-01-15T00:00:00Z'
doi: ''

# Schedule page publish date (NOT publication's date).
publishDate: '2024-01-15T00:00:00Z'

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ["article-journal"]

# Publication name and optional abbreviated publication name.
publication: "*ACM Transactions on Computer Systems*"
publication_short: ""
ccf_rank: A

abstract: Loop tiling and fusion are two essential transformations in optimizing compilers to enhance the data locality of programs. Existing heuristics either perform loop tiling and fusion in a particular order, missing some of their profitable compositions, or execute ad-hoc implementations for domain-specific applications, calling for a generalized and systematic solution in optimizing compilers.In this article, we present a so-called basteln (an abbreviation for backward slicing of tiled loop nests) strategy in polyhedral compilation to better model the interplay between loop tiling and fusion. The basteln strategy first groups loop nests by preserving their parallelism/tilability and next performs rectangular/parallelogram tiling to the output groups that produce data consumed outside the considered program fragment. The memory footprints required by each tile are then computed, from which the upward exposed data are extracted to determine the tile shapes of the remaining fusion groups. Such a tiling mechanism can construct complex tile shapes imposed by the dependences between these groups, which are further merged by a post-tiling fusion algorithm for enhancing data locality without losing the parallelism/tilability of the output groups. The basteln strategy also takes into account the amount of redundant computations and the fusion of independent groups, exhibiting a general applicability.We integrate the basteln strategy into two optimizing compilers, with one a general-purpose optimizer and the other a domain-specific compiler for deploying deep learning models. The experiments are conducted on CPU, GPU, and a deep learning accelerator to demonstrate the effectiveness of the approach for a wide class of application domains, including deep learning, image processing, sparse matrix computation, and linear algebra. In particular, the basteln strategy achieves a mean speedup of 1.8× over cuBLAS/cuDNN and 1.1× over TVM on GPU when used to optimize deep learning models; it also outperforms PPCG and TVM by 11% and 20%, respectively, when generating code for the deep learning accelerator.

# Summary. An optional shortened abstract.
summary: "*ACM Transactions on Computer Systems*"

tags:
- Source Themes
featured: false

# links:
# - name: ""
#   url: ""
url_pdf: 'https://dl.acm.org/doi/10.1145/3635305'
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
