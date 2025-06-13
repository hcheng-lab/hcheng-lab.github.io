---
title: "Cheng Lab - Research & Software"
layout: textlay
excerpt: "Cheng Lab -- Research & Software"
sitemap: false
permalink: /research/
---

# Research

[comment]: <> (![]({{ site.url }}{{ site.baseurl }}/images/respic/SciPost.png){: style="width: 70%; float: center; margin: 0px"})

Our overarching goal is to develop novel algorithms to address important and fundamental problems in computational genomics. Below are some of the key research themes we are currently exploring:

#### __High-performance genome assembly algorithm__
*De novo* assembly, especially *de novo* haplotype-resolved assembly, has been a central problem and remains one of the most challenging tasks in bioinformatics for four decades. It involves multiple advanced algorithms such as sketching, alignment and many branches in graph theory, and demands programming skills of the highest level. We have developed a series of *de novo* assembly algorithms, including hifiasm, hifiasm (Hi-C) and hifiasm (UL), which are designed to produce optimal genome assemblies by combining different data types. These algorithms have been widely used and have already become the dominant long-read genome assemblers. Currently, we are particularly interested in developing *de novo* assembly algorithms for complex genomes with polyploid alterations such as cancer genomes and polyploid plant genomes.

#### __Comprehensive variant calling and interpretation__
For the human genome, variant calling is typically performed through read alignment, which aligns fragmented reads back to the human reference genome. However, the generic reference genome often lacks specific personal information, leading to potential inaccuracies and biases, especially within highly repetitive and structurally different regions. Consequently, there is a rapidly growing demand for *de novo* genome assembly—a methodology that reconstructs the genome without relying on a reference. Leveraging our computational expertise, we aim to develop innovative variant calling and interpretation methods that are based on *de novo* genome assembly.

#### __Resolving challenging medically relevant genes__
Many critical medically relevant genes, such as HLA, SMN1, SMN2, C3, C4, and NOTCH2NLC, are difficult to resolve
due to high repetitiveness and structural variation. Most computational approaches rely on read-to-reference
alignments, which are constrained by the inaccuracies in reference genomes. Our goal is to develop assembly-based, 
reference-free computational methods to accurately reconstruct these challenging genomic regions.

# Software

* [hifiasm][sw-hifiasm]: a comprehensive *de novo* genome assembly toolkit supporting various data types and functionalities, 
  published in [Cheng et al (2021)][pub-ha1], [Cheng et al (2022)][pub-ha2], [Cheng et al (2024)][pub-ha3] and [Cheng et al (2025)][pub-ha4].
  <img style="margin: 0px" src="https://img.shields.io/github/stars/chhylp123/hifiasm"/>
  <a href="https://bioconda.github.io/recipes/hifiasm/README.html"><img style="margin: 0px" src="https://img.shields.io/conda/dn/bioconda/hifiasm.svg?style=flag&label=Bioconda"/></a>

[sw-hifiasm]: https://github.com/chhylp123/hifiasm
[pub-ha1]: https://www.nature.com/articles/s41592-020-01056-5
[pub-ha2]: https://www.nature.com/articles/s41587-022-01261-x
[pub-ha3]: https://www.nature.com/articles/s41592-024-02269-8
[pub-ha4]: https://www.biorxiv.org/content/10.1101/2025.04.14.648685v1