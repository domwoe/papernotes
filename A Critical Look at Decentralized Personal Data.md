## A Critical Look at Decentralized Personal Data Architectures

Arvind Narayanan
Solon Barocas
Vincent Toubiana
Helen Nissenbaum
Dan Boneh

Internet was conceived as a decentrlized network but the most successful web applications tend towards centralization.

There has been counter movements towards re-decentralization but these haven't been very successful so far. 
These include:
* Personal data stores
* Vendor relationship management systems
* Federated and distributed social networks

### Historical Overview 

* Late 90s: 'Negotiated privacy techniques'. Commercial infomediaries that take custody of consumers' data and help draft contracts for exchange and usage
* Died in early 2000
* Resurrection in late 2000
* Mydex's white paper recapitulates much that was descirbed by Lumeria a decade ago

### Representative Survey

Infomediaries are trusted parties that should represent the users in exchange with marketers. Therefore infomediaries are a kind of brokers. It has been argued that telecommunications providers, banks and other parties such as providers of home entertainment set-top boxes are ideally suited to be infomediaries.

Non-independent (technical) classification dimensions:
* Locus of data hosting: remote, TTP, distributed, local
* Open standards vs. proprietary (This greatly affects interoperability)
* Open vs. closed-source implementations
* Data portability: data export, APIs (for third parties), or none

Classification in terms of social values:
* Privacy
* Utility (overall social (societal?) benefit)
* Cost
* Innovation

'We suggest that much of the reason for what we see as overenthusiastic claims about decentralized system is that design characteristics have been confused with values'

### Drawbacks of Decentralization

* An architecture without a single point of data aggregation, management and control has several technical disadvantages.
Functionality: There are several types of computations that are hard or impossible without a unified view of the data. Suffer more from network unreliability, resulting in a tradeoff between consistency and availability. 

* Decentralized systems need standardization and interoperability. While these characteristics may lead to longterm innovation it slows down the process in the short term. Shapiro notes two benefits of standardization: greater realization of network effects and protection of buyers from stranding, and one cost: constraints on variety and innovation, and argues that the impact on competition can be either a benefit or a cost.


* Centralized systems have economics of scale (hosting, development, maintenance, branding, advertisement)

* Cognitive factors: Installation of software, more control = more decisions -> cognitive overload

### On Control over Personal Data

Absolute control is impossible. Suggest that control over information is probably not the right conceptualization of privacy, if privacy is the end goal.

### Open standards and Interoperability

Open standards necessary but not sufficient for interoperability, because there are too many open 'standards'.

The more functionality that has to be standardized the harder.

### Recommendations

* Economic feasibility: Are there entities with the economic incentives to play the various roles that are called for?
* Are you shooting at the right target? Do people have the values you think they do?
* Incorporate other notions of regulability. No extreme.
* Offer advantages other than privacy to users.
* Design with standardization in mind.
* Target limited feature sets.
* Work with regulators. As numerous law/economics scholars have pointed out, market solutions appear to underprovide privacy and regulation can tweak the environment to address this imbalance .

