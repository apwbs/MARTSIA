# MARTSIA: Multi-Authority Approach to Transaction Systems for Interoperating Applications

MARTSIA (Multi-Authority Approach to Transaction Systems for Interoperating Applications) is an approach for secrecy-preserving, immutable, access-controlled information exchange via public blockchain for process management. In short, it resorts to Multi-Authority Ciphertext Policy Attributed Based Encryption (MA-CP-ABE) to handle the ciphering/deciphering cycle, a content-addressed Distributed Hash Table (DHT) file system (IPFS) to handle the storage of documents, and smart contracts to enforce the access grants and notarise the data flow.

MARTSIA comes implemented in two versions:
- [MARTSIA/Ethereum](https://github.com/apwbs/MARTSIA-Ethereum) employs Ethereum and other EVM-based blockchain platforms as its backbone;
- [MARTSIA/Algorand](https://github.com/apwbs/MARTSIA-Algorand) adopts Algorand and its AVM.
Other variants of our platforms are available and listed below.

The approach is presented in 
“[MARTSIA: Enabling Data Confidentiality for Blockchain-based Process 
Execution](https://arxiv.org/abs/2303.17977)” accepted at 
[EDOC 2023](https://www.rug.nl/research/bernoulli/conf/?lang=en) and published with DOI [10.1007/978-3-031-46587-1_4](https://doi.org/10.1007/978-3-031-46587-1_4). 
Please find the presented slides on [SlideShare](https://www.slideshare.net/EdoardoMarangone/martsia-enabling-data-confidentiality-for-blockchainbased-process-execution).
An extended version of the paper is available on arXiv: 
“[Enabling Data Confidentiality with Public Blockchains](https://arxiv.org/abs/2308.03791)”.

## Client-server key exchange

By default, MARTSIA resorts to a
Secure Sockets Layer (SSL) client-server connection
to exchange decryption keys.

This scheme is employed to integrate MARTSIA with an existing blockchain-based process execution platform.
The folder named `caterpillar-interaction` in the
[MARTSIA-Ethereum](https://github.com/apwbs/MARTSIA-Ethereum) repository 
contains an integrated porting of
[Caterpillar](https://github.com/orlenyslp/Caterpillar)
with MARTSIA (please read our [paper](https://arxiv.org/abs/2303.17977) for more information).

## Blockchain-based key exchange
We have also designed an alternative scheme for the exchange
that uses the blockchain itself as a backbone.
Please find it implemented in
[Ethereum](https://github.com/apwbs/MARTSIA-Ethereum-KoB)
and [Algorand](https://github.com/apwbs/MARTSIA-Algorand-KoB).

## Multi-signature smart contracts

Furthermore, we provide alternative versions of the smart contracts
requiring multiple signatures to enable operations.
Again, the code is available for both the
[Ethereum](https://github.com/apwbs/MARTSIA-Ethereum-CSC) and
[Algorand](https://github.com/apwbs/MARTSIA-Algorand-CSC) platforms.

## Demo
The repository with the MARTSIA-demo paper and its corresponding code, video and Wiki is available at
[MARTSIA-demo](https://github.com/apwbs/MARTSIA-demo).

Along with the MARTSIA demo, you can find a video presentation of its usage:
[MARTSIA demo video](https://www.youtube.com/watch?v=RAcifWw1_B0)

## Citation
If you liked our approach, are using it as a building block of your tool or are considering it for your related work,
feel free and welcome to cite our manuscript!
Please find the BibTeX below for convenience:
```
@InProceedings{   Marangone.etal/EDOC2023:MARTSIA,
  author        = {Marangone, Edoardo and Di Ciccio, Claudio and Friolo,
                  Daniele and Nemmi, Eugenio Nerio and Venturi, Daniele and
                  Weber, Ingo},
  booktitle     = {EDOC},
  title         = {{MARTSIA}: Enabling Data Confidentiality for
                  Blockchain-based Process Execution},
  year          = {2023},
  pages         = {58--76},
  series        = {Lecture Notes in Computer Science},
  crossref      = {EDOC2023},
  doi           = {10.1007/978-3-031-46587-1_4}
}
@Proceedings{     EDOC2023,
  title         = {Enterprise Design, Operations, and Computing - 27th
                  International Conference, {EDOC} 2023, Groningen, The
                  Netherlands, October 30 - November 3, 2023, Proceedings},
  year          = {2024},
  editor        = {Henderik A. Proper and Luise Pufahl and Dimka
                  Karastoyanova and van Sinderen, Marten and Jo{\~{a}}o L. R.
                  Moreira},
  isbn          = {978-3-031-46586-4},
  publisher     = {Springer},
  series        = {Lecture Notes in Computer Science},
  volume        = {14367}
}
```
