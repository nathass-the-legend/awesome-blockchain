# blockchain-tech-slack

> Curated list of resources for the development and applications of block chain.

The blockchain is an incorruptible digital ledger of economic transactions that can be programmed to record not just financial transactions but virtually everything of value (by [Don Tapscott](https://www.linkedin.com/pulse/whats-next-generation-internet-surprise-its-all-don-tapscott)).

<font color=#0099ff size=3>**This isn't merely a compilation of online materials; it's a carefully curated and verified selection of data, designed to genuinely enhance your learning journey and prove beneficial for your growth and practical application.**</font>

## Contents
<details><summary>Click to expand</summary>

- [blockchain-tech-slack](#blockchain-tech-slack)
  - [Contents](#contents)
  - [Frequently Asked Questions (F.A.Q.s) & Answers](#frequently-asked-questions-faqs--answers)
  - [Basic Introduction](#basic-introduction)
  - [Development Tutorial](#development-tutorial)
  - [Releated Tools](#releated-tools)
    - [Solidity](#solidity)
    - [truffle](#truffle)
    - [web3.js](#web3js)
  - [Further Extension](#further-extension)
    - [Papers](#papers)
    - [Books](#books)
  - [Contribute](#contribute)

</details>

## Frequently Asked Questions (F.A.Q.s) & Answers

**Q: What's a Blockchain?**

A: A blockchain is a distributed database with a list (that is, chain) of records (that is, blocks) linked and secured by
digital fingerprints (that is, crypto hashes).
Example from [`genesis_block.json`](https://github.com/yjjnls/awesome-blockchain/tree/master/src/js/genesis_block.json):

```js
{
    "version": 0,
    "height": 1,
    "previous_hash": null,
    "timestamp": 1550049140488,
    "merkle_hash": null,
    "generator_publickey": "18941c80a77f2150107cdde99486ba672b5279ddd469eeefed308540fbd46983",
    "hash": "d611edb9fd86ee234cdc08d9bf382330d6ccc721cd5e59cf2a01b0a2a8decfff",
    "block_signature": "603b61b14348fb7eb087fe3267e28abacadf3932f0e33958fb016ab60f825e3124bfe6c7198d38f8c91b0a3b1f928919190680e44fbe7289a4202039ffbb2109",
    "consensus_data": {},
    "transactions": []
}
```

![](Basic/img/blockchain-jesus.png)

**Q: What's a Hash? What's a (One-Way) Crypto(graphic) Hash Digest Checksum**?

A: A hash e.g. `d611edb9fd86ee234cdc08d9bf382330d6ccc721cd5e59cf2a01b0a2a8decfff`
is a small digest checksum calculated
with a one-way crypto(graphic) hash digest checksum function
e.g. SHA256 (Secure Hash Algorithm 256 Bits)
from the data. Example from [`crypto.js`](https://github.com/yjjnls/awesome-blockchain/blob/master/src/js/crypto.js):

```js
function calc_hash(data) {
    return crypto.createHash('sha256').update(data).digest('hex');
}
```

A blockchain uses

-   the block header (e.g. `Version`, `TimeStamp`, `Previous Hash...` )and
-   the block data (e.g. `Transaction Data...`)

to calculate the new hash digest checksum.

**Q: What's a Merkle Tree?**

A: A Merkle tree is a hash tree named after Ralph Merkle who patented the concept in 1979
(the patent expired in 2002). A hash tree is a generalization of hash lists or hash chains where every leaf node (in the tree) is labelled with a data block and every non-leaf node (in the tree)
is labelled with the crypto(graphic) hash of the labels of its child nodes. For more see the [Merkle tree](https://en.wikipedia.org/wiki/Merkle_tree) Wikipedia Article.

Note: By adding crypto(graphic) hash functions you can "merkelize" any data structure.

**Q: What's a Merkelized DAG (Directed Acyclic Graph)?**

A: It's a blockchain secured by crypto(graphic) hashes that uses a directed acyclic graph data structure (instead of linear "classic" linked list).

Note: Git uses merkelized dag (directed acyclic graph)s for its blockchains.


**More Q&A**
- [Blockchain Interview Questions](https://mindmajix.com/blockchain-interview-questions)
- [10 Essential Blockchain Interview Questions](https://www.toptal.com/blockchain/interview-questions)
- [Top 36 Blockchain Job Interview Questions & Answers](https://blockchainsfactory.com/blockchain-interview-questions/)

---
## Basic Introduction

<!--    
### Encryption knowledge
   -->

-   **Encryption knowledge**  
    * [Basic concepts]() - Asymmetric encryption, Digital signature, Certificate  

### Consensus


<!--
### Exchange
    -->
-   **Exchange**  
<!--
### Applications
    -->
-   **Applications**  
    * [Do You Need a Blockchain?](https://spectrum.ieee.org/computing/networks/do-you-need-a-blockchain)  

<!--     
### Governance
    -->
-   **Governance**
    * [Blockchains should not be democracies](https://haseebq.com/blockchains-should-not-be-democracies/)                                       
<!-- * [](https://github.com/yfeng125/blockchain-tutorial/blob/master/doc/%E2%80%8B25.%E6%AF%94%E7%89%B9%E5%B8%81%EF%BC%9A%E6%89%A9%E5%AE%B9%E4%B9%8B%E4%BA%89%E3%80%81IFO%E4%B8%8E%E9%93%BE%E4%B8%8A%E6%B2%BB%E7%90%86.md)   -->


<!--     
### Digital currency ranking
    -->
-   **[Digital currency ranking](https://coinmarketcap.com/)**   

---
## Development Tutorial

### Beginner
#### [BlockChain Starter For Beginners]((https://prasannabrabourame.medium.com/blockchain-kickstarter-from-scratch-9a3906596cd0)) 
---
### Intermediate
---
### Advanced
---
## Related Tools

### [Remix IDE](https://remix-project.org/) - development of smart contracts

## Programming

### [Solidity](https://solidity.readthedocs.io/en/develop/index.html) 



### web3.js
-   [doc](https://web3js.readthedocs.io/en/1.0/) 

---
## Further Extension
### [Papers](https://github.com/decrypto-org/blockchain-papers)

### Books


---

## Contribute

Contributions welcome!

1.  Fork it (<https://github.com/nathass-the-legend/blockchain-tech-slack/fork>)
2.  Clone it (`git clone https://github.com/nathass-the-legend/blockchain-tech-slack`)
3.  Create your feature branch (`git checkout -b your_branch_name`)
4.  Commit your changes (`git commit -m 'Description of a commit'`)
5.  Push to the branch (`git push origin your_branch_name`)
6.  Create a new Pull Request

If you found this resource helpful, give it a 🌟 otherwise contribute to it and give it a ⭐️.