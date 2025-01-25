# Blockchain

## Introduction
In this repository, we delve into the intricacies of blockchain technology, exploring its origins and examining why it is crucial today.

## ECDSA and secp256k1
HTTPS in web3 employs ECDSA, considered more advanced than the earlier RSA algorithm.  
Bitcoin specifically uses the [secp256k1 curve](https://github.com/bitcoin-core/secp256k1), whose parameters are believed to be minimally random.  

For more on RSA and digital signatures, see:  
[https://cryptobook.nakov.com/digital-signatures/rsa-signatures](https://cryptobook.nakov.com/digital-signatures/rsa-signatures)

## Proof of Mining
Mining is the process of creating a block of transactions to be added to a Proof-of-Work (PoW) blockchain. It simply extends the chain by adding a new block.  
Peers in the mining process are called miners—a miner can be any node running specialized mining software.

### Key Points
• No double spending, block size, and all transactions must be validated  
• Miners receive rewards only when proof of work is demonstrated

### Proof of Work
This is a consensus mechanism deciding which blocks and transactions are valid, and who can add new blocks. Both Bitcoin and Ethereum rely on PoW or alternative mechanisms like Proof of Stake (PoS).  
Mining software repeatedly hashes a block of data until it finds a hash below a target difficulty.

#### PoW Algorithm Steps
1. Take the current block’s header  
2. Append a nonce (starting at 0)  
3. Hash data from steps 1 and 2  
4. Check the hash against the target  
5. If the hash is below the target, the puzzle is solved and a reward is earned; otherwise, increment the nonce and repeat

For practical exploration, you can use:  
• [Online SHA256 tool](https://emn178.github.io/online-tools/sha256.html)  
• [Blockstream info](https://blockstream.info) for the latest transactions and blocks

