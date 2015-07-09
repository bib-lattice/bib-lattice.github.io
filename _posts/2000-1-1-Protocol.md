---
layout: post
title: Protocols
---

# Identificaitons

## With average-case/worst-case reductions

* [MV03-C] D. Micciancio and S. Vadhan: Statistical zero-knowledge proofs with efficient provers: lattice problems and more. CRYPTO 2003
    *  Combining with MR07, we have ID schemes based on GapSVP with approximation factor O~(n^{1.5})
    *  basic: 3-round, SZK, (0,1/2+eps)
* [Lyu08-PKC] Vadim Lyubashevsky: Lattice-based identification schemes secure under active attacks. PKC 2008
    * Concurrently-secure ID schemes based on GapSVP or Ideal-SVP with approximation factor O~(n^2)
    *  basic: 3-round, WI, (1/e, eps)
* [Lyu08-Thesis] Vadim Lyubashevsky: Towards Practical Lattice-Based Cryptography. Ph.D Thesis
    * Concurrently-secure ID schemes based on Ideal-SVP with approximation factor O~(n^3)
* [KTX08-AC] Akinori Kawachi, Keisuke Tanaka, and Keita Xagawa: Concurrently secure identification schemes based on the worst-case hardness of lattice problems. ASIACRYPT 2008
    * ID schemes based on GapSVP or Ideal-SVP with approximation factor O~(n). Using Stern's scheme (CRYPTO 1993).
    *  basic: 3-round, SZK, (0,2/3+eps)
* [Lyu09-AC] Vadim Lyubashevsky: Fiat-Shamir With Aborts: Applications to Lattice and Factoring-Based Signatures. ASIACRYPT 2009
    * Concurrently-secure ID schemes based on Ideal-SVP with approximation factor O~(n^2)
    *  3-round, WI, (1/e,eps)
* [SSTX09-AC] 
    *  Identity-based Identification in the ROM. (GPV IBE + MV ZKPoK)
* [Xag10-Thesis] Keita Xagawa. Cryptography with Lattices. Ph.D Thesis
    *  Concurrently secure, 3-round,  ID schemes based on Trapdoor Hash.
    *  3-round, HVSZK, (0,eps)
* [Ruc10-SCN] Markus R&uuml;ckert. Adaptively Secure Identity-Based Identification from Lattices without Random Oracles. SCN 2010
    *  basic: 3-round, SZK, (0,2/3+eps)?
* [CLRS10-ProvSec] Pierre-Louis Cayrel, Richard Lindner, Markus R&uuml;ckert, and Rosemberg Silva: Improved Zero-knowledge Identification with Lattices. ProvSec 2010, Tatra Mountains Mathematical Publications, Volume 53, Issue 1, Pages 33?63, February 2013.
    *  basic: 5-round, SZK, (0,(q+1)/(2q)+eps)
* [CLRS10-Latincrypt] Pierre-Louis Cayrel, Richard Lindner, Markus R&uuml;ckert, and Rosemberg Silva: A Lattice-Based Threshold Ring Signature Scheme. LATINCRYPT 2010
* [SCL11-ITW] Rosemberg Silva, Pierre-Louis Cayrel, and Richard Lindner: A Lattice-Based Batch Identification Scheme. ITW 2011
* [Lyu12-EC] Vadim Lyubashevsky: Lattice signatures without trapdoors. Eurocrypto 2012
* [AFLT12-EC] Michel Abdalla, Pierre-Alain Fouque, Vadim Lyubashevsky, Mehdi Tibouchi. Tightly-secure signatures from lossy identification schemes. Eurocrypt 2012
* [LNSW13-PKC] San Ling, Khoa Nguyen, Damien Stehl&eacute;, and Huaxiong Wang: Improved Zero-knowledge Proofs of Knowledge for the ISIS Problem, and Applications. PKC 2013
* [DDLL13-C] L&eacute;o Ducas, Alain Durmus, Tancr&egrave;de Lepoint, and Vadim Lyubashevsky: Lattice Signatures and Bimodal Gaussians. CRYPTO 2013, [[ePrint 2013/383:http://eprint.iacr.org/2013/383]]

## Without average-case/worst-case reductions

* [HT08] Shunichi Hayashi, Mitsuru Tada: A Digital Signature Scheme Based on NP-Complete Lattice Problems. IEICE Transactions 91-A(5): 1253-1264 (2008)
    * ID scheme based on Non-negative Binary Exact Length Vector Problem (NBELVP) in the l_{1} norm.
* [XT09-ProvSec] Kieta Xagawa and Keisuke Tanaka: Zero-Knowledge Protocols for NTRU: Application to Identification and Proof of Plaintext Knowledge. ProvSec 2009
    * SZKPOK for NTRU

# Protocols

* [GK05] S. Goldwasser and D. Kharchenko: Proof of plaintext knowledge for the Ajtai-Dwork cryptosystem. (TCC 2005)
    * A variant of the AD PKE with proof of plaintext knowledge.
* [XKT07] K. Xagawa, A. Kawachi, K. Tanaka: Proof of plaintext knowledge for the Ajtai-Dwork cryptosystem. ([[TR C-236:http://www.is.titech.ac.jp/research/research-report/C/C-236.pdf]], 2007)
    * Two variants of the Regev 03 and the Regev 05 PKEs with proofs of plaintext knowledge.
* [BD10-TCC] Rikke Bendlin and Ivan Damg&aring;rd. Threshold decryption and zero-knowledge proofs for lattice-based cryptosystems. TCC 2010
    * A proof for plaintext knowledge for Reg05 with subexponential parameters.
* [BDOZ11-EC] Rikke Bendlin, Ivan Damg&aring;rd, Claudio Orlandi, and Sarah Zakarias. Semihomomorphic encryption and multiparty computation. EUROCRYPT 2011, [[ePrint 2010/514:http://eprint.iacr.org/2010/514]]
* [AJLATVW12-EC] Gilad Asharov, Abhishek Jain, Adriana L&oacute;pez-Alt, Eran Tromer, Vinod Vaikuntanathan, and Daniel Wichs. Multiparty computation with low communication, computation and interaction via threshold FHE. EUROCRYPT 2012, [[ePrint 2011/613, Asharov, Jain and Wichs:http://eprint.iacr.org/2011/613]], 
    * -See section F.2 and F.3 of 2011/613 for gap \Sigma protocols.
* [DL12-SCN] Ivan Damg&aring;rd and Adriana L&oacute;pez-Alt: Zero-Knowledge Proofs with Low Amortized Communication from Lattice Assumptions. SCN 2012
