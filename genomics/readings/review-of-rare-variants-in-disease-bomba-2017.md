# Review of rare variants in disease \(Bomba 2017\)

### Key Points

#### The Bomba paper:

* Reviewed major techniques used to detect and analyze rare variants
* Gave an overview of statistical methods used to analyze rare variants
* Gave examples of studies that successfully studied rare variants 

### Review Questions

\(Answers at the bottom of the page\)

1. What is population stratification?
2. What three major methods are used to detect rare variants?
3. What is the difference between SKAT and SKAT-O?
4. Explain the major limitation of burden tests \(as compared to variance tests\)

### **Overview**

To detect rare variants, researchers can use \(1\) imputation, \(2\) custom genotyping arrays, and \(3\) next-generation sequencing. Imputation is a computational technique that infers genotypes from public databases, whereas custom genotyping arrays and next generation sequencing are wet-lab techniques.

To analyze rare variants, researchers use \(1\) burden tests such as CAST, which combine rare variants to increase power but assume that all of those variants have the same effect on the phenotype of interest \(2\) Variant component tests such as SKAT, which improve on the standard burden test by allowing for bidirectional effects and applying other weighting techniques. \(3\) Tests that combine approaches from burden tests and variant component tests, such as SKAT-O, and \(4\) Some tests that do not fall into the previous tests but are not discussed in the paper, such as LASSO and EG. 

The paper also talks about study design. A common trend called population stratification is that a variant may be rare in the general population, but more common in certain smaller populations. Studies can take advantage of this principle, such as the deCODE study, which used Icelandic populations to identify rare variants and a potential drug target.

### **More Detail**

This study aimed to provide a resource for continuing rare variant research. That's important because there are lots of interactions between rare variants

To computationally improve power of a study, you can use a technique called imputation. First, phased haplotypes are used to build reference panel. Then, a study that detects fewer variants can computationally infer new variants. WGS projects like the 1000 Genomes Project provide public reference panel. 

To 

* Diseased-focused
  * Immunochip \(autoimmune, inflammatory\)
  * Exomechip \(high-confidence unique, protein-altering variants\)

**WGS**

* Increasingly used due to lowered cost
  * WES cost less

#### Computational methods

* Regular statistics doesn't work
  * Simple regression doesn't have enough power
  * More rare variants means high multiple testing penalty
* Burden Test \(e.g. CAST, which is binary, also ARIEL and WSS\)
  * Simple or complex \(0 or 1\) or \(apply weight based on frequency\)
  * Score a functional region of the genome
    * Add up all rare variants and score that as one score
      * Regress against phenotype
  * Limitation: assume that all variants have the same effect on the phenotype
* Variance Component Test \(SKAT\)
  * Assume: there are risk and protective alleles
    * More flexible with different data sets
    * More consideration to weighted statistics
  * Accounts for different effects
  * Score each SNP individually, then compute a region-level p value
  * E.g. SKAT
* Combined tests
  * Generally more realistic
    * Fisher method or SKAT-O
  * Combine variance component and burden, get a more powerful model. E.g. SKAT-O \(combine SKAT with burden test\)
* Other
  * Designed to account for signal sparsity
    * Often take longer
  * LASSO, EG, Baysian approaches

**Analyses for rare variant association tests**

Which method will be the best one for the data set?

* Using stimulated type 2 diabetes genomes:
  * Combined tests \(SKAT-O, MiST\) have more power to detect rare variants
  * Linkage disequilibrium should be reflected \(haplotypes are not represented as expected\)

Problems: tests are under powered

Solution: More replication, control for confounding variables.

* Bigger samples help
* Combining tests help power
* How to increase replication?
  * Genotype the same cohort again
  * Incorporate geographical and family-based models
* Study design is also important
  * Isolated/inbred populations \(e.g. APOC3 relevance in lipid levels\)
    * Dutch population, Sardinia.
    * A variant that is rare in general pop may not be as rare in this population \(population stratification\)
      * E.g. iceland
      * Rare in global studies but common in sample
  * Complete knockout alleles
    * Loss of function
      * ExAC used to discover new low-frequency variants
    * But may not actually cause disease state, needs some skepticism
  * PROMIS study
    * Inactivated 961 genes in at least 1 participant

**Initial results**

25 different studies --&gt; 31 genes with some conditions

Great table in powerpoint \(group?\) for UK10K, SardiNIA, deCode, goNL, and CHARGE

* Non-synonymous SNVs in Denmark
* UK10K Project
* deCODE
  * Generated pop-specific refernece panel from Iceland
    * Applied that reference panel to 90,000 people with available SNP arrays
    * Infer over 250,000 more people from genealogical records
  * Takeaways: pop-specific reference panel, and massive study size
  * Results: 7 rare variants and a potential drug target

**Future prospects**

* Few GWAS have been able to be translated
  * May become more common

### **Additional Considerations**

### Videos!

