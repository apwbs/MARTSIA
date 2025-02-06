# MARTSIA

**Multi-Authority Approach to Transaction Systems for Interoperating Applications**  
**** 

MARTSIA is a decentralized approach for secrecy-preserving, immutable, access-controlled information exchange via public blockchain for process management. 
In short, it resorts to Multi-Authority Ciphertext Policy Attributed Based Encryption (MA-CP-ABE) to handle the ciphering/deciphering cycle, a content-addressed Distributed Hash Table (DHT) file system (IPFS) to handle the storage of documents, and smart contracts to enforce the access grants and notarise the data flow.

Several actors cooperate in a process execution within the framework: _(i)_ the **Data Owner**, who encrypts data using an MA-CP-ABE policy; _(ii)_ the **Reader**, who intends to decrypt it; _(iii)_ the **Attribute Certifier**, who assigns MA-CP-ABE attributes to the Readers;  and _(iv)_ the **Authority Network**, a set of Authorities responsible for generating segments of decryption keys for the Reader. Using these keys, the Reader can decrypt the data.

MARTSIA comes implemented in two versions:
- [MARTSIA-Demo](https://github.com/apwbs/MARTSIA-Demo) employs EVM-based blockchain platforms as its backbone;
- [MARTSIA-Algorand](https://github.com/apwbs/MARTSIA-Algorand) adopts Algorand and its AVM.

All the other variants of our framework are available and listed below.

## Blockchain-based key exchange
 
We have also designed an alternative scheme for the request and transmission of key segments that uses the blockchain itself as a backbone.
Please find it implemented in [EVM](https://github.com/apwbs/MARTSIA-EVM-OnChain) and [Algorand](https://github.com/apwbs/MARTSIA-Algorand-KoB).

## Multi-signature smart contracts

Furthermore, we provide alternative versions of the smart contract requiring multiple signatures to enable operations.
The code for the Algorand platform is available in this repository [MARTSIA-Algorand-CSC](https://github.com/apwbs/MARTSIA-Algorand-CSC).

## Literature and links
For more information on MARTSIA, please consult our paper entitled "[MARTSIA: Enabling Data Confidentiality for Blockchain-based Process Execution](https://arxiv.org/abs/2303.17977)" accepted at 
[EDOC 2023](https://www.rug.nl/research/bernoulli/conf/?lang=en) and published with DOI [10.1007/978-3-031-46587-1_4](https://doi.org/10.1007/978-3-031-46587-1_4). 
Please find the presented slides on [SlideShare](https://www.slideshare.net/EdoardoMarangone/martsia-enabling-data-confidentiality-for-blockchainbased-process-execution).

An extended version of the above paper entitled is available on arXiv: "[Enabling Data Confidentiality with Public Blockchains](https://arxiv.org/abs/2308.03791)" (currently under review).

An additional paper titled "[MARTSIA: Safeguarding Data Confidentiality in Blockchain-Driven Process Execution](https://arxiv.org/abs/2407.10684)" is available on arXiv. 

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
