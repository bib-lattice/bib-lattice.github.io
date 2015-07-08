---
layout: post
title: Toolbox
---

# On the assumptions

* Ajtai
* Regev
* [[[GKPV10-ICS]]] S. Goldwasser, Y. Kalai, C. Peikert and V. Vaikuntanathan: Robustness of the Learning with Errors Assumption. ICS 2010
* [[[LPR10-EC]]] Vadim Lyubashevsky and Chris Peikert and Oded Regev: On Ideal Lattices and Learning with Errors Over Rings. EUROCRYPT 2010, [[ePrint 2012/230:http://eprint.iacr.org/2012/230]]
* [[[OPW11-C]]] Adam O'Neill, Chris Peikert, Brent Waters: Bi-Deniable Public-Key Encryption. CRYPTO 2011, [[ePrint 2011/352:http://eprint.iacr.org/2011/352]]
	* Proposal of the extended LWE assumption.
* [[[DD12-PKC]]] Leo Ducas and Alain Durmus: Ring-LWE in Polynomial Rings. PKC 2012, [[ePrint 2012/235:http://eprint.iacr.org/2012/235]]
* [[[AP12-PKC]]] Jacob Alperin-Sheriff, Chris Peikert: Circular and KDM Security for Identity-Based Encryption. PKC 2012.
	* Improvement of the extended LWE assumption.
* Adeline Langlois and Damien Stehl&eacute;: Hardness of decision (R)LWE for any modulus. [[ePrint 2012/090:http://eprint.iacr.org/2012/090]], withdrawn
* [[[BPR12-EC]]] Abhishek Banerjee, Chris Peikert, Alon Rosen: Pseudorandom Functions and Lattices. EUROCRYPT 2012, [[ePrint 2011/401:http://eprint.iacr.org/2011/401]]
	* Proposal of the LWR assumption
* [[[LL12-eP]]] Adeline Langlois and Damien Stehl&eacute;: Worst-Case to Average-Case Reductions for Module Lattices. [[ePrint 2012/090:http://eprint.iacr.org/2012/090]]
* [[[BLPRS13-STOC]]] Zvika Brakersi, Adeline Langlois, Chris Peikert, Oded Regev, Damien Stehl&eacute;: Classical Hardness of Learning with Errors. STOC 2013
* [[[GGH13-EC]]] Sanjam Garg, Craig Gentry, and Shai Halevi: Candidate Multilinear Maps from Ideal Lattices and Applications. EUROCRYPT 2013.
* [[[LPR13-EC]]] Vadim Lyubashevsky and Chris Peikert and Oded Regev: A Toolkit for Ring-LWE Cryptography. EUROCRYPT 2013.
* [[[DMQ13-EC]]] Nico D&ouml;ttling and J&ouml;rn M&uuml;ller-Quade: Lossy Codes and a New Variant of the Learning-With-Errors Problem. EUROCRYPT 2013.
* [[[MP13-C]]] Daniele Micciancio and Chris Peikert: Hardness of SIS and LWE with Small Parameters.  CRYPTO 2013, [[ePrint 2013/069:http://eprint.iacr.org/2013/069]]
* [[[AKPW13-C]]] Joel Alwen and Stephan Krenn and Krzysztof Pietrzak and Daniel Wichs: Learning with Rounding, Revisited: New Reduction, Properties and Applications. CRYPTO 2013
	* Improving the LWR assumption

# Estimations

* [[[BLRS08-PQC]]] J. Buchmann, R. Lindner, M. R&uuml;ckert, and M. Schneider: Explicit hard instances of the shortest vector problem. PQCrypto 2008
	* See http://www.latticechallenge.org/
* [[[ACFFP12-SCC]]] Martin R. Albrecht and Carlos Cid and Jean-Charles Faug&egrave;re and Robert Fitzpatrick and Ludovic Perret: On the Complexity of the BKW Algorithm on LWE. SCC 2012, [[ePrint 2012/636:http://eprint.iacr.org/2012/636]]


#  Toolbox

* [[[RS10-eP]]] M. R&uuml;ckert and M. Schneider: Estimating the Security of Lattice-based Cryptosystems. [[ePrint 2010/137:http://eprint.iacr.org/2010/137]]

# Sampling

* [[[Kle01]]] 
* [[[GPV08]]] ... 
* [[[Pei10-C]]] Chris Peikert: An Efficient and Parallel Gaussian Sampler for Lattices. CRYPTO 2010, [[ePrint 2010/088:http://eprint.iacr.org/2010/088]]
* [[[DN12-AC]]] Leo Ducas and Phong Q. Nguyen. Faster Gaussian Lattice Sampling using Lazy Floating-Point Arithmetic. Asiacrypt 2012
* [[[AGHS12-eP]]] Shweta Agrawal and Craig Gentry and Shai Halevi and Amit Sahai: Discrete Gaussian Leftover Hash Lemma over Infinite Domains. [[ePrint 2012/714:http://eprint.iacr.org/2012/714]]
* [[[AR13-arXiv]]] Divesh Aggarwal and Oded Regev: A Note on Discrete Gaussian Combinations of Lattice Vectors. [[arXiv1308.2405:http://arxiv.org/abs/1308.2405]]
* [[[RVV13-SAC]]] Sujoy Sinha Roy, Frederik Vercauteren, and Ingrid Verbauwhede: High Precision Discrete Gaussian Sampling on FPGAs. SAC 2013
* [[[BCGHW13-SAC]]] Johannes Buchmann, Daniel Cabarcas, Florian G&ouml;pfert, Andreas H&uuml;lsing, and Patrick Weiden: Discrete Ziggurat: A Time-Memory Trade-off for Sampling from a Gaussian Distribution over the Integers. SAC 2013
* [[[DDLL13-C]]] Leo Ducas, Alain Durmus, Tancrede Lepoint, and Vadim Lyubashevsky: Lattice Signatures and Bimodal Gaussians. CRYPTO 2013

# Toolbox 2

## Lattice Algorithms

* LLL, BKZ, BKZ2.0, enum, Sieve, and more.
* [[[LN13-CTRSA]]] Mingjie Liu and Phong Q. Nguyen: Solving BDD by Enumeration: An Update. CT-RSA 2013
* [[[PSZ12-SAC]]] Thomas Plantard, Willy Susilo and Zhenfei Zhang: Lattice Reduction for Modular Knapsack. SAC 2012
	* Recursive LLL
* [[[IKMT13-eP]]] Tsukasa Ishiguro, Shinsaku Kiyomoto, Yutaka Miyake, and Tsuyohsi Takagi: Parallel Gauss Sieve Algorithm: Solving the SVP in the Ideal Lattice of 128 dimensions. [[ePrint 2013/388:http://eprint.iacr.org/2013/388]]

# Template of Attacks

* [[[CS97-EC]]] Don Coppersmith and Adi Shamir: Lattice attacks on NTRU. EUROCRYPT 1997
* [[[PSZ12-SAC]]] Thomas Plantard, Willy Susilo and Zhenfei Zhang: Lattice Reduction for Modular Knapsack. SAC 2012
* [[[HM12-SCN]]] Gottfried Herold and Alexander Meurer: New Attacks for Knapsack Based Cryptosystems. SCN 2012
	* Improve Shamir's well-known attack.

#  Implementations [#r937fa17]

* [[[GP12-Latin]]] Tim G&uuml;neysu and Thomas P&ouml;ppelmann: Towards Efficient Arithmetic for Lattice-Based Cryptography on Reconfigurable Hardware. Latincrypt 2012
* [[[GFSHB12-CHES]]] Norman G&ouml;ttert, Thomas Feller, Michael Schneider, Sorin A. Huss, and Johannes Buchmann: On the Design of Hardware Building Blocks for Modern Lattice-Based Encryption Schemes. CHES 2012
* [[[GLP12-CHES]]] Tim G&uuml;neysu, Vadim Lyubashevsky, and Thomas P&ouml;ppelmann: Practical Lattice-based Cryptography: A Signature Scheme for Embedded Systems. CHES 2012
* [[[WHCB13-eP]]] Patrick Weiden, Andreas H&uuml;lsing, Daniel Cabarcas, and Johannes Buchmann: Instantiating Treeless Signature Schemes. [[ePrint 2013/065:http://eprint.iacr.org/2013/065]]
* [[[EB13-SAC]]] Rachid El Bansarkhani and Johannes Buchmann: Improvement and Efficient Implementation of a Lattice-based Signature Scheme. SAC 2013
* [[[PG13-SAC]]] Thomas P&omul;ppelmann and Tim G&uuml;neysu: Towards Practical Lattice-Based Public-Key Encryption on Reconfigurable Hardware. SAC 2013
