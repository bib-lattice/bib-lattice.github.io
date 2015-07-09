---
layout: posts
title: Other Protocols
---


# OT

* [PVW08-C] Chris Peikert, Vinod Vaikuntanathan, and Brent Waters: A framework for efficient and composable oblivious transfer. CRYPTO 2008
    * UC-secure OT from LWE; static corruption, single-use CRS.

# PIR [#z91dba40]

# NISZK [#i3bcfc4f]

* [PV08-C] Chris Peikert and Vinod Vaikuntanathan: Noninteractive statistical zero-knowledge proofs for lattice problems. CRYPTO 2008
    * NISZK for SIVP, GapCRP, GapGSMP, and coGapSVP with approximation factors O~(\sqrt{n}).

# KE [#z8fe9526]

* Ruckert and Peikert: CT-RSA
    *  It mentioned a simple key exchange from LWE, although there is no proof on correctness and security.
* [Ding12-eP] Jintai Ding: A Simple Provably Secure Key Exchange Scheme Based on the Learning with Errors Problem. [[ePrint 2012/688:http://eprint.iacr.org/2012/688]]
    *  I cannot agree his proof.
* [Geo13-Tatra] Adela Georgescu: An LWE-based key transfer protocol with anonymity. [[Tatra Mountains Mathematical Publications. Vol. 53, Issue 1:http://www.degruyter.com/view/j/tmmp.2012.53.issue-1/v10127-012-0042-8/v10127-012-0042-8.xml]]
    *  I cannot agree the correctness of ``An LWE Diffie-Hellman Key Exchange.''
* [BCDP13-eP] Olivier Blazy and C&eacute;line Chevalier and L&eacute;o Ducas and Jiaxin Pan: Errorless Smooth Projective Hash Function based on LWE. [[ePrint 2013/821:https://eprint.iacr.org/2013/821]]
    *  Now, I can agree the proof. the ratio B/q matters.

# PAKE [#a08c0bc3]

* [KV09-AC] Jonathan Katz and Vinod Vaikuntanathan: Password-based authenticated key exchange based on lattices. ASIACRYPT 2009
    *  3-move in the BPR model
* [DF11-CIS] Yi Ding and Lei Fan: Efficient Password-Based Authenticated Key Exchange from Lattices. 
    *  3-move in the BPR model
* [BCDP13-eP] Olivier Blazy and C&eacute;line Chevalier and L&eacute;o Ducas and Jiaxin Pan: Errorless Smooth Projective Hash Function based on LWE. [[ePrint 2013/821:https://eprint.iacr.org/2013/821]]
    *  q is superpolynomial
    *  2-move in the BPR model
    *  3-move in the UC model


# AKE [#x835e729]

* [FSXY12-PKC] Atsushi Fujioka, Koutarou Suzuki, Keita Xagawa, Kazuki Yoneyama: Strongly Secure Authenticated Key Exchange from Factoring, Codes, and Lattices. PKC 2012, [[ePrint 2012/211:http://eprint.iacr.org/2012/211]]
    * In the standard model.
* [FSXY13-ASIACCS] ... 
    * In the ROM.

# Secret Sharing [#u105f1b2]

* [Geo11-IJCA] Adela Georgescu: A LWE-based Secret Sharing Scheme. [[IJCA Special Issue on Network Security and Cryptography NSC(3), pp.27-29, December 2011:http://www.ijcaonline.org/specialissues/nsc/number3/4339-spe035t]]
    * She (I think she) proposed an n-out-of-n secret sharing based on LWE. Let us consider a large prime p and a generator g of GF(p). (Note: She seems to set q as an order of <g> implicitly).
    * Consider a secret s in Z_q^d.
        * For i = 1,..,d-1, we choose (a_i,b_i) = (a_i, a_i s_i + e_i) as an LWE sample.
        * For i = d, we set (a_d, b_d) = (a_d, a_d s_d + e_d), where e_d = -(e_1+e_2+...+e_{d-1}).
    * A share for i is S_i = (g^{a_i}, g^{b_i}).
* [BM12-WISTP] Rachid El Bansarkhani and Mohammed Meziani: An Efficient Lattice-Based Secret Sharing Construction. WISTP 2012
    *  verifiable secret sharing.
