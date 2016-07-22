title={b-money},
author={Wei Dai},
year={1998}

> In a crypto-anarchy the government is not temporarily destroyed but permanently forbidden and permanently unnecessary. It's a community where the threat of violence is impossible, and violence is impossible becasue its participantts cannot be linked to their true names or physical locations.

> A community is defined by the coorperation of its participants, and efficient cooperation requires a medium of exchange (money) and a way to enforce contracts.

## Description of b-money protocol

B-money protocol entails creation and transfer of money and enforcing of contracts.
Based on pseudonyms and signatures (public key cryptography)

Peer-to-peer protocol:
* Everyone has a ledger with all balances
* Everyone can create money by solving a easily verifyable computational puzzle
* Monetary units created correspond to lowest cost of production
  > For example if a problme tales 100 hours to solve on the computater that solves it most economically, and it takes 3 standard baskets to purchase 100 hours of computing time on that computer on the open market, the upon the broadcast of the solution to that problem everyone credits the broadcaster's accout by 3 units. 
* Transfer of money by broadcasting signed messages
* Contracts include a maximum reparation in case of default and should include an arbitrator
* Enforcement of contracts: Each party broadcasts a suggested reparation/fine schedule and any arguments or evidence in his favor. Each participant modifies accounts according to his conclusions.

Federated protocol:
* Servers hold accounts
* Messages are sent to a random subset of servers
* Recepeient/Counterparty should confirm that message was received
* Servers are required to deposit a certain amount of money in a special account to be used as potential fines or rewards for proof of misconduct.
* Servers need to periodically publish and commit to their state

## Discussion

B-money is surprisingly close to Bitcoin. Pseudonmous identities and transaction authentication using public key cryptography is used. Every participant (or a federation in the second protocol) keeps a subjective copy of the ledger. Money creation by solving easily verifyable computational puzzles. The notion of contracts with deposits and arbitration. All these was implemented in Bitcoin. However, B-money leaves  open how divergences in the ledgers are settled. In particular contract enforcement in case of dispute can lead to divergence.
The monetary policy differs also from Bitcoin. Furthermore B-Money follows a account-based model in contrast to Bitcoin's UTXO model.   
