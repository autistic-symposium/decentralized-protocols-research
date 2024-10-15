## tendermint

<br>

* consensus protocol for ordering events in a distributed network under adversarial conditions (aka byzantine fault tolerant consenus, or atomic broadcast).
* tendermint consists of two technical components: a blockchain consensus engine and a generic application interface, and works even if up to 1/3 of machines fail in arbitrary ways.
* tendermint core (the consensus engine) performs BFT state machine replication (SMR) for arbitrary deterministic, finite state machines.
* the application interface (abci) enables the transactions to be processed in any programming language.

<br>
<br>

<p align="center">
<img src="https://github.com/go-outside-labs/decentralized-protocols-research/assets/138340846/fbb43593-d1d0-4efe-ae7e-80d880333a60" width="60%" align="center" style="padding:1px;border:1px solid black;" title="Jan 7th"/>
</p>


<br>
<br>

---

### references


* **[tendermint docs](https://docs.tendermint.com/)**
* **[tenderming abci](https://github.com/tendermint/tendermint/tree/v0.34.x/abci)**
* **[the latest gossip on BFT consensus, e. buchman et al.](https://arxiv.org/abs/1807.04938)**
