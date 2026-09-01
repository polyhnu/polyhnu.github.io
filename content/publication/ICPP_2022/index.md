---
title: 'Automatically Generating High-performance Matrix Multiplication Kernels on the Latest Sunway Processor'

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
  - Xiaohan Tao
  - Yu Zhu
  - Boyang Wang
  - Jinlong Xu
  - Jianmin Pang
  - Jie Zhao
# Author notes (optional)
author_notes:
  - ''
  - ''
  - ''
  - ''
  - ''
  - 'Corresponding author'

date: '2022-09-01T00:00:00Z'
doi: ''

# Schedule page publish date (NOT publication's date).
publishDate: '2022-09-01T00:00:00Z'

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ['paper-conference']

# Publication name and optional abbreviated publication name.
publication: In *Proceedings of the 51st International Conference on Parallel Processing*
publication_short: In *ICPP 2022*
ccf_rank: B

abstract: We present an approach to the automatic generation of efficient matrix multiplication code on the latest Sunway processor, which will be employed by the next-generation machine of Sunway TaihuLight, one of the fastest supercomputers on earth. The method allows users to write simple C code and automatically generates high-performance matrix multiplication kernels. It uses polyhedral transformations to implement rapid compute decomposition, data exchanges across memory hierarchy and memory latency hiding. An assembly routine is finally integrated into the generated kernels. While achieving up to 90.14% of the theoretical peak performance, our method surpasses a highly tuned library by 9.44%. Compared with existing techniques, our approach reduces the software development life cycle to generate efficient matrix code from months to seconds. We also take into account batched matrix multiplication and some fusion patterns for deep learning (DL), outperforming the library-based implementations by 1.30 × and 1.67 ×.

# Summary. An optional shortened abstract.
summary: In *Proceedings of the 51st International Conference on Parallel Processing (ICPP 2022)*

tags: []

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://dl.acm.org/doi/10.1145/3545008.3545031'
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
