title={Architecture of the Hyperledger Blockchain Fabric}
author={Christian Cachin}
year={2016}
keywords={permissioned, blockchain, consenus, byzantine-fault tolerant, smart contracts}

abstract={A blockchain is best understood in the model of state-machine replication [8], where a
service maintains some state and clients invoke operations that transform the state and generate outputs.
A blockchain emulates a “trusted” computing service through a distributed protocol, run by nodes connected
over the Internet. The service represents or creates an asset, in which all nodes have some stake.
The nodes share the common goal of running the service but do not necessarily trust each other for
more. In a “permissionless” blockchain such as the one underlying the Bitcoin cryptocurrency, anyone
can operate a node and participate through spending CPU cycles and demonstrating a “proof-of-work.”
On the other hand, blockchains in the “permissioned” model control who participates in validation and
in the protocol; these nodes typically have established identities and form a consortium. A reportcompares the two models [9].}


* Permissioned blockchain with two kinds of peers: Validating and non-validating peers. A non-validating peer acts as a proxy for transaction-issuing clients and may verify but not execute transactions.

* Arbitrary smart contracts as Go programs in Docker container (chaincode)
* Pluggable consensus protocol
* Security support through certificate authorities for TLS certificates, enrollment certificates, and transaction certificates
* Event Framework
* Node.js client SDK

Architecture:

Validating peers run a BFT consenus protocol for a replicated state machine that accepts three tyoes of transactions as operations:
* Deploy transactions (deploys chaincode contracts)
* Invoke transactions (invokes chaincode contracts)
* Query transaction

For connecting to the network a peer needs an encrollment certificate from an enrollment CA that is part of the membership services. Once connected a peer may acquire transaction certificates, which are needed to submit transactions. Transaction cerficates are issued by a transaction CA and support pseudonymous authorization for the peers submitting transactions, in the sense that multiple transaction certificates issued to the sameeer cannot be linked with each other. Chaincodes and states are encrypted using a blockchain specific symmetric key. 

https://www.zurich.ibm.com/dccl/papers/cachin_dccl.pdf
