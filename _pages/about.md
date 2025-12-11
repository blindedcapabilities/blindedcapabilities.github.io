---
layout: about
permalink: /
title: BLACKOUT
subtitle: Data-Oblivious Computation with Blinded Capabilities

# profile:
#   align: right
#   image: prof_pic.jpg
#   image_circular: false # crops the image to make it circular
#   more_info: >
#     <p>555 your office number</p>
#     <p>123 your address street</p>
#     <p>Your City, State 12345</p>

selected_papers: false # includes a list of papers marked as "selected={true}"
social: false # includes social icons at the bottom of the page

announcements:
  enabled: false # includes a list of news items
  scrollable: true # adds a vertical scroll bar if there are more than 3 news items
  limit: 5 # leave blank to include all the news in the `_news` folder

latest_posts:
  enabled: false
  scrollable: true # adds a vertical scroll bar if there are more than 3 new posts items
  limit: 3 # leave blank to include all the blog posts
---

<!-- # BLACKOUT: Data-Oblivious Computation with Blinded Capabilities -->
<!-- # Data-Oblivious Computation with Blinded Capabilities -->

<br>

#### Overview

Lack of memory-safety and exposure to side channels are two prominent, persistent challenges for the secure implementation of software. Memory-safe programming languages promise to significantly reduce the prevalence of memory-safety bugs, but make it more difficult to implement side-channel-resistant code. We aim to address both memory-safety and side-channel resistance by augmenting memory-safe hardware with the ability for data-oblivious programming. We describe an extension to the CHERI capability architecture to provide blinded capabilities that allow data-oblivious computation to be carried out by userspace tasks. We also present BLACKOUT, our realization of blinded capabilities on a FPGA softcore based on the speculative out-of-order CHERI-Toooba processor and extend the CHERI-enabled Clang/LLVM compiler and the CheriBSD operating system with support for blinded capabilities. BLACKOUT makes writing side-channel-resistant code easier by making non-data-oblivious operations via blinded capabilities explicitly fault. Through rigorous evaluation we show that BLACKOUT ensures memory operated on through blinded capabilities is securely allocated, used, and reclaimed and demonstrate that, in benchmarks comparable to those used by previous work, BLACKOUT imposes only a small performance degradation (1.5% geometric mean) compared to the baseline CHERI-Toooba processor. 

#### Publications

<div class="publications">
  {% bibliography -f {{ site.scholar.bibliography }} --group_by none --query @*[selected]* %}
</div>

<!-- ### Blog posts

- BliMe: NDSS'24 [talk](https://youtu.be/cfyvaW1wwQk?si=TuICEfLogqUjTgAp), [pdf](/assets/pdf/platsec/BliMe-NDSS24-slides.pdf)
- Dolma: HOST'24 [poster](/assets/pdf/platsec/Dolma-HOST24-poster.pdf) -->

#### Blog posts
- [SSG](https://blog.ssg.aalto.fi/2025/10/making-software-both-memory-safe-and.html)

#### Presentations
- CCS'25 [Video](https://youtu.be/YcWzuwbvdic?si=ku5a_CuW7N88KgJx), [Slides](assets/pdf/CCS25.pdf)

#### Source code

- [CCS'25 Artifact](https://zenodo.org/records/17035867?token=eyJhbGciOiJIUzUxMiJ9.eyJpZCI6ImM3YmNkOWYxLTY1NGQtNDdjMy1hY2Q3LWM1MjE2YmRkMmNjMyIsImRhdGEiOnt9LCJyYW5kb20iOiJhNzdiMGY5N2VjYjU4ZDdhYzU4MDk3NzI1NjkxNDYxYyJ9.CscvIsUJ7mMT8avu_DqRjKBe5al9n8-kFrOQYoGujwAVWPk60ZTOE_RNyfnCniQCpA3BTSoE7eB0QjPSeqxNQA)
- [GitHub Repos](https://github.com/blindedcapabilities)