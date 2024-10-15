## 🧱⛓ intros to blockchain 

<br>


### tl; dr

* **blockchains have the following core functions** (although modular blockchains specialize in one or two):
  * execution: transaction execution and state update.
  * settlement: finality and dispute resolution.
  * consensus: agreement on transaction ordering.
  * data availability: prove data was published to the network.
    
* **in a blockchain, each block consists of two pieces**:
  * a block header: metadata for the block, which consists of some basic information about the block, including the Merkle root of txs.
  * the transaction data: making up the majority of the block, and consisting of actual transactions.

* **in general, a blockchain has two types of nodes**:
  * full nodes (fully validating nodes): they download and check that every tx in the blockchain is valid, and require lots of resources.
  * light clients: they don't download or validate any tx, but instead thye only download the block header and assume that the block only contains valid txs (less secure). light clients can rely on full nodes sending them a fraud proof if a block contains a invalid tx.

* **the data availability problem:**
   - in order to a full node to generate a fraud proof for a block, they need to know the tx data for that block. if a block producer just publishes the block header, but not the tx data, then full nodes won't be able to check if the txs are valid and generate fraud proofs.
   - it's a requirement that block producers must publish all the data for the blocks, but this needs to be enforced.
   - to solve this problem, there need to be a way for light clients to check that the tx data for a block was actually published to the network so full nodes can check it.   
   



<br>

---

### in this dir

<br>

* **[ethereum blockchain](ethereum.md)**
* **[solana blockchain](solana.md)**


<br>

----

### resources

<br>

* **[ef's ethereum protocol wiki](https://epf.wiki/#/)**
* **[celestia's namespaced merkle tree](https://github.com/celestiaorg/nmt)**
* **[jellyfish merkle tree, by z. gao et al](https://developers.diem.com/papers/jellyfish-merkle-tree/2021-01-14.pdf?ref=127.0.0.1)**
* **[leaves of hash, by trail of bits](https://blog.trailofbits.com/2019/06/17/leaves-of-hash/)**
* **[how merkle trees work, by consensys](https://media.consensys.net/ever-wonder-how-merkle-trees-work-c2f8b7100ed3)**
* **[neo-cypherpunk toolkit, by go outside labs](https://github.com/go-outside-labs/neo-cypherpunk-toolkit)**
* **[bitcoin memory pool](https://www.blockchain.com/explorer/mempool/btc)**
* **[a survey of execution client diversity, from ethstaker](https://paragraph.xyz/@ethstaker/execution-client-diversity)**
* **[on a rusty sparse merkle tree experiment, by mia stein](https://mirror.xyz/go-outside.eth/zX1BaGZLHAcQOKdhFnSSM0VW67_-OFCi5ZegGFPryvg)**
* **[on uploading your soul to the interplanetary sys, by mia stein](https://mirror.xyz/go-outside.eth/A3iJGhXTJI5fgQoZVgIu3ovPV1P8zrxigpwngm0n4I0)**
* **[ethereum transaction visualizer](https://github.com/naddison36/tx2uml)**
