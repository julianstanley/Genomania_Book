---
description: Overview of Sequencing Technologies
---

# Sequencing Technologies

### Chapter Overview

* \*\*\*\*[**Sanger sequencing**](sanger-sequencing.md) ****was the first major DNA sequencing technology. It is highly accurate for read lengths up to ~1kb, but is prohibitively expensive for high-throughput sequencing. Sanger sequencing is still used today, but mostly for very small sequences of DNA. Sanger sequencing is sequencing by synthesis. 
* \*\*\*\*[**Pyrosequencing**](pyrosequencing.md) by 454 was the first next-generation sequencing technology. While it revolutionized the field, it recently became noncompetitive with Illumina technologies \(see [this academic paper](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0090485) and [this report](http://www.bio-itworld.com/2013/10/16/six-years-after-acquisition-roche-quietly-shutters-454.html)\). Pyrosequencing is sequencing by synthesis. 
* \*\*\*\*[**SOLiD sequencing**](solid-sequencing.md) is one of the first platforms NOT to sequence by synthesis. It's based on a 2-nucleotide sequencing by ligation. Since each base is passed over twice in a single run, SOLiD sequencing is very accurate. However, it has become less common, mainly due to very short read lengths \(~50-75bp\) and a very long time to run \(2 weeks, compared to approx 24 hours for Illumina\). 
* \*\*\*\*[**Illumina sequencing** ](short-read-sequencing.md)generally uses short reads \(50-300bp\) and sequences relatively accurately with a relatively low cost, which makes it the most popular platform for most sequencing projects. Illumina sequencing is sequencing by synthesis. 
* \*\*\*\*[**PacBio SMRT sequencing**](pacbio-smrt-sequencing.md) detects fluorescent labeled dNTP analogs in real time. It produces very long reads \(up to 30k at once\), but does so with very high error rates. SMRT sequencing is still active today, usually being used with on specific sequences such as those with low sequence complexity. 



| Method | Read Length | Error Rate | Cost per Gb \(approximate\) | Main Error Type |
| :--- | :--- | :--- | :--- | :--- |
| SOLID | 50 | &lt;0.1% | $70 | AT Bias |
| Illumina | 50-300 | ~0.1% | $40 | Substitution |
| 454 \(Pyrosequencing\) | 100-700 | ~1% | $80 | Insertion/Deletion |
| Sanger | 400-1000 | &lt;0.1% | $2,400,000 | Substitution |
| PacBio | 1000-30,000 | 13% | $1,000 | Insertion/Deletion |

