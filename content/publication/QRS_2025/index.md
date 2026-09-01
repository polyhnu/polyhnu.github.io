---
title: 'Scalable Detection of Floating-point Errors via Adaptive Parallel Subdomain Search'

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
  - Zuoyan Zhang
  - Shihan Yuan
  - Hongru Yang
  - Jie Zhao
  - Jinchen Xu

# Author notes (optional)
author_notes:
  - ''
  - ''
  - ''
  - ''
  - 'Corresponding author'

date: '2025-05-30T00:00:00Z'
doi: ''

# Schedule page publish date (NOT publication's date).
publishDate: '2025-05-30T00:00:00Z'

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ['paper-conference']

# Publication name and optional abbreviated publication name.
publication: In *Proceedings of the 25th IEEE International Conference on Software Quality, Reliability and Security*
publication_short: In *QRS 2025*
ccf_rank: C

abstract: "Floating-point error detection is crucial in numerical computing, particularly for multi-parameter functions where even minor errors can propagate and significantly impact results. The sparse distribution of floating-point errors poses a significant detection challenge, as significant deviations are triggered by only rare inputs. Existing search algorithms face two major limitations: poor scalability for multi-parameter functions and insufficient utilization of floating-point representation characteristics. To address these challenges, we propose SDPS (Scalable Detection via Parallel Subdomain Search), a novel algorithm that combines adaptive domain partitioning with floating-point-specific heuristics. SDPS employs a multi-level error classification system and specialized point generation strategies, supported by efficient parallel processing through dynamic task allocation. Our comprehensive evaluation demonstrates that SDPS significantly outperforms state-of-the-art methods in both detection accuracy and computational efficiency, especially for multi-parameter functions where it effectively addresses the exponential growth of search space that limits existing approaches."

# Summary. An optional shortened abstract.
summary: In *Proceedings of the 25th IEEE International Conference on Software Quality, Reliability and Security (QRS 2025)*

tags: []

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://ieeexplore.ieee.org/document/11173470'
url_code: 'https://github.com/zuoyanzhang/FPEPD/tree/macos'
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
