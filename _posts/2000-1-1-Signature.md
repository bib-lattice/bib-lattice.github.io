# with average-case/worst-case reductions

* [GPV08-STOC] C. Gentry, C. Peikert, and V. Vaikuntanathan. &ldquo;Trapdoors for hard lattices and new cryptographic constructions.&rdquo; (STOC 2008, http://eprint.iacr.org/2007/432 )
    * sEUF-CMA secure signature in ROM based on GapSVP with approximation factor O~(n^2) or O~(n^3)
* [LM08-TCC] V. Lyubashevsky and D. Micciancio. &ldquo;Asymptotically efficient lattice-based digital signatures.&rdquo; (TCC 2008)
    * One-time signature based on Ideal-SVP with approximation factor O~(n^2).
* [AP09-STACS] J. Alwen and C. Peikert. &ldquo;Generating Shorter Bases for Hard Random Lattices.&rdquo; (STACS 2009, TCS 2010, http://eprint.iacr.org/2008/521 )
    * Improving [[[Ajt99].
* [SSTX09-AC] D. Stehl&eacute;, R. Steinfeld, K. Tanaka, and K. Xagawa. &ldquo;Efficient public key encryption based on ideal lattices.&rdquo; (ASIACRYPT 2009, http://eprint.iacr.org/2009/285 )
    * Ideal-lattice versions of the Alwen    * Peikert constructions.
* [Boy10-PKC] X. Boyen. &ldquo;Of lettuces of lattices : a framework for short signatures and IBE with full security.&rdquo; (PKC 2010)
    * Merged. See the full version of [[[ABB10-EC].
* [Ruc10-PQCrypto] M. R&uuml;ckert. &ldquo;Strongly Unforgeable Signatures and Hierarchical Identity-based Signatures from Lattices without Random Oracles.&rdquo; (PQCrypto 2010, http://eprint.iacr.org/2010/070 )
    * An improvement of [[[CHKP10-?]
* [BF11-PKC] D. Boneh and D. Mandell Freeman. &ldquo;Linearly Homomorphic Signatures over Binary Fields and New Tools for Lattice-Based Signatures.&rdquo; (PKC 2011, http://eprint.iacr.org/2010/453 )
* [MP12-EC] Micciancio and Peikert.
    *  As an applicaiton, they proposed a wCMA-secure signature scheme. A proof is based on the argument similar to Hohenberger and Waters, and CHKP10.

For signature schemes based on the Fiat-Shamir transformations, see [[Identification]].

* [GCZ12-WISM] Chunxiang Gu, Li Chen, and Yonghui Zheng. &ldquo;ID-Based Signatures from Lattices in the Random Oracle Model.&rdquo; (WISM 2012)
    *  Combining [[[ABB10-C] + [[[GPV08-STOC]

## Implementations

* [GOPS13-PQC] Tim Guneysu and Tobias Oder and Thomas Poppelmann and Peter Schwabe: Software Speed Records for Lattice-Based Signatures. PQCrypto 2013.


## Extensions

### Ring Signatures

* [KTX08-AC]
    *  Ring Sig. from the KTX ad-hoc ID.
* [BK10-eP] Z. Brakerski and Y. Tauman Kalai. &ldquo;A Framework for Efficient Signatures, Ring Signatures and Identity Based Encryption in the Standard Model.&rdquo; (http://eprint.iacr.org/2010/086 )
    *  Based on the CHKP sig.
* [CLRS10-Latincrypt] P.-L. Cayrel, R. Lindner, M. R&uuml;ckert, and R. Silva. &ldquo;A Lattice-Based Threshold Ring Signature Scheme.&rdquo; (LATINCRYPT 2010)
    *  Another twist of ...
* [Wang10-eP] J. Wang. &ldquo;Ring Signature and Identity-Based Ring Signature from Lattice Basis Delegation.&rdquo; (http://eprint.iacr.org/2010/378 )
    *  ???
* [WS11-ICICS] Jin Wang and Bo Sun: Ring Signature Schemes from Lattice Basis Delegation. ICICS 2011
    * (1) Based on the GPV Sig in the ROM. (2) Based on the Boyen Sig in the StdM.
* [JS13-PQC] Schrek Julien and Bettaieb Slim: Improved Lattice-Based Threshold Ring Signature Scheme. PQCrypto 2013.
* [AMBBFG13-Africacrypt] Carlos Aguilar Melchor, Slim Bettaieb, Xavier Boyen, Laurent Fousse, and Philippe Gaborit: Adapting Lyubashevsky’s Signature Schemes to the Ring Signature Setting. Africacrypt 2013


### Blind Signature

* [Ruc10-AC] M. R&uuml;ckert: Lattice-based Blind Signatures. ASIACRYPT 2010, [[ePrint 2008/322:http://eprint.iacr.org/2008/322]]
    * See the version 2010/02/26.
* [GCZ12-WISM] Chunxiang Gu, Li Chen, and Yonghui Zheng. &ldquo;ID-Based Signatures from Lattices in the Random Oracle Model.&rdquo; (WISM 2012)
    *  Combining [[[ABB10-C] + [[[GPV08-STOC]. They also proposed ID-based blind sig. in the ROM.


### Group Signature and more 

* [GKV10-AC] D. Gordon, J. Katz, and V. Vaikuntanathan. &ldquo;A group singnature scheme from lattice assumptions.&rdquo; (ASIACRYPT 2010, http://eprint.iacr.org/2011/060 )
    * A (static) group signature scheme from LWE and SIS in the ROM.
* [CNR12-SCN] Jan Camenisch, Gregory Neven, and Markus Ruckert &ldquo;Fully Anonymous Attribute Tokens from Lattices.&rdquo; (SCN 2012)
    * ... from LWE and SIS in the ROM. 


# GGH

## Proposal

* [GGH97-C] O. Goldreich, S. Goldwasser, and S. Halevi. &ldquo;Public-key cryptosystem from lattice reduction problems.&rdquo; (CRYPTO 1997, ECCC 1997)
    * ...
* [PSW08-PKC] T. Plantard, W. Susilo, and K. T. Win. &ldquo;A digital signature scheme based on CVP_{\infty}.&rdquo; (PKC 2008)
    * A variant of the GGH signature scheme based on CVP_{\infty}. It seems resist the Nguyen    * Regev attack.
* [PSWH08-IJAC] T. Plantard, W. Susilo, K. T. Win, Q. Huang. &ldquo;Efficient lattice-based signature scheme.&rdquo; (International Journal of Applied Cryptography 2008)
    * The journal version of [[[PSW08-PKC]

## Attacks

* [NR06-EC] P. Q. Nguyen and O. Regev. &ldquo;Learning a parallelepiped: Cryptanalysis of GGH and NTRU signatures.&rdquo; (EUROCRYPT 2006)
    * Attacks on GGH and NTRU with about 90000 signatures

# NTRU (NSS, R-NSS, NTRUSign)

## Proposal

* Pre-NSS (The rump session of CRYPTO 2000)
* [HPS01-EC] J. Hoffstein, J. Pipher, and J. H. Silverman. &ldquo;NSS: An NTRU lattice-based signature scheme.&rdquo; (EUROCRYPT 2001)
* R-NSS (The rump session of EUROCRYPT 2001, Draft 2.0 of EESS#1)
* [HHPSW03-CTRSA] J. Hoffstein, N. Howgrave-Graham, J. Pipher, J. H. Silverman, and W. Whyte. &ldquo;NTRUSign: Digital signatures using the NTRU lattice.&rdquo; (CT-RSA 2003)
* [HWH08-IEEEIT] Y. Hu, B. Wan, and W. He. &ldquo;NTRUSign with a new perturbation.&rdquo; (IEEE Transactions on Information Theory, vol.54, 2008)
* [MA09-eP] Chunbo Ma and Jun Ao. &ldquo;NTRU based group oriented signature.&rdquo; http://eprint.iacr.org/2009/498
* [MA10-ETCS] Chunbo Ma and Jun Ao. &ldquo;NTRU Based Group Oriented Signature and its Applications in RFID.&rdquo; (ETCS 2010)


## Attacks

* [Mir01-eP] I. Mironov &ldquo;A note on cryptanalysis of the preliminary version of the NTRU Signature Scheme.&rdquo; (ePrint 2001/005)
    * Attack on Pre-NSS
* [GJSS01-AC] C. Gentry, J. Jonsson, J. Stern, and M. Szydlo &ldquo;Cryptanalysis of the NTRU Signature Scheme (NSS) from EUROCRYPT 2001&rdquo; (The rump session of EUROCRYPT 2001, ASIACRYPT 2001)
    * Attacks on NSS
* [GS02-EC] C. Gentry and M. Szydlo. &ldquo;Cryptanalysis of the revised NTRU signature scheme.&rdquo; (EUROCRYPT 2002)
    * Attacks on R-NSS
* [Szy03-EC] M. Szydlo. &ldquo;Hypercubic lattice reduction and analysis of GGH and NTRU signatures.&rdquo; (EUROCRYPT 2003)
    * ...
* [MYK04-ACISP] S. J. Min, G. Yamamoto, and K. Kim. &ldquo;Weak property of malleability in NTRUSign.&rdquo; (ACISP 2004)
    * Proposal of strongly existential forgery against NTRUSign.
* [NR06-EC] P. Q. Nguyen and O. Regev. &ldquo;Learning a parallelepiped: Cryptanalysis of GGH and NTRU signatures.&rdquo; (EUROCRYPT 2006)
    * Attacks on NTRUSign without perturbations.
* [DN12-AC] Leo Ducas and Phong Q. Nguyen &ldquo;Learning a Zonotope and More: Cryptanalysis of NTRUSign Countermeasures.&rdquo; (ASIACRYPT 2012)
    * Attacks on NTRU with pertuabations (or deformations [[[HWH08-IEEEIT]).
