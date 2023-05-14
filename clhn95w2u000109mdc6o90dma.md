---
title: "An Overview of Hyperledger Fabric 2.0: Components, Architecture, and Features"
seoTitle: "Hyperledger Fabric 2.0: A Guide to Components, Architecture,Features"
seoDescription: "Discover Hyperledger Fabric 2.0, a modular and scalable distributed ledger technology platform for enterprise blockchain apps with key components,features."
datePublished: Sun May 14 2023 10:07:39 GMT+0000 (Coordinated Universal Time)
cuid: clhn95w2u000109mdc6o90dma
slug: an-overview-of-hyperledger-fabric-20-components-architecture-and-features
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1684056139580/778a5cad-36cc-4001-8d4e-940d2675ae76.webp
tags: blockchain, hyperledger, wemakedevs

---

## Introduction

Hyperledger Fabric is a blockchain platform designed for developing enterprise-grade decentralized applications. It is a powerful and flexible blockchain technology that enables enterprises to build secure, scalable, and decentralized applications. Fabric is part of the Hyperledger family of blockchain frameworks, which is hosted by the Linux Foundation. Other frameworks of Hyperledger are - Burrow, Indy, Iroha, Grid and Sawtooth.

Fabric was created for permissioned networks, as opposed to open blockchains like Bitcoin or Ethereum, where anybody may see the data and take part in consensus. For use cases where privacy, scalability, and regulatory compliance are crucial, Fabric is therefore well-suited. Because of Fabric's modular architecture, developers can modify and expand the platform to match the unique requirements of their applications. It also enables "chaincode" or smart contracts to be written in many other programming languages, such as Go, JavaScript, and Java.

This blog provides a comprehensive overview of the main components, architecture, and features of Hyperledger Fabric 2.0.

## Components of Hyperledger Fabric 2.0

Hyperledger Fabric 2.0 is composed of several key components -

1. **Ledger:** A ledger is a distributed database that keeps track of all transactions and the network's status. Different ledger types can be employed for various use cases because the ledger is designed to be modular.
    
2. **Chaincode:** Chaincode is the smart contract or business logic layer in the Hyperledger Fabric architecture. It is a program that defines the rules for the blockchain network and executes transactions. Chaincode can be written in multiple programming languages like Go, JavaScript, and Java.
    
3. **Channel:** A channel is a private and secure area of a Hyperledger Fabric blockchain network where users can conduct secure and private transactions. With the help of Hyperledger Fabric 2.0, many participant groups can share data in a private, confidential manner and communicate through a variety of methods.
    
4. **Peers**: The network's nodes are referred to as peers. They run smart contracts and keep a copy of the ledger. Endorsing peers and committed peers are the two different categories of peers in Hyperledger Fabric 2.0.
    
    * **Endorsing Peer:** An endorsing peer is responsible for executing chaincode and simulating transactions to ensure they meet the required endorsement policy.
        
    * **Committing Peer:** A committing peer is responsible for committing validated transactions to the ledger and maintaining a copy of the ledger.
        
5. **Ordering Service:** Creating blocks that are added to the ledger and organizing transactions are the responsibilities of the ordering service. It guarantees a consistent view of the ledger across all network nodes.
    
6. **Membership service provider (MSP):** The MSP is in charge of overseeing network access control and identity management. It establishes the guidelines for node and user access to the network.
    
7. **Certificate Authority:** Digital certificates for network users are issued and managed by a Certificate Authority (CA). The CA provides a safe system for the distribution of public keys, guarantees the legitimacy of the network users, and encrypts all communication.
    

## Architecture of Fabric 2.0

The architecture is divided into five main layers:

1. **Application Layer:** Applications that communicate with the blockchain network are included in the application layer. Applications that use APIs to communicate with the Hyperledger Fabric network are included in the application layer. The SDKs (Software Development Kits) offer these APIs, which allow programmers to create unique blockchain applications.
    
2. **Smart Contract Layer:** This layer consists of chaincode. All the rules and logic of the blockchain network are established here.
    
3. **Consensus Layer:** This layer contains the consensus method that is employed to make sure that every node on the network is in agreement regarding the ledger's current state. The pluggable consensus method employed by Hyperledger Fabric 2.0 enables the adoption of several consensus algorithms depending on the particular network requirements. The Raft consensus algorithm is the default mechanism for reaching consensus in Hyperledger Fabric 2.0. Other consensus mechanisms are Kafka and Solo.
    
    * **Raft:** Raft is a consensus algorithm that is used to manage a replicated log. Raft is a crash fault-tolerant consensus algorithm that can tolerate up to (N-1)/2 node failures.
        
    * **Kafka:** A distributed streaming platform called Kafka can be used with Hyperledger Fabric as a consensus mechanism. High scalability and fault tolerance are features of Kafka's design. Kafka was created for systems that process large amounts of data and has a million messages per second throughput.
        
    * **Solo:** Solo is a consensus algorithm that is used for testing and development purposes. It is not suitable for production use. Solo is a simple consensus algorithm that does not require a consensus mechanism and is therefore not suitable for use in a production environment.
        
4. **Communication Layer:** This layer consists of the protocols for exchanging messages among network users. Multiple communication protocols, such as gRPC, REST, and Kafka, are supported by Hyperledger Fabric 2.0.
    
5. **Infrastructure Layer:** This layer is made up of the membership service provider (MSP), orderer, and peer nodes. Peer nodes interact with one another to validate transactions and maintain the ledger. Transactions are distributed to peer nodes via orderer nodes, which also organize and package them into blocks. The MSP is in charge of maintaining network participants' digital identities and offering a secure communication mechanism.
    

## Features

Hyperledger Fabric 2.0 includes several new features and improvements over the previous versions, including:

* **Private data collections:** A new feature called private data collections has been added in Fabric 2.0 that enables the private storage of sensitive data on the network. Only authorized parties can see private data, which improves the network's security and privacy.
    
* **Identity mixer:** The identity mixer is a new feature that allows users to create anonymous transactions on the blockchain while still upholding trust and integrity.
    
* **Expanded access control:** The expanded access control features in Fabric 2.0 enable more precise control over who can access the network and how.
    
* **Improved consensus algorithms:** Consensus algorithms, which are in charge of ensuring that each node has a consistent view of the network, have been optimized to increase their effectiveness and scalability.
    
* **Support for parallel transaction execution:** Improvements for faster and more effective transaction processing have been made. This includes assistance with parallel transaction execution, which enables the processing of numerous transactions concurrently.
    
* **Support for multiple programming languages:** Fabric 2.0 supports multiple programming languages so that developers can build smart contracts and applications in the language of their choice.
    

## Conclusion

Hyperledger Fabric 2.0 is a potent platform for distributed ledger technology and can be used to develop enterprise-grade blockchain applications. Because of its flexible and scalable architecture, developers can create unique blockchain solutions to fit the demands of their particular companies. The platform's major features, including numerous channels, chaincode, and certificate authorities, enable secure and effective data management, while its pluggable consensus method and support for multiple communication protocols provide scalability and adaptability. With blockchain technology gaining acceptance, Hyperledger Fabric 2.0 is in a strong position to take the lead among solutions for companies wishing to utilize the advantages of this technology.

## References

* [What is Hyperledger Fabric? (](https://aws.amazon.com/blockchain/what-is-hyperledger-fabric/)[amazon.com](http://amazon.com)[)](https://aws.amazon.com/blockchain/what-is-hyperledger-fabric/)
    
* [A Blockchain Platform for the Enterprise — hyperledger-fabricdocs main documentation](https://hyperledger-fabric.readthedocs.io/en/release-2.5/)
    
* [Hyperledger Fabric in Blockchain - GeeksforGeeks](https://www.geeksforgeeks.org/hyperledger-fabric-in-blockchain/)
    
* [https://medium.com/@sumit.vedpathak](https://medium.com/@sumit.vedpathak)
    
* [https://blockchain.oodles.io/dev-blog/components-of-hyperledger-fabric-network/](https://blockchain.oodles.io/dev-blog/components-of-hyperledger-fabric-network/)