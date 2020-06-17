# Theoretical model
We developed a theoretical statistical model that allow us to determine a threshold in terms of string length to avoid spurious matches between two genomes based on genome lengths and GC-contents. We denote genome length as _n<sub>1</sub>_ and _n<sub>2</sub>_ respectively. We denote GC-content as _g<sub>1</sub>_ and _g<sub>2</sub>_ respectively. We assume that the numbers of nucleotides in a genome sutisfy the the following two conditions:
(1) genome does not contain any bases other than adenine (A), guanine (G), cytosine (C), and thymine (T) (there are no unknown or partially recognized nucleotides), and the numbers of these four nucleotides add up to the length of a genome.
(2) the number of Gs equals the number of Cs, and the number of As equals the number of Ts;  

Thus, we define probabilities for observing certain nucleotides in two genomes as follows

![Fig.1](/images/p_nuc.png)

Therefore, the probability p of a single nucleotide match assuming that nucleotides are independent is the following:

![Fig.2](/images/p_match.png)
