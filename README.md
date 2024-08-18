# Medi_Chain
## Inspiration
For decades, medical records are under the ownership of hospitals. It often it takes days to request a hospital to transfer a record, and sometimes impossible to transfer across states/countries.

We want to change that. And that’s why we created MediChain - a true ownership of our medical records powered by blockchain technology.

## What it does
MediChain is a blockchain-based electrical medical records (EMR) decentralized application (Dapp).

MediChain is powered by IPFS, where patients’ medical records are stored on the distributed file system, not owned by any centralized entity. A patient can access his or her records by interacting with a smart contract on the Ethereum blockchain, forming a digital identity of the patient on the decentralized network.

A healthcare provider can register using a crypto wallet like Metamask. The healthcare provider can register a patient by using the public address of the patient’s wallet , usually provided during an appointment.

The health provider can search for a patient’s records using the address, and upload a new record for the patient. The patient can also view his or her records, after connected with a wallet which address is registered by the health provider.

## How we built it
There are three major components of MediChain:

1. React client (connected with crypto wallet)
2. Solidity smart contract on Ethereum (ETH) blockchain
3. Interplanetary file system (IPFS)
The client first connects with crypto wallet, and use smart contract to mint a patient or doctor block if the public address of the user’s wallet is not registered.

The client can upload a record file to IPFS, which address is linked to a patient block in ETH chain. The client can get all record addressed stored in a patient block from smart contract, and get a record file by its address from IPFS.
