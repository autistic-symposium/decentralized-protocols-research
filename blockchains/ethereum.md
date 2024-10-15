## ethereum blockchain

<br>

#### evm execution

* in native execution, evm will load the bytecode and execute the opcodes in the bytecodes one by one from the beginning.
* each opcode can be thought as doing the following steps:
  1. read elements from stack, memory, or storage.
  2. perform some computation on these elements.
  3. write back results to stack, memory, or storage.


<br>


#### light clients


* light clients receive the block headers, which contain a merkle root (more on this later) that can be used to query full nodes to verify if a transaction is included in a particular block.


<br>

#### ethereum roadmap

<br>

<img width="600"  src="https://user-images.githubusercontent.com/1130416/234419153-76ab9f89-00e8-48e7-93c4-c8d880ec2007.png">


<br>

----

### external resources

<br>

* [geth code for stateDB](https://github.com/ethereum/go-ethereum/blob/d4d288e3f1cebb183fce9137829a76ddf7c6d12a/core/state/statedb.go#L64)
* [understanding trie databases, by d. brickwood](https://medium.com/shyft-network/understanding-trie-databases-in-ethereum-9f03d2c3325d)
