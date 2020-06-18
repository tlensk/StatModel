# Theoretical model
We developed a theoretical statistical model that allow us to determine a threshold in terms of string length to avoid spurious matches between two genomes based on genome lengths and GC-contents. We denote genome length as _n<sub>1</sub>_ and _n<sub>2</sub>_ respectively. We denote GC-content as _g<sub>1</sub>_ and _g<sub>2</sub>_ respectively. We assume that the numbers of nucleotides in a genome sutisfy the the following two conditions:
(1) genome does not contain any bases other than adenine (A), guanine (G), cytosine (C), and thymine (T) (there are no unknown or partially recognized nucleotides), and the numbers of these four nucleotides add up to the length of a genome.
(2) the number of Gs equals the number of Cs, and the number of As equals the number of Ts;  

Thus, we define probabilities for observing certain nucleotides in two genomes as follows

![Fig.1](/images/p_nuc.png)

Therefore, the probability p of a single nucleotide match assuming that nucleotides are independent is the following:

![Fig.2](/images/p_match.png)

And conversely, the probability of a single nucleotide mismatch is 1 – p.

For example, if    _g<sub>1</sub>_ =  _g<sub>2</sub>_ = 0.5 (i.e., GC-content in both genomes is 50%) then _p_=0.25. 

We assume that nucleotide matches are mutually exclusive then the probability of a match between two strings of length _k_ equals _p<sup>k</sup>_. Thus, the probability that two string of length _k_ mismatch is (1 – _p<sup>k</sup>_).

Moreover, the probability of no match between a particular string of length _k_ and a set of _m_ strings of length _k_ is equal to
<br>
(1 – _p<sup>k</sup>_)_<sup>m</sup>_. Thus, the probability that no string out of a set of q strings, each of length _k_, matches any string out of a separate set of _m_ strings, each of length _k_:

![Fig.3](/images/prob.png)

To compute this probability, we use the following formula:

![Fig.4](/images/prob_e.png)

In addition, we use the power series to compute log(1-x) for small x (x < 0.25).

![Fig.5](/images/log.png)



