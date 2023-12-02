# Blockchain

facilitates peer to peer transfer of data
here data is digital assets, so currency (digital)
in a decentralized network

immutable time-stamped series of records of transactions that is managed by a cluster of nodes or computers, but not owned by a single entity.

Blockchain helps in enabling the provision of financial services at a very low cost

A digital database or ledger is dist among the nodes of different peer-to-peer networks.

Every new block adds 6.25 BTCs in the system.
And we also have an upper limit (so controlled supply)

50 -> 25 -> 12.5 -> 6.25  (halved every 4 years)

Difficulty can be increased or decreased depending on how much are getting mined per 10m

Supply Cap at 21M

Types of Ciphers:
Block, Stream, Symmetric Key Encryption, Public Key
AES, RSA, Elliptical Curves
Key management and assoc.

Hash Function
Random sized inp -> Fixed size outp
Output Hash Digest (Hex number), Hash Code etc
$$
H : \{0,1\} : \{0, 1\}^n, h = H(M)
$$
output h is usually smaller than M (message).

Features:
Deterministic, Quick,
Avalanche Effect : Minor change in input results in massive change in output.
One-Way (no reversing) | Mathematically Infeasible.
Collision Resistance | Infeasible to find two messages with same hash values.
Non predictable, 256bit Hash function makes it difficult to search for collisions.

Blockchain Usage in Food Manfc.
Ocean to Plate;
Details of Tuna dish, mostly about it's transportation status and other details
Tuna Dish -> Restaurant freezer, Supplier -> Distb -> Processing -> Merchant -> port Auction -> Fishing date.
Hygiene proof

Example in Medicine and Drugs
Journey of drug from raw materials and info
It helps remove the risk of using expired drug, and unnecessary stock piling for black market.

Crypto Kitties is an example of game/fun cryptocurrencies.

Tempering with Blockchain?
Many users keep the updated copy due to the ledger being distributed among the nodes of different peer-to-peer networks in a decentralized network.
If anyone changes or alters any block, they will also have to alter every subsequent block added after that.
They would lose in the end, and other's copies will be different from them.

Apolitical and Amoral
It doesn't care who gets the fund
Circular Economy : How can such small number of coins sustain such a large economy.

But it offers/supports social inclusion
Cross border payments
Helps in fundraising like for Ukraine and Palestine
Financial inclusion for areas where formal banking is broken

# Encryption and Decryption

Symmetric Key Encryption
![image-20231128215808793](C:\Users\Prashant(Gaz)\AppData\Roaming\Typora\typora-user-images\image-20231128215808793.png)

Sender and User share the same (symmetric) key.
Cipher(P, K) ----> CT ----> Decipher(CT, K) ----> P

Block Cipher
Encrypts n-bit plaintext blocks to n-bit ciphertext blocks.
Things to configure; Block size, Key size, Number of rounds
(Data and Storage complexity)

AES is also a symmetric key algorithm

Problems with Key management in SKC
Number of keys to keep
Key Generation, Size and also exchange
Key exchange should be done such that Key remains secret

Public Key Cryptography
Two related keys;
$$
K_{pub} \ and \ K_{pri}
$$
are used for encry/decry or signing/verifying
Public key certificate / digital document is issued, that binds user to it's public key. And giving them control and access of the corresponding private key.

Features:
Infeasible to find a private key only with the knowledge of public key and algorithm.
PKI
Trust Management
Example : RSA

![image-20231128220802382](C:\Users\Prashant(Gaz)\AppData\Roaming\Typora\typora-user-images\image-20231128220802382.png)

RSA Algorithm
Choose too huge prime numbers P and Q
Calculate N = P * Q
Select public key (E) such that it is not a factor of (P-1) and (Q-1)
Select the private key (D) such that the following equation is true:
$$
(D*E) mod (P-1) * (Q-1) = 1
$$
For encryption:
$$
C = P^Emod(N)
$$
For decryption:
$$
P = C^Dmod(N)
$$
Elliptic Curve Cryptography
Based on the intractability (impossible/diff nature) of some math problems.
Based on algebraic structure of elliptical curves over finite fields

Finite Fields
Field of integers modulo p, where p is a prime
GF(p) - Galois Field of p or 
$$
F_p
$$
Finite field has m * p elements, if m = 1, then the field can be considered a prime field, if m > 1, then we have extension fields.

![image-20231128221953169](C:\Users\Prashant(Gaz)\AppData\Roaming\Typora\typora-user-images\image-20231128221953169.png)

# Consensus Mechanisms

Proof of Work
Miners solve hash puzzles for Proof of Work
Eth2 uses Proof of Stake
similar to proof of authority in Bank consortiums

# Supply Chain Management

There is no transparency in old supply chain methods
No way to check and verify every moment of supply process
It is easy for malicious actors to modify the supply chain for their benifits
Both companies and users suffer cause of this

If each prod is digitized, can carry a serial number for unique id, st <Pic, Id>
Then each asset can be monitored and tracked
<Live video, Id>  ---> Track assets in real time

### Ocean to Plate

Relevant details of the journey of a Tuna fish (example) since it's fished to the point where it's a dish.
Authentication over Blockchain
Hygiene proof

Another Examples
Project Food Trust - IBM and Walmart
Pharmaceutical Drug journey to patient from raw material
Consumption records for a particular patient, to monitor what are they taking

Advantages and Benefits
Transaction time and other info is recorded
Overhead
Data loss, tampering, Fraud and Cyber crime risks are reduced
IOT integration in supply chain is possible

### TE-Food (Farm to table)

Platform that offers solns to farm-to-table food traceability using blockchain
It helps the consumers, govt, food firms, as it make the supply chain more transparent.
Network also seeks to support
Food firms get a better understanding of their food suppliers
Consumers get clarity of their food, allowing them to make informed decisions
Governments get a real time picture of the food market, for safety monitoring etc
Farms can share data about their product, like its origins, food safety, transport volumes and other logistics.
Processors can share info regarding processing and packaging, which would be helpful to the retailers.

Addition features;

transparent food information, and recognize brands with traceability.

* Establish direct communication with consumers - Engage directly with
  consumers, and collect valuable data about them.
* Become compliant to import regulations of target countries - Unlock export
  possibilities to countries which require traceability information.
* Improve operational efficiency - Analyze and optimize your supply chain
  processes.
* Position your premium products - Provide proofs of your quality
  sustainability claims.
* Quicker (and targeted) product recalls - Automate your product recalls, and narrow down the scope to the affected batches.

### IBM Food Trust

Modular solution for digital supply chain built on the blockchain
Network of growers, processors, wholesalers, distributors, manufacturers, retailers.
Connects participants to an immutable shared record of transaction data, processing details and more
It is permissioned.

### Blockchain for Record verification

Property, Land records verification.
Covid vaccination certi.

### Blockchain explorers

View and explore transactions, info such as transaction history, balance of each address and the blocks that have been mined
Investigating transactions
etherscan, polygonscan

Tainted Coins
Blockchain addresses that have been blocked by the OFAC of US Treasure dept, they are blocked from being used to send or receive Bitcoin.
Every country may have their own blacklists
Ex; Silk Road darkent, WannaCry ransomware
Addresses maybe associated with terrorists and drug traffickers.
You can get sanctions, and lose Bitcoin if you trade with these addresses.

Bitcoin White lists
Addresses that are allowed to interact/trade
They are created to prevent unauthorized access to service.
help to prevent illeagal activites, fraud and theft
improve security
They are based on factors such as user identity, trade history and risk profile
No publicly known whitelists for Bitcoin.

Good Bitcoin
Since Bitcoins can be explored and examined by anyone, it is important for financial institutions to reserve Good Bitcoins

Blockchain Use Cases
Tokenization, Tokenomics (Private sell tokens)
Fungible (How much you have) and Non-Fungible Tokens (Which one you have)

# Ethereum

Ethereum is a distributed public blockchain network
A platform for sharing information across the globe
ETH is the decentralized currency, also known as Ether
Ethereum network pays transaction fees for computational services

### Hash rate

Measure of computational power that is used to solve the crypto hash function/puzzle.
Measured in Hashes per second (H/s)
More miners -> More hash rate
Because miners add their own computing power to the network
Quick hash rate -> Transactions are processed more quickly -> Also makes it difficult for an attacker to mount a successful attack on the network
High hash rate -> less profitability of mining, as many miners are competing.

### For control of the network

An attacker must control 51% or more of the total computational power of the network in a (PoW Network) and must control 51% or more currency in a (PoS Network) 

### Mining Pool

Group of miners put together their computational power to increase their changes of solving a block and earning the reward.
It increases your chances of solving the puzzle/block but decreases your reward too.
Can reduce electricity costs
Easier to manage mining operation as group handles the technical aspects (and provides tools) for you
Susceptible to scam or fraud so reputation of the pool is important to consider

# Solana

Blockchain platform designed to be scalable, secure and energy-efficient
PoH, proof of history consensus mechanism, processes transactions much faster
50K transactions / sec can be processed
Censorship resistant (No one can control)

**Applications**

**DeFi** : Decentralized Finance, lending platforms and derivative markets
**NFTs** : Trade or Create NFTs
**Gaming** : Decentralized Gaming
**Web3** : Dec. Web applications

### Why different blockchains

Different blockchains offer a wide range of possibilities and features, to improve efficiency, security, transparency

Cryptocurrencies need to be highly decentralized, secure
Supply chain management need to be more scalable and private
Some have truly decentralized, some don't
Different blockchains are suited for different stages of development, for different cultures and jurisdictions

### Public Blockchains

Open to anyone
Most decentralized
Often used for cryptocurrencies

Ex; Bitcoin, Litecoin (fast and cheap alt), Ethereum

### Private Blockchains

Permissioned
Only authorized people can join
Often used by businesses and organizations, improve security, privacy, efficiency.
Faster, more governable and interoperable with the current or existing financial system

Ex; Hyperledger Fabric, R3 Corda

### Consortium Blockchains

Hybrid of public and private
controlled by a consortium of organizations rather than a single entity
More decentralized than Private, but less than Public

Ex; TE-Food, IBM Food Trust, Stellar

# Privacy Coins

Cryptocurrencies that use encryption tech to hide the sender, receiver and the amount of transactions
Used for private and anonymous transactions
Diff for third parties to track

 **Usage**

Protect financial privacy
Avoid censorship
Make anonymous donations
Conduct Illegal activities

### Monero

Monero (XMR), focused on privacy
can't be tracked or traced
PoW consensus
Uses Ring Signatures, Stealth Addresses and Ring Confidential Transactions

Ring Signatures : Ring signature is **a type of digital signature that can be performed by any member of a set of users that each have keys**. Therefore, a message signed with a ring signature is endorsed by someone in a particular set of people.

### Zcash

Fair and Open | Avail to all
Secret messages
Faster than Bitcoin
Self-funded dev
Fast, low fees for transactions

**Z and T Addresses**

T-addresses are publicly viewable
Z-addresses are shielded, do not reveal address, amount or any other info (sensitive)
Both are interoperable
Zero-knowledge proofs
Prover says to the verifier they possess specific knowledge, protocol uses a secret key to confirm the possession of information. Miners check the shielded transaction by verifying the key.

### Dash

Open source
Fast, cheap, global
Uses **PrivateSend** to hide details of transactions

### R3 Corda

Open Source
Permissioned
R3 is global finance tech company
Founded by a group of banks, tech companies and financial institutions

**Used in** :

Trade Finance
Supply chain management
Used in Regulation, for KYC and Anti Money Laundering (AML)

# Meme Coins

Meme is an idea, spreads from person to person
Dogecoin is the first meme coin (Shiba Inu Meme)

**Things to know**

Highly volatile
Can lose their value quickly
May not have real world uses
Pump-and-dump schemes
Unregulated, No guarantee that you will be able to cash out

## Dogecoin

Lighthearted alternative to traditional cryptocurrencies
Launched as a joke by Billy Marcus, Jackson Palmer (Reddit Friends)
Created to be abundant
130 million circulating
10K produced every minute
Musk supports it and other AltCoins

# Bitcoin vs Ethereum

**Bitcoin**

Wallet/Exchange apps
Bitcoin Blockchain Protocol
P2P and OS
Hardware

**Ethereum Stack**

Verticals : End user apps
Application Framework ; Smart contracts
Ethereum Blockchain and EVM
P2P and OS
Hardware

# Ethereum Block

![image-20231129012049995](C:\Users\Prashant(Gaz)\AppData\Roaming\Typora\typora-user-images\image-20231129012049995.png)

# Smart Contracts

Self executing contracts
stored on the blockchain
automate a lot of tasks
(transfer of funds, voting)

EVM is a Turing complete (system that can simulate Turing machines) computer that runs on every Ethereum node
Responsible for executing smart contracts
It breaks them down into opcodes
Smart contracts are written in solidity
It's a statically typed langauge

Code example
```solidity
// SPDX-License-Identifier: GPL-3.0 
pragma solidity >= 0.4.16 < 0.9.0;
contract Test
{ 
	
	// Declaring state variables 
	uint public var1;
	uint public var2;
	uint public sum;

	// Defining public function 
	// that sets the value of 
	// the state variable 
	function set(uint x, uint y) public
	{ 
		var1 = x;
		var2 = y;
		sum=var1+var2;
	} 
	
	// Defining function to 
	// print the sum of 
	// state variables 
	function get( 
	) public view returns (uint) { 
		return sum; 
	} 
}

```

### Execution

When the Target address in transaction is a smart contract, then the execution code is activated and ran on the EVM
Input is the payload field of transaction
Current state -> Var defined in the code
State of the SC is updated by this execution
EVM first executes its Bytecode when SC is called
EVM can access and change the state of the blockchain
Result in receipts

# Basic Attention Token (BAT)

Was developed to improve the broken ad market
built on top of Ethereum (open source)
Advertisers will give publishers BATs based on the measured attention of users
Users also get BATs for participating
Transparent, data privacy
Advertisers get better reporting and performance

**Ad Situation**

The ad-tech ecosystem that has evolved over the last two decades is a bewildering variety of middlemen and complexity.
No efficient marketplace for attention
Users lost their privacy, facing malware and slow speeds, annoying pop-ups
Poor reporting and targeting for advertisers
User attention is mis-priced
Electronic pollution
Clickbait and time wasting of users
Forces users to use Ad Blockers, Publisher loses.

**Bat offers solution because** :

It properly prices of user attention
users will not feel violated
BAT connects advertisers, publishers and users, creating an effective marketplace
digital and transparent
Attention be measured as viewed for content and ads only in the browser’s active tab in real time.
Brave makes it possible

![image-20231129015825028](C:\Users\Prashant(Gaz)\AppData\Roaming\Typora\typora-user-images\image-20231129015825028.png)

Brave defends your data
cuts out third party trackers and stops data leakage
provides publishers good revenue
aims to resent online ad-based web ecosystem

### Blockchain in Real Estate

Smart contracts can transform real estate practices
Brokers, real estate agents, hard money lenders and anyone dealing in property can profit
Mortgage lenders can sign agreements using smart contracts
No need for broker, lawyers or other middle men
execution is managed auto by network so no bias or manipulation by third party

### Handling exceptions in Blockchain

Need for an auto deterministic way
well defined process is needed to improve the trust
one policy is to allow the first transaction and reject all the other that reference the same asset

# Forks

Mechanisms that add to the robustness of the blockchain framework
**Bitcoin Forks** : Changes to the network to create a new blockchain on top of original chain

### Soft and Hard Forks

Hard implies major change in protocol, a new version maybe on top of the prev
Soft is essentially minor process or  adjustment by bootstrapping a new software, more like a software patch

Soft fork's updated version is backward compatible
When Bitcoin network and the nodes adapt new set of rules such as change in block size or new transaction type being introduced

In hard forks, change of protocol is not backward compatible, so users will need to update the software to see changes. It is a permanent divergence from original

**Bitcoin & Ethereum Forks**

Bitcoin Cash, Gold, SV
Ethereum Classic : First known Eth fork, after 2016 Dao Attack, that resulted in theft of millions.
Byzantium and Constantinople: soft forks in '17, '19 several improvements, faster block confirmation, lower transaction fees

**Ethereum 2.0**

Major upgrade
Aimed to improve network scalability, security
transitioned from Proof of Work to Proof of Stake
implemented through a series of serious of hard forks

# Blockchain, IoT and AI/ML

IoT is a collection of sensors, software and tech to gather data and dist. online
IIot (Industrial IoT) transforming industrial processes
Issues : Single point failure, unauthorized access, hacking, mis-config of sensors, data security and integrity.

IoT + Blockchain -> More security, enhancing privacy, streamlined operations

# Smart Contracts (Deep)

**Foundation**

SC are computer program that consists of self-executable code, 
They ensure proper access control 
if SC conditions are met -> it triggers a contract statement -> results kept on the blockchain
Advantages

**Advantages**

Decentralization
Improved privacy, scaling
Verifiable self-exec chain codes
Changed written on the blockchain automatically after trigger and execution

**Characters**

Distributed, Deterministic, Immutable
Autonomy, Transparent
Trustless, Self Enforcing and Self Verifying

**Examples**

Solidity (EVM), Lisk (JS), Hyperledger Fabric
Mostly, Domain Specific Langs are used instead of GPLs.

**DAO**

Was hacked, 50 million stolen
Introduced a Hard Fork on Ethereum

**Oracles**

Smart contracts cannot access external data which is required to control the execution of business logic.
Oracle is an interface that delivers data from external source to smart contracts.

Oracles can deliver different types of data ranging from weather reports, real-world news, and corporate actions to data coming from Internet of Things (IoT)
devices.

Smart contracts can subscribe to Oracles and pull the data (or get pushed)

Oracles should not be able to manipulate the data they provide
they must provide authentic data
But how to trust third party on this?
If data is provided by a large reputable third party, then it raises the issue of centralization (standard oracles)

Decentralized oracles built on distributed mech can solve this problem

Hardware oracles get real world data from physical devices
These can be tempered with so the devices must be temper proof

**Smart Oracles**

Proposed in Codius
Entities like Oracles, but with added capability of contract code execution
May or may not be deployed on the blockchain
Usually part of big apps like DAOs.

# AI

Artificial intelligence (AI) is the ability of a machine to perform tasks
that typically require human intelligence. This includes tasks such as learning, reasoning, problem-solving, and interacting with the environment.
