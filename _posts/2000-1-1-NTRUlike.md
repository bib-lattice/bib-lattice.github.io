---
layout: post
title: NTRU and its variants
---

# Proposal

* J. Hoffstein? Proposal of NTRU (The rump session in CRYPTO 1996)
* [HPS98] J. Hoffstein, J. Pipher, J. H. Silverman: NTRU: A ring-based public key cryptosystem. (ANTS 1998)
    * In Z[x]/(q,X^N-1).
* [BS02] W. D. Banks and I. Shparlinski: A variant of NTRU with non-invertible polynomials. (INDOCRYPT 2002)
    * A generalization of NTRU.
* [GOS02] P. Gaborit, J. Ohler, and P. Sol&eacute;: CTRU, a polynomial analogue of NTRU. ([[rapport de recherche INRIA RR-4621, Nov., 2002:http://hal.archives-ouvertes.fr/inria-00071964/en/]])
    * A variant in (F_2[T])[X]/(Q[X],X^N-1). See [[RR-4621:http://www.inria.fr/rrrt/rr-4621.html]]
* [CG05] M. Coglianese and B.-M. Goi: MaTRU: A new NTRU-based cryptosystem. (INDOCRYPT 2005)
    * A variant in M_{k,k}(R)[X]/(q,X^n-1), where R=Z[X]/(X^n-1).
* [Kou06] R. Kouzmenko &ldquo;Generalizations of the NTRU cryptosystem. (Diploma Project, Winter semester 2005-2006)
    * A variant in ((Z[i])[X])/(q,X^N-1). It is called NTRU using Gaussian integers. See [[ALGO+LMA - Output - MSc Theses:http://algo.epfl.ch/index.php?p=output_diplomapr&l=en]]. He/She also cryptanalyzed CTRU [GOS02].
* [YZ06] J. Yao, G. Zeng &ldquo;Enhanced NTRU cryptosystem eliminating decryption failures. (Journal of Systems Engineering and Electronics, vol. 17, No. 4, 2006)
    * The main motivation is eliminating wrap failures. In order to resist the CCA attacks, the authors set pk=(h=f^{-1}*g_1, l=p*f^{-1}*g_2). Encryption is obtained as e=m*h+l*r. They insisted that the scheme without padding can resist the CCA attacks.
* [Tru07] K. R. Truman: Analysis and extension of non-commutative NTRU. (Ph.D Thesis, University of Maryland)
    * ...
* [NSP08-ICON] Rakesh Nayak, C. V. Sastry, Jayaram Pradhan: A matrix formulation for NTRU cryptosystem. (ICON 2008)
    * A varinat in M_{n,n}(Z_q). 
    * C = pR H + M  mod q, where M in M_n(-1,0,+1)
* [Vat09] N. Vats: NNRU, a noncommutative analogue of NTRU. ([[arXiv 0902.1891v1:http://arxiv.org/abs/0902.1891]])
    * A variant in M_{k,k}(Z)[X]/(q,X^n-I_{k,k}).
* [MZM09] E. Malekian, A. Zakerolhosseini, A. Mashatan: QTRU: A lattice attack resistant version of NTRU. ([[ePrint 2009/386:http://eprint.iacr.org/2009/386]])
    * A variant in R+Ri+Rj+Rk, where R = Z_q[X]/(X^N-1).
* [MZ09] E. Malekian, A. Zakerolhosseini: NTRU-like public key cryptosystems beyond Dedekind domain up to alternative algebra. ([[ePrint 2009/446:http://eprint.iacr.org/2009/446]])
    * A variant employing octonions.
* [XT09-SCIS] Keita Xagawa and Keisuke Tanaka: NFALSE: Another Ring-Based Public Key Cryptosystem with Faster Encryption. (SCIS 2009)
    * A variant employing in Z_q[X]/(X^n+1) with n = 2^z.
* [NKM10-DCC] Monica Nevins, Camelia KarimianPour, Ali Miri: NTRU over rings beyond {\mathbb{Z}}. Designs, Codes and Cryptography, July 2010, Volume 56, Issue 1, pp 65-78.
* [PD11-WISA] Yanbin Pan, Yingpu Deng: A General NTRU-Like Framework for Constructing Lattice-Based Public-Key Cryptosystems. WISA 2011
    *  http://rd.springer.com/chapter/10.1007/978-3-642-27890-7_9
    *  Similar to [NSP08-ICON] but moderate parameters.
* [JV13-DCC] Katherine Jarvis, Monica Nevins: ETRU: NTRU over the Eisenstein integers. (DCC 2013)
    *  http://rd.springer.com/article/10.1007/s10623-013-9850-3
    *  Replacing Z with the ring of the Eisenstein integers.

# Parameter Settings

* [HHHW09] P. Hirschhorn, J. Hoffstein, N. Howgrave-Graham and W. Whyte: Choosing NTRU Parameters in Light of Combined Lattice. (ACNS 2009)
    * A proposal of parameter setting algorithm considering the meet-in-the-middle attack.

# NTRU with A/W reduction [#ied160cc]

* [SS11-EC] Damien Stehle, Ron Steinfeld: Making NTRU as Secure as Worst-Case Problems over Ideal Lattices. EUROCRYPT 2011
    *  Secure NTRU in Z_q[X]/(X^n+1) from RingLWE.
* [SLP+12-PKC] Ron Steinfeld, San Ling, Josef Pieprzyk, Christophe Tartary, Huaxiong Wang: NTRUCCA: How to Strengthen NTRUEncrypt to Chosen-Ciphertext Security in the Standard Model. PKC 2012
    *  CCA2 version of [SS11-EC].

# Attacks

* [CS07] D. Coppersmith and A. Shamir: Lattice attacks on NTRU (EUROCRYPT 1997)
    * ...
* [Sil99] J. H. Silverman: A meet-in-the-middle attack on an NTRU private key. (NTRU Tech. Rep. #004-ver.2, 1999.)
    * Odlyzko's meet-in-the-middle attack and its improvement.
* [JJ00] &Eacute; Jaulmes and A. Joux: A chosen-ciphertext attack against NTRU. (CRYPTO 2000)
    *  
* [Gen01] C. Gentry: Key recovery and message attacks on NTRU-Composite. (EUROCRYPT 2001)
    * A 3-minute attack on NTRU-256 using a folding lattice technique.
* [NP02] P. Q. Nguyen and D. Pointcheval: Analysis and improvements of NTRU encryption paddings. (CRYPTO 2002)
    *  
* [Arn02] F. Arnault: Cryptanalyse de CTRU. (Talk, Dec., 2002)
    * An attack on CTRU [GOS02]. See [[Programme du groupe de travail &quot;Arithm&eacute;tique-Cryptographie-Codage 2002-2003&quot;:http://www.unilim.fr/laco/seminaires/ACC/archives03.html]]
* [HNP+03] N. Howgrave-Graham, P. Q. Nguyen, D. Pointcheval, J. Proos, J. H. Silverman, A. Singer, and W. Whyte: The impact of decryption failures on the security of NTRU encryption. (CRYPTO 2003)
    *  
* [HHHK03] D. Han, J. Hon, J. W. Han, and D. Kwon: Key recovery attacks on NTRU without ciphertext validation routine. (ACISP 2003)
    *  
* [SSV04] J. H. Silverman, N. P. Smart, and F. Vercauteren: An algebraic approach to NTRU (q=2n) via Witt vectors and overdetermined systems of nonlinear equations. (SCN 2004)
    *  
* [SSS04] T. E. Seidel, D. Socek, and M. Sramka: Parallel symmetric attack on NTRU using non-deterministic lattice reduction. (Designs, Codes and Cryptography, 32 (1-3), 2004)
    *  
* [GHN06] N. Gama, N. Howgrave-Graham, and P. Q. Nguyen: Symplectic lattice reduction and NTRU. (EUROCRYPT 2006)
    * Speeding up lattice reduction algorithms (?)
* [MR06] T. Meskanen and A. Renvall: A wrap error attack against NTRUEncrypt. (Discrete Applied Mathematics 154(2), 2006)
    *  
* [GN07] N. Gama and P. Q. Nguyen: New Chosen-Ciphertext Attacks on NTRU. (PKC 2007)
    *  
* [SW07] J. H. Silverman and W. Whyte: Timing attacks on NTRUEncrypt via variation in the number of hash calls.&ldquo; (CT-RSA 2007)
    *  
* [How07] N. Howgrave-Graham: A hybrid lattice-reduction and meet-in-the-middle attack against NTRU. (CRYPTO 2007)
    *  
* [MY08] P. Mol and M. Yung: Recovering NTRU secret key from inversion oracles.&ldquo; (PKC 2008)
    *  
* [Vat08] N. Vats: Algebraic cryptanalysis of CTRU cryptosystem. (COCOON 2008)
    * Third attack against CTRU [GOS02].
* [LSCH10] M.-K. Lee, J. E. Song, D. Choi, and D.-G. Han.  &ldquo;Countermeasures against Power Analysis Attacks for the NTRU Public Key Cryptosystem. (IEICE Transactions on Fundamentals of Electronics, Communications and Computer, Vol.E93-A No.1 (2010))
    *  
* [KY12-MoCrySEn] Abdel Alim Kamal, Amr Youssef: A Scan-Based Side Channel Attack on the NTRUEncrypt Cryptosystem. (MoCrySEn 2012)
    *  
* [YYXS14-SCIS] Yamaguchi, Yasuda, Xavier, Sakurai (in Japanese, SCIS 2014 2E3-4)
    *  Attack against [NSP08-ICON]

# Other Miscellaneous Results [#iccb2986]

* [NSW03] M. Naslund, I. Shparlinski, and W. Whyte: On the bit security of NTRUEncrypt. (PKC 2003)
    *  
* [LYP05] X. Lv, B. Yang, and C. Pei: Efficient Traitor Tracing Scheme Based On NTRU. (PDCAT 2005)
    *  
* [YHZ05] W. Yu, D. He, and S. Zhu: Study on NTRU decryption failures. (ICITA 2005)
    *  
* [Sta05] M. Stam: A key encapsulation mechanism for NTRU. (IMA Int. Conf. 2005)
    *  
* [LKSP07] M.-K. Lee, J. W. Kim, J. E. Song, and K. Park: Sliding window method for NTRU. (ACNS 2007)
    *  
* [BDL08] J. Buchmann, M. D&ouml;ring, and R. Lindner: Efficiency improvement for NTRU. (Sicherheit 2008)
    * I found the paper. See Lindner's website, http://www.cdc.informatik.tu-darmstadt.de/mitarbeiter/rlindner.html.
* [WZ08] S. Wei and Z. Zhuo: Research on PKI model based on NTRU. (ISECS 2008)
* [LKSP13-IEICE] Mun-Kyu LEE, Jung Woo KIM, Jeong Eun SONG, and Kunsoo PARK: Efficient Implementation of NTRU Cryptosystem Using Sliding Window Methods. IEICE TRANSACTIONS on Fundamentals of Electronics, Communications and Computer Sciences, Vol.E96-A, No.1, pp.206-214
    * 
