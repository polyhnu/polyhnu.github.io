---
title: 'Optimizing the Memory Hierarchy by Compositing Automatic Transformations on Computations and Data'

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
  - Jie Zhao
  - Peng Di

# Author notes (optional)
author_notes:
  - 'Corresponding author'
  - 'Corresponding author'


date: '2020-10-17T00:00:00Z'
doi: ''

# Schedule page publish date (NOT publication's date).
publishDate: '2020-10-17T00:00:00Z'

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ['paper-conference']

# Publication name and optional abbreviated publication name.
publication: In *Proceedings of the 53rd IEEE/ACM International Symposium on Microarchitecture*
publication_short: In *MICRO 2020*
ccf_rank: A

abstract: Optimizing compilers exploit the memory hierarchy using loop tiling and fusion, but these two transformations usually interfere with each other due to the oversight of transformations on data in memories. We present a novel composition of loop tiling and fusion in this paper. Unlike existing tiling-after-fusion algorithms that only transform computation spaces, our approach first applies rectangular/parallelogram tiling to live-out computation spaces for fitting the memory hierarchy, followed by the computation of the memory footprints required by each tile. The upwards exposed data extracted from the memory footprints are used to determine the tile shapes of intermediate computation spaces, allowing the construction of arbitrary tile shapes. Finally, our technique implements a post-tiling fusion strategy for maximizing data locality without losing tilability or parallelism of live-out computation spaces, thereby enabling storage reduction and reuse, and optimizing the memory hierarchy. We demonstrate that our approach can achieve superior performance on both CPU and GPU architectures over the state of the art by experimenting on 11 benchmarks extracted from numerous domains including neural networks, image processing, sparse matrix computation and linear algebra. Also, the results of the ResNet-50 model on an AI accelerator show that our approach can obtain 16% performance improvement.

# Summary. An optional shortened abstract.
summary: In *Proceedings of the 53rd IEEE/ACM International Symposium on Microarchitecture (MICRO 2020)*

tags: []

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://ieeexplore.ieee.org/document/9251965/'
url_code: ''
url_dataset: ''
url_poster: ''
url_project: ''
url_slides: 'https://yaozhujia.github.io/assets/pdf/micro2020-presentation.pdf'
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
