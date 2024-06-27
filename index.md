---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: page
title: Home
page_title: Welcome to the Cheng Lab @ Yale
---

**We are a computational genomics lab based in the [Department of Biomedical Informatics and Data Science (BIDS)][BIDS] at Yale University, School of Medicine.** Our research is dedicated to creating highly efficient computational methodologies for genomic applications, including genome assembly, read alignment, variant calling, and string indexing. We have developed a series of *de novo* genome assembly algorithms (e.g. [hifiasm][Hifiasm]) that have been extensively utilized across a variety of large-scale sequencing projects, such as the [Human Pangenome Reference Consortium][HPRC], the [Vertebrate Genomes Project][VGP], and the [Darwin Tree of Life project][DWOT]. Within these projects, we also work closely with collaborators to explore the applications of genome assemblies. Our lab is always open to new collaboration opportunities with both basic science and clinical research groups.


{% include spareline.html%}
- **We are currently seeking postdocs, students, and staff to join our team**. For more information, please view our available [vacancies][Vaca].

<!---
{% include linebreaker.html%}

- We are interested in disease systems of multi-cellular components especially cancer. 
- We lead development of computational, statistical, and machine learning methods that leverage large-scale and multi-omic data to understand cancer initiation, progression, and therapeutic responses. 
- We foster an interdisciplinary, inclusive, and supportive environment. We welcome computational biologists, bioinformaticians, computer scientists, MDs, immunologists, and oncologists. 
- We are enthuastic collaborators to work on real-world biological and translational genomics problems. 
- <u>Postdocs</u> or PhD soon-to-be who work on computational biology, bioinformatics, cancer genomics, single-cell omics, spatial transcriptomics, machine learning, genetic variant function, and biological questions in cancer or tumor microenvironment - Welcome to contact and join us! If possible please include (1) CV or Resume (2) A short research statement describing previous/ongoing work and proposed research and interest (3) 1-3 representative publications (published, accepted, or preprint) (4) Three names of references and contact information. Thanks! (Job postings to come)
- <u>Prospective students</u> interested in our research are encouraged to apply through Duke graduate programs: Computational Biology and Bioinformatics ([CBB] - PhD), Biostatsistics (PhD & MS). (Or co-mentoring for other Duke programs!) Graduate admission decisions are made by program committee. If contacting for interest, please include (1) CV or Resume (2) Short description of research experiences and interest (3) Three names of references and contact information. We will also be available for CBB & Biostats students to rotate soon.
-->

{% include linebreaker.html%}
---
## Research interests

#### __Complex genome reconstruction with *de novo* assembly__

*De novo* assembly, especially *de novo* haplotype-resolved assembly, has been a central problem and remains one of the most challenging tasks in bioinformatics for four decades. It involves multiple advanced algorithms such as sketching, alignment and many branches in graph theory, and demands programming skills of the highest level. We have developed a series of *de novo* assembly algorithms, including hifiasm, hifiasm (Hi-C) and hifiasm (UL), which are designed to produce optimal genome assemblies by combining different data types. These algorithms have been widely used and have already become the dominant long-read genome assemblers. Currently, we are particularly interested in developing *de novo* assembly algorithms  for complex genomes with polyploid alterations such as cancer genomes and polyploid plant genomes.

{% include spareline.html%}

#### __Comprehensive variant calling and interpretation__

For the human genome, variant calling is typically performed through read alignment, which aligns fragmented reads back to the human reference genome. However, the generic reference genome often lacks specific personal information, leading to potential inaccuracies and biases, especially within highly repetitive and structurally different regions. Consequently, there is a rapidly growing demand for *de novo* genome assembly—a methodology that reconstructs the genome without relying on a reference. Leveraging our computational expertise, we aim to develop innovative variant calling and interpretation methods that are based on *de novo* genome assembly.


{% include linebreaker.html%}
---
## Selected publications

- <strong>Cheng H</strong>, Asri M, Lucas J, Koren S, Li H#. "Scalable telomere-to-telomere assembly for diploid and polyploid genomes with double graph." <a href="https://www.nature.com/articles/s41592-024-02269-8" target="_blank"><strong><em>Nat Methods</em></strong></a> (2024).

- <strong>Cheng H</strong>, Jarvis ED, Fedrigo O, Koepfli KP, Urban L, Gemmell NJ, Li H#. "Haplotype-resolved assembly of diploid genomes without parental data." <a href="https://www.nature.com/articles/s41587-022-01261-x" target="_blank"><strong><em>Nat Biotechnol</em></strong></a> (2022).

- <strong>Cheng H</strong>, Concepcion GT, Feng X, Zhang H, Li H#. "Haplotype-resolved de novo assembly using phased assembly graphs with hifiasm." <a href="https://www.nature.com/articles/s41592-020-01056-5" target="_blank"><strong><em>Nat Methods</em></strong></a> (2021).

- <strong>Cheng H</strong>, Wu M, Xu Y#. "FMtree: a fast locating algorithm of FM-indexes for genomic data." <a href="https://academic.oup.com/bioinformatics/article/34/3/416/4160683" target="_blank"><strong><em>Bioinformatics</em></strong></a> (2018).


<!---
{% include image.html image_path="pics/RI_1.png" image_width="50%" %}

The advance of sequencing technologies makes it possible to produce high-quality reads that are both long and accurate. However, most existing de novo assembly algorithms could not take full advantage of the power of long accurate reads, as they were originally designed for long error-prone reads. To this end, we have been developing a haplotype-resolved assembly algorithm [hifiasm](https://www.nature.com/articles/s41592-020-01056-5) (*Cheng et al. Nat Methods* 2021), which introduces a haplotype-aware error correction strategy to faithfully reconstruct different haplotypes and resolve repeats. Additionally, hifiasm incorporates the graph-binning strategy, leveraging the topological information of the assembly graph to significantly improve the quality of trio-binning assemblies. The benchmark conducted by the Human Pangenome Reference Consortium (HPRC) showed that hifiasm outperformed all other algorithms by a large margin, enabling it to be the assembler of choice by HPRC. Hifiasm has also been widely used by many other large-scale sequencing projects, such as the Genome in a Bottle (GIAB), the Vertebrate Genomes Project (VGP), as well as the Darwin Tree of Life project (DToL).



{% include linebreaker.html%}
{% include spareline.html%}


{% include image.html image_path="pics/RI_2.png" image_width="50%" %}

The limitation of hifiasm is that it requires parental data to produce fully-phased assemblies, which is not always available. To address this limitation, we have been extending hifiasm to yield single-sample fully-phased assemblies by integrating additional Hi-C data. The extended hifiasm, termed [hifiasm (Hi-C)](https://www.nature.com/articles/s41587-022-01261-x) (*Cheng et al. Nat Biotechnol* 2022), combines the local phasing information of long reads with the long-range phasing information of Hi-C reads to achieve chromosome-scale phasing. Hifiasm (Hi-C) solves the fully-phased assembly problem as a max-cut-based optimization problem, and leverages the topological structure of the assembly graph for further improvement. Several consortiums, such as the Human Pangenome Reference Consortium (HPRC) and the Vertebrate Genomes Project (VGP), are deploying hifiasm (Hi-C) at scale.


{% include linebreaker.html%}
{% include spareline.html%}

{% include image.html image_path="pics/RI_3.png" image_width="50%" %}

The advent of accurate PacBio High-Fidelity (HiFi) long reads enables the haplotype-resolved assembly to become a routine procedure for large genomes. However, HiFi reads, while precise, often fall short in length to resolve long exact repeats, leading to fragmented segments in repeat-dense areas, such as centromeres. Building upon my earlier HiFi-only hifiasm algorithm, I developed a hybrid assembly approach, termed [hifiasm (UL)](https://www.nature.com/articles/s41592-024-02269-8) (*Cheng et al. Nat Methods* 2024). This incorporates the considerably longer, albeit less accurate, ultra-long ONT reads. The advantages of hifiasm (UL) stem mainly from the novel double graph framework, which integrates assembly graphs at different scales, maximizing the capabilities of both HiFi and ultra-long reads. The Human Pangenome Reference Consortium (HPRC) is assembling 150 telomere-to-telomere human genomes utilizing hifiasm (UL) due to its demonstrated superior performance.
-->

[DFCI]: https://ds.dfci.harvard.edu/
[HSPH]: https://www.hsph.harvard.edu/
[LiuLab]: https://liulab-dfci.github.io/
[MylesLab]: https://mylesbrownlab.dana-farber.org/
[LinLab]: https://content.sph.harvard.edu/xlin/people.html
[SongLab]: https://song.igb.illinois.edu/
[UIUC]: https://illinois.edu/
[BIDS]: https://medicine.yale.edu/biomedical-informatics-data-science/
[Hifiasm]: https://github.com/chhylp123/hifiasm
[HPRC]: https://humanpangenome.org/
[VGP]: https://vertebrategenomesproject.org/
[DWOT]: https://www.darwintreeoflife.org/
[DukeSoM]: https://medschool.duke.edu
[DukeNeurosurgery]: https://neurosurgery.duke.edu/news/yi-zhang-joins-duke-neurosurgery-faculty
[DukeBB]: https://biostat.duke.edu
[Contact]: mailto:yi.zhang@duke.edu
[CBB]: https://medschool.duke.edu/education/biomedical-phd-programs/computational-biology-and-bioinformatics-program
[Vaca]: https://hcheng-lab.github.io/join/ 
