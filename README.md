# MARTSIA: Multi-Authority Approach to Transaction Systems for Interoperating Applications

This is the master and principal GitHub repo of the Multi-Authority Approach to Transaction Systems for Interoperating 
Applications (MARTSIA) project. From here you will be redirected to all the available repos.
The MARTSIA approach is presented in two papers. The first one is 
"[MARTSIA: Enabling Data Confidentiality for Blockchain-based Process 
Execution](https://arxiv.org/abs/2303.17977)" accepted at 
[EDOC 2023](https://www.rug.nl/research/bernoulli/conf/?lang=en). [DOI](https://doi.org/10.1007/978-3-031-46587-1_4) of the conference (to appear). 
The second paper about MARTSIA, that extends the work done in the first one, is 
"[Enabling Data Confidentiality with Public Blockchains](https://arxiv.org/abs/2308.03791)".

MARTSIA is implemented in Ethereum and Algorand. The first implementation is the one where the keys are exchanged via a
client-server Secure Sockets Layer (SSL) connection. Here you can find the 
[Ethereum](https://github.com/apwbs/MARTSIA-Ethereum) implementation and the 
[Algorand](https://github.com/apwbs/MARTSIA-Algorand) one. 
In the Ethereum repo there is a folder called "caterpillar-interaction" where you can find all the necessary to run 
MARTSIA-Ethereum along with
[Caterpillar](https://github.com/orlenyslp/Caterpillar) as explained in the papers.

The second implementation is the one where the keys are exchanged via blockchain. Here you can find the 
[Ethereum](https://github.com/apwbs/MARTSIA-Ethereum-KoB) implementation and the 
[Algorand](https://github.com/apwbs/MARTSIA-Algorand-KoB) one.

The third implementation is the one where the smart contracts control the access and the behavior of the users. Here you 
can find the 
[Ethereum](https://github.com/apwbs/MARTSIA-Ethereum-CSC) implementation and the 
[Algorand](https://github.com/apwbs/MARTSIA-Algorand-CSC) one. 