# Concept Unit

## Deployment

In this module, you will be deploying **GoQuorum QuickStart** on azure which is an essential step for obtaining the **RPC endpoint**. The major steps involved in the deployment are as follows: 

- Creating the Quorum Dev QuickStart on azure by filling in some basic details
- Access the virtual machine with the SSH method using **Putty**
- Activate the RPC endpoint by setting up the blockchain


## Define RPC Endpoint

In this module, you will be learning on deploying the GoQuorum Blockchain as the first steps towards building Decentralized applications (dApps). All the decentralized application, need a way to communicate with blockchain. Without this communication, dApps cannot access or transfer any information or even make transactions on the blockchain on which they operate. 

The connection between dApps and blockchain is facilitated by RPC Endpoints. They are the nodes that are essential elements of decentralized application development. They are more specifically called as Ethereum RPC Nodes. RPC is an abbreviation for a remote procedure call, and they are a form of inter-process communication. In blockchain terms, a server is often referred to as a node. These nodes are also referred to as RPC nodes, and they allow us to read blockchain data and send transactions to different networks. This means that an RPC node is vital to enable our application to function correctly.


## Define GoQuorum Quickstart

GoQuorum is a service provided by ConsenSys on which is also available on Microsoft Azure. It is an open-source protocol layer that provides developers with the flexibility and reliability needed to make their blockchain applications successful. It consists of configurable components and API’s, enabling us to customize our use case production environment. 

The Quorum Developer Quickstart is a command line tool that allows users to set up a development GoQuorum network on their local machine in less than two minutes. The quickstart is written in Javascript and designed to be run as a global npm module from the command line.

Quorum Dev Quickstart has many small services on a single Azure VM, like, private network comprising of 4 validators, RPC node, private transaction nodes, monitoring, and more. 
