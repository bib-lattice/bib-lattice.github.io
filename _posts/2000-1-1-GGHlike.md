---
layout: post
title: GGH and its variants
---

# Proposals

* [GGH97-C-Pub] Oded Goldreich, Shafi Goldwasser, and Shai Halevi: Public-key cryptosystem from lattice reduction problems. CRYPTO 1997, ECCC 1997
    * ...
* [NS98GGH-EL] DaeHun Nyang and JooSeok Song: Method for hiding information in lattice. Electronics Letters Vol.34, Issue 23. (1998)
    * A variant changing a plaintext encode GGH.
* [Mic01-CaLC] Daniele Micciancio: Improving lattice based cryptosystems using the Hermite normal form. CaLC 2001
    * Reducing the size of pk in [GGH97-C-Pub] by using HNF.
* [SCM01] P. Sole, C. Charnes, and B. Martin: A lattice-based McEliece scheme for encryption and signature. Electronic Notes in Discrete Mathematics, vol. 6, 2001
    * Rediscovery of [GGH97-C-Pub].
* [PJH03-PKC] Seong-Hun Paeng, Bae Eun Jung, Kil-Chan Ha: A Lattice Based Public Key Cryptosystem Using Polynomial Representations. PKC 2003
    * Reducing the size of keys in [GGH97-C-Pub] using circulant matrices.
* [PRS09-QuantumCom] T. Plantard, M. Rose, W. Susilo: Improvement of lattice-based cryptography using CRT. QuantumComm 2009
    * Improved versions of GGH and [Mic01-CaLC].
* [YK12-ISITA] Masayuki Yoshino, Noboru Kunihiro: Improving GGH cryptosystem for large error vector. ISITA 2012

Note: NTRU and the dual Regev encryption with strong trapdoor can be considered as special case of the GGH cryptosystem.

# Attacks

* [Ngu97-C] Phong. Q. Nguyen: Cryptanalysis of the Goldreich-Goldwasser-Halevi cryptosystem from CRYPTO '97. (CRYPTO 1999)
    * Attacks succeed up to n=350 for challenges in [GGH97-C-Pub]
* [HKY07-PKC] Daewan Han, Myung-Hwan Kim, Yongjin Yeom: Cryptanalysis of the Paeng-Jung-Ha cryptosystem from PKC 2003. PKC 2007
    * Attacks succeed up to n=1000 for [PJH03-PKC].
* [LH10-MiCS] Moon Sung Lee, Sang Geun Hahn: Cryptanalysis of the GGH Cryptosystem. Mathematics in Computer Science 3(2): 201-208 (2010), SCC 2008
    * Attack with partially known plaintext. They solved the 400-dimensional challenge in [GGH97-C-Pub] with help of Nguyen's results [Ngu97].

