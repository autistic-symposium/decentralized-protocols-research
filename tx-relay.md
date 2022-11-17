## transaction relays

<br>

1. validator client requests a block without transactions fron consensus node (blinded block)
2. consensus node queries multiple MEV relays for best bid
3. consensus node selects best bid and incorporates it into the bindled block
4. validator client request the consensus node to include txs to the block and broadcast the signed block
5. consensus node requests the winning relay to include the txs to the signed block
6. consesus node broadcasts signed unblinded block to the network
