---
layout: post
title: Encryption
---


# PKEs, IBEs, and more [#ic2b985e]

## With average-case/worst-case reductions [#s4068035]

### Proposals [#raa4471b]

* [[[AD97-STOC]]] Mikl&oacute;s Ajtai and Cynthia Dwork: A public-key cryptosystem with worst-case/average-case equivalence. (STOC 1997, ECCC TR96-065)
    * 1-bit PKE based on O(n^12)-uSVP (I think the approximation factor is O(n^11)).
* [[[GGH97-C-Eli]]] Oded Goldreich, Shafi Goldwasser, and Shai Halevi: Eliminating decryption errors in the Ajtai-Dwork cryptosystem. (CRYPTO 1997, ECCC TR97-018)
    * Errorless version of the Ajtai-Dwork cryptosystem.
* [[[Reg03-STOC]]] Oded Regev: New lattice based cryptographic constructions. (STOC 2003, J. ACM 2004)
    * 1-bit PKE based on O(n^1.5)-uSVP
* [[[Reg05-STOC]]] Oded Regev: On lattices, learning with errors, random linear codes, and cryptography. (STOC 2005, J. ACM 2009)
    * 1-bit PKE based on SVP with approximation factor O~(n^1.5) (under quantum reduction).
* [[[KTX07-PKC]]] Akinori Kawachi, Keisuke Tanaka, and Keita Xagawa: Multi-bit public-key cryptosystem based on lattice problems. (PKC 2007, SCIS 2006)
    * O(log n)-bit versions of the Ajtai-Dwork, Regev03, Regev05, and Ajtai05 cryptosystems.
* [[[AD07-ECCC]]] Mikl&oacute;s Ajtai and Cynthia Dwork: The first and fourth public-key cryptosystems with worst-case/average-case equivalence. (ECCC TR07-097)
    * Improved version?
* [[[PW08-STOC]]] Chris Peikert and Brent Waters: Lossy trapdoor functions and their applications. (ePrint 2007/348, STOC 2008)
    * LWE-based O(n)-bit PKE secure in the sense of IND-CCA2 w/o RO
* [[[PVW08-C]]] Chris Peikert, Vinod Vaikuntanathan, and Brent Waters: A framework for efficient and composable oblivious transfer. (ePrint 2007/348, CRYPTO 2008)
    * O(n)-bit version of the Regev05 cryptosystem
* [[[GPV08-STOC]]] Craig Gentry, Chris Peikert, and Vinod Vaikuntanathan: Trapdoors for hard lattices and new cryptographic constructions. (STOC 2008)
    * ``Dual'' Encryption.
* [[[Pei09-STOC]]] Chris Peikert: Public-key cryptosystems from the worst-case shortest vector problem. (STOC 2009)
    * LWE-based IND-CCA2 PKE. If q &gt; 2^{n/2}, LWE &gt; GapSVP. This construction employs [[[AP09]]]
* [[[GV09-Manuscript]]] Shafi Goldwasser and Vinod Vaikuntanathan: . ()
    * According to [[[Pei09]]], Goldwasser and Vaikuntanathan prepared a manuscript on a CCA2-secure PKE from lattices.
* [[[LM09-C]]] Vadim Lyubashevsky and Daniele Micciancio: On bounded distance decoding, unique shortest vectors, and the minimum distance problem. (CRYPTO 2009)
    * A reduction from uSVP to GapSVP using Peikert's idea. This shows that the AD PKE and the Regev 03 PKE is based on the worst-case hardness of GapSVP_{O(n^{2.5})} and GapSVP_{O(n^2)}. (Why O(n^{2.5})?)
* [[[SSTX09-AC]]] Damien Stehl&eacute;, Ron Steinfeld, Keisuke Tanaka, and Keita Xagawa: Efficient public key encryption based on ideal lattices. (ASIACRYPT 2009, [[ePrint 2009/285:http://eprint.iacr.org/2009/285]])
    * IND-CPA secure PKE, DS w/ RO, IBI w/ RO, etc. from Ideal-SVP
* [[[CDMW09-AC]]] S. G. Choi, D. Dachman-Soled, T. Malkin, and H. Wee: Improved Non-Committing Encryption with Applications to Adaptively Secure Protocols. (ASIACRYPT 2009)
    * 2-round non-committing encryption from LWE. (Damg&aring;rd and Nielsen [[[DN00]]] gave a 3-round construction from LWE.)
* [[[BD10-TCC]]] B. Bendlin and I. Damg&aring;rd: Threshold decryption and zero-knowledge proofs for lattice-based cryptosystems. (TCC 2010, [[ePrint 2009/391:http://eprint.iacr.org/2009/391]])
    * A threshold PKE with distributed key-generation protocol based on the Regev 05 PKE. A plaintext proof-of-knowledge protocol is more efficient than the one by Xagawa, Kawachi, and Tanaka.
* [[[GHV10-EC]]] Craig Gentry, Shai Halevi, Vinod Vaikuntanathan: A simple BGN-type cryptosystem from LWE. (EUROCRYPT 2010)
    * Homomorphic Encryption: Add-then-Mult-then-Add
* [[[LPR10-EC]]] Vadim Lyubashevsky, Chris Peikert, Oded Regev: On ideal lattices and learning with errors over rings. (EUROCRYPT 2010)
    * The search-to-decision reduction for RingLWE. A new (but old) embedding.
* [[[CL10-eP]]] Huiyan Chen and Zichen Li: Lattice-based public key cryptosystem provably secure against adaptive chosen ciphertext attack. ([[ePrint 2010/121:http://eprint.iacr.org/2010/121]])
    * I found a simple CCA2 attack against their PKE...
* [[[Che10-eP]]] Huiyan Chen: CCA-secure cryptosystem from lattice. ([[ePrint 2010/127:http://eprint.iacr.org/2010/127]])
    * Again, I found a simple CCA2 attack against his/her PKE...
* [[[LP11-RSA]]] R. Lindner and Chris Peikert: Better Key Sizes (and Attacks) for LWE-Based Encryption. (CT-RSA 2011)
    * ...
* [[[SSP11-ACISP]]] Reza Sepahi, Ron Steinfeld, Josef Pieprzyk: Lattice-Based Completely Non-malleable PKE in the Standard Model (Poster). (ACISP 2011)
    *  Completely NM-CCA2 secure PKE. See the journal version [[[SSP12-DCC]]].
* [[[XXZ11-PQCrypto]]] Xiang Xie, Rui Xue, and Rui Zhang: Efficient Threshold Encryption from Lossy Trapdoor Functions. (PQCrypto 2011)
    *  I feel that &ldquo;employing a steam-hammer to crack a nut.
* [[[CGW13-ep]]] Daniel Cabarcas, Florian G&ouml;pfert, Patrick Weiden: Provably Secure LWE-Encryption with Uniform Secret. [[ePrint 2013/164:http://eprint.iacr.org/2013/164]]
    * An IND-CPA PKE based on the LWE assumption with small uniform errors ([[[DMQ13-EC]]] and [[[MP13-eP]]]).





### KDM/LR/RKA/DE [#f35c87a5]

* [[[BFO08]]]
    *  DE from Lossy TDFs.
* [[[AGV09-TCC]]] Akavia, Goldwasser, and Vaikuntanathan: Simultaneous hardcore bits and cryptography against freezing attacks. (TCC 2009)
    * On the security of Regev's encryption scheme against leakage of secret key. In addition, they proposed a simultaneous hardcore function for LWE.
* [[[ACPS09-C]]] Benny Applebaum, David Cash, Chris Peikert, and Amit Sahai: Fast cryptographic primitives and circular-secure encryption based on hard learning problems. (CRYPTO 2009)
    * KDM-CPA secure PKEs for any affine function from GapSVP.
* [[[DGK+10-TCC]]] Yevgeniy Dodis, Shafi Goldwasser, Yael Tauman Kalai, Chris Peikert, Vinod Vaikuntanathan: Public-Key Encryption Schemes with Auxiliary Inputs. TCC 2010
    * It shows the dual encryption scheme in [[[GPV08-STOC]]] has the key-leakage security.
* [[[BGK11-TCC]]] Z. Brakerski, Shafi Goldwasser, and Y. Kalai: Circular-secure encryption beyond Affine functions. (TCC 2011, [[ePrint 2009/485:http://eprint.iacr.org/2009/485]])
    * Beyond Affine KDM
* [[[BHHI10-EC]]] B. Barak, I. Haitner, D. Hofheinz, and Y. Ishai: Bounded Key-Dependent Message Security. (EUROCRYPT 2010, [[ePrint 2009/511:http://eprint.iacr.org/2009/511]])
    * Beyond Affine KDM.
* [[[AHI11-ICS]]] Benny Applebaum, Danny Harnik, Yuval Ishai: Semantic Security under Related-Key Attacks and Applications. ICS 2011
    *  additionally, RK-CPA2 SKE from LWE
* [[[BV11-C]]] Zvika Brakerski, Vinod Vaikuntanathan: Fully Homomorphic Encryption from Ring-LWE and Security for Key Dependent Messages. CRYPTO 2011, Rump session at TCC 2011.
    *  
* [[[Wee12-EC]]] Hoeteck Wee: Dual Projective Hashing and Its Applications     * - Lossy Trapdoor Functions and More. EUROCRYPT 2012
    *  New deterministic encryption from LWE.
* [[[ASP12-PKC]]] Jacob Alperin-Sheriff, Chris Peikert: Circular and KDM Security for Identity-Based Encryption. PKC 2012
    * UserKey dependente massage security.
* [[[Wee12-PKC]]] Hoeteck Wee: Public Key Encryption against Related Key Attacks. PKC 2012
    *  additionally, weakly RK-CCA2 PKE from LWE
* [[[XXZ12-ACNS]]] Xiang Xie, Rui Xue, and Rui Zhang: Inner-Product Lossy Trapdoor Functions and Applications. (ACNS 2012)
    *  
* [[[XXZ12-SCN]]] Xiang Xie, Rui Xue, and Rui Zhang: Deterministic Public Key Encryption and Identity-Based Encryption from Lattices in the Auxiliary-Input Setting. (SCN 2012, [[ePrint 2012/463:http://eprint.iacr.org/2012/463]])
    *  
* [[[SSP12-DCC]]] Reza Sepahi, Ron Steinfeld and Josef Pieprzyk: Lattice-based completely non-malleable public-key encryption in the standard model. (DESIGNS, CODES AND CRYPTOGRAPHY)
    *  
* [[[SS11-EC]]] Damien Stehl&eacute;, Ron Steinfeld: Making NTRU as Secure as Worst-Case Problems over Ideal Lattices. EUROCRYPT 2011
    *  Secure NTRU in Z_q[[[X]]]/(X^n+1) from RingLWE.
* [[[SLP+12-PKC]]] Ron Steinfeld, San Ling, Josef Pieprzyk, Christophe Tartary, Huaxiong Wang: NTRUCCA: How to Strengthen NTRUEncrypt to Chosen-Ciphertext Security in the Standard Model. PKC 2012
    *  CCA2 version of [[[SS11-EC]]].
* [[[AKPW13-C]]] Joel Alwen and Stephan Krenn and Krzysztof Pietrzak and Daniel Wichs: Learning with Rounding, Revisited: New Reduction, Properties and Applications. CRYPTO 2013, [[ePrint 2013/098:http://eprint.iacr.org/2013/098]]
    *  Improving parameters in [[[XXZ12-SCN]]] by improving the parameters of the LWR assumption.




###  Attacks [#if32d62d]

* [[[NS98]]] P. Q. Nguyen and J. Stern: Cryptanalysis of the Ajtai-Dwork cryptosystem. (CRYPTO 1998, ECCC TR98-010)
    * Up to n=32 in experimental manner.
* [[[HGS99]]] C. Hall, I. Goldberg, and B. Schneier: Reaction attacks against several public-key cryptosystems. (ICICS 1999)
    * A CCA1 universal-break attack against the Ajtai-Dwork cryptosystem.
* [[[PS09]]] T. Plantard and W. Susilo: Broadcast attacks against lattice-based cryptosystems. (ACNS 2009)
    * A heuristic attacks against several lattice-based PKEs.

### tmp [#h8926311]

* [[[YWZWW11]]] Xiaoyuan Yang, Liqiang Wu, Minqing Zhang, Ping Wei, and Lixian Wei: An ideal lattice based IBE scheme in the standard model. (Wuhan University Journal of Natural Sciences. Volume 16, Number 5 (2011), 439-446)
    *  [[Paper:http://www.springerlink.com/content/q04q542x7221q857/]].
* [[[OMO11]]] Okuhata, Manabe, and Okamoto: イデアル格子に基づくIDベース暗号 (SCIS 2011).
    * They proposed IBE based on Ideal-SVP.
* [[[Geo13-ICT-EurAsia]]] Adela Georgescu: Anonymous Lattice-Based Broadcast Encryption.  ICT-EurAsia 2013 (+ AsiaARES 2013?)
    * http://link.springer.com/chapter/10.1007/978-3-642-36818-9_39
* [[[YWZC13-CMA]]] Xiao-yuan Yanga, Li-qiang Wua, Min-qing Zhanga, and Xiao-Feng Chen: An efficient CCA-secure cryptosystem over ideal lattices from identity-based encryption. (Computers & Mathematics with Applications, Vol.65, Issue 9, May 2013, pp.1254    * 1263)


## Fully Homomorphic Encryption [#zea3bb8c]
See [[FHEs]]

## IBE and more [#k31a6884]
See [[IBE_and_more]].
