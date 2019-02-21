# Sanger Sequencing

### Key Points

#### Sanger sequencing:

* was the **first major method** for DNA sequencing
* is **sequencing by synthesis** in which a ddNTP is used as a terminator
* has read lengths up to **1kb**, is accurate, but relatively **low-throughput**
* can be read on a **gel** \(older\) or through a **capillary** \(more modern\)

### Review Questions

\(Answers at the bottom of the page\)

1. In what use cases might Sanger sequencing still be used today?
2. What are ddNTPs, and how do they vary from dNTPs?
3. How are ddNTPs labeled?
4. Approximately what year was Sanger sequencing first created?

Additional quiz questions here: [https://stanford.edu/~dsull/e25b\_quiz.html](https://stanford.edu/~dsull/e25b_quiz.html)

### **Overview**

Sanger sequencing, published in PNAS by [Fred Sanger in 1977](https://doi.org/10.1073/pnas.74.12.5463),  is one of the first methods used to reliably sequence DNA. In the first stages, it works like polymerase chain reaction \(PCR\), except in a reaction mixture spiked by terminating ddNTPs. Since the ddNTPs inhibit DNA strand elongation, the spiking of ddNTPs can essentially produce a library of truncated strands. By determining the identify of the ddNTP \(ddATP, ddTTP, ddGTP, ddCTP\) at the end of each truncated strand, we can piece together the sequence of each nucleotide along the complete strand. 

### **More Detail**

Four reaction mixtures are set up containing Taq polymerase, a primer, template DNA, all four dNTPs, and one of four terminating **ddNTPs**. We will determine the sequence of DNA by elongating the DNA \(like in PCR\) and terminating that elongation at different points along the growing strand. This technique of sequencing as the DNA strand elongates is called **sequencing by synthesis**. 

Dideoxynucleotides \(ddNTPs\) are identical to deoxynucleotides \(dNTPs\) except that their 3' hydroxyl group has been hydrated into a hydrogen. Since, in DNA elongation, the 3' hydroxyl acts as a nucleophile to extend the strand, a ddNTP blocks further elongation. 

![ddNTP \(right\) lacks the 3&apos;-hydroxyl of a functional dNTP \(left\)](../../.gitbook/assets/image%20%288%29.png)

In one reaction mixture, assuming an adequate number of elongation cycles and a correct ratio of dNTP:ddNTP \(functional:terminating\), the reaction mixture will contain fragments of the original sequence. All of those fragments will begin at the 5' end of the sequence and end at the particular ddNTP that was in the reaction mixture. For example, the reaction mixture with ddATP will contain all of the fragments of the original DNA strand that end in 'A'. 

With four reaction mixtures, we can begin to build back our sequence. If the DNA fragment that is 1-bp long was found in the ddATP pool, the original sequence begun with 'A'. If the 2-bp fragment was found in the ddCTP pool, the second nucleotide in the sequence is 'C', and so-on for up to 1000-bp.

To view the relative sizes of the DNA fragments in each reaction mixture, the ddNTPs that are included in the previous reaction will have been radiolabeled so that they will be visible in gel electrophoresis. Each of the 4 reaction mixtures are loaded into a gel and, working from the bottom of the gel \(smallest fragment\) to the top of the gel \(largest fragment\), we can reconstruct the DNA sequence. Generally, these gels can only accurately discriminate at a **1-bp** resolution up to around 1,000 base pairs. 

![Inferring DNA sequence from gel. Rightmost column shows sequence, from bottom\(5&apos;\) to top \(3&apos;\)](../../.gitbook/assets/image%20%287%29.png)

![Overall schematic of Sanger sequencing](../../.gitbook/assets/image%20%2810%29.png)

### **Additional Considerations**

Modern Sanger sequencing does not typically use regular gel electrophoresis \(mostly because the gels are very large and time-consuming to read\).   
  
Instead, ddNTPs are labeled fluorescently with different colors. That way, Sanger sequencing can be done in just one reaction lane. Then, DNA fragments are passed single-file through a gel capillary, and a high-speed camera takes pictures of each DNA fragment \(just like a gel, the smaller fragments move more quickly\) and fluorescent signals from the camera are then transformed into a DNA sequence.

![Schematic for capillary Sanger sequencing](../../.gitbook/assets/image%20%286%29.png)

#### 

![Original Sanger sequencing gel](../../.gitbook/assets/image%20%284%29.png)



### Videos!

{% embed url="https://www.youtube.com/watch?v=UTDwfgIM-ss" %}

{% embed url="https://www.youtube.com/watch?v=vK-HlMaitnE" %}

### Question Answers



1. Sanger sequencing is still commonly used today to validate short stretches of DNA, such as parts of the 16S rRNA gene in bacteria. It's still the most accurate way to sequence &lt;1kB pieces of DNA.
2. ddNTPs are 3'-deoxy, meaning they lack a 3'-OH on their ribose moiety that dNTPs have, therefore they are elongation-terminating. 
3. ddNTPs can be radiolabeled \(with phosphorous\) or florescent labeled. 
4. 1977. 

