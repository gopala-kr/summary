## <a name='blockchains'> Blockchains
* [Bitcoin-NG: A Scalable Blockchain Protocol](https://www.usenix.org/system/files/conference/nsdi16/nsdi16-paper-eyal.pdf) (2016): Bitcoin-NG (Next Generation) focuses on scalability. It's a Byzantine fault tolerant blockchain protocol that is
robust to extreme churn and shares the same trust model as Bitcoin. The paper also introduces quantitative metrics for evaluating Nakamoto consensus protocols.

* [Blockstack: A Global Naming and Storage System Secured by Blockchains](https://blockstack.org/blockstack.pdf) (2016): This paper presents the design and implementation of Blockstack, a global naming and storage system built on top of a blockchain. Blockstack is agnostic of the underlying blockchain, and currently uses Bitcoin. The paper also describes lessons from a production deployment of an earlier system that was on a smaller blockchain.

## <a name='consensus'> Consensus
* [In Search of an Understandable Consensus Algorithm](https://www.usenix.org/system/files/conference/atc14/atc14-paper-ongaro.pdf) (2014): This paper presents Raft, which is equivalent to multi-Paxos but much easier to understand. There have been dozens of real-world Raft implementations, some of which are in production use, within the couple of years that this work came out.

## <a name='consistency'> Consistency
* [Don’t Settle for Eventual: Scalable Causal Consistency for Wide-Area Storage with COPS](http://www-bcf.usc.edu/~wyattllo/papers/cops-sosp11.pdf) (2011): This paper defines casual+ consistency and presents a key/value store that delivers this consistency model across wide-area networks. The paper is also interesting to get background on different consistency models.

