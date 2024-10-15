## rollups

<br>

* rollups move computation (and state storage) off-chain, but keep some data per tx on-chain, using compression tricks to replace data with computation wherever possible (but scalability is still limited by the data bandwidth of the underlying blockchain).



<p align="center">
<img width="500" src="https://user-images.githubusercontent.com/1130416/234379326-901ed83c-4bc5-4c97-bad8-3b9d96dfb1b7.png">
</p>


- an on-chain smart contract maintains a state root (the merkle root) of the state of the rollup.
- anyone can publish a batch (collection of txs, compressed to form the previous state root and the new state root).
- the contract checks that the previous state root in the batch matches the current state root - if not, it switches the state root to the new state root.
- for depositing and withdrawing, txs can have input or output outside the rollup state (processed within the batches).
- optimistic (fraud proof) or zk (validity proof) rollups are solutions to know that the post-state roots in the batches are correct.


<br>

<p align="center">
<img width="250" src="https://user-images.githubusercontent.com/1130416/234935489-f65f98a0-a6ac-4b86-b40d-e4aac97733b7.png">
</p>


<br>

---

### ethereum optimistic l2s

<br>

##### arbitrum one
- started rollups
- largest TVL

##### optimism
- rollup from optimism collective, with a rich ecosystem of l2
- tool to create l2 part of the superchain

##### mantle
- l2 from bitdao

<br>

---

### ethereum zk-rollups l2s

<br>

##### zksync era
- the leading zk-rollup and a zkevm (zk-rollups that use ethereum virtual machine to execute transactions are called zkevms)
- the only zkevm that supports native account abstraction in the consensus layer of the chain

##### starknet
- zk-rollups from starkware
- not a zkevm
- used the cairo language
- has recently open-souced their STARK prover

##### polygon zkevm
- part of polygon 2.0, an ecosystem of zk-rollups
- converting polygon pos into a zk-validum
- has their prover open-sourced

#### linea
- another recent zkevm from consensys


<br>


<p align="center">
<img width="500" src="https://user-images.githubusercontent.com/1130416/234379163-f55493b4-7ad5-4d0d-9021-0f722cbe34a6.png">
</p>

<br>

---

### in this dir

* **[zkps](https://github.com/go-outside-labs/decentralized-protocols-research/tree/main/cryptography/zkps)**


<br>


---

### resources

<br>

* **[what are rollups, by ef](https://ethereum.org/en/developers/docs/scaling/zk-rollups/)**
* **[upgrading ethereum book, by b. edgington](https://eth2book.info/bellatrix/)**
* **[an incomplete guide to rollups, by vitalik](https://vitalik.ca/general/2021/01/05/rollup.html)**
* **[validity rollups on bitcoin, by john light](https://bitcoinrollups.org/)**
* **[covenants, by bitcoin optech](https://bitcoinops.org/en/topics/covenants/)**
* **[a rollup-centric ethereum roadmap](https://ethereum-magicians.org/t/a-rollup-centric-ethereum-roadmap/4698)**
