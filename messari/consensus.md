__Consensus__

Decred employs a hybrid [proof-of-work](https://messari.io/resource/proof-of-work) (PoW) [proof-of-stake](https://messari.io/article/proof-of-stake) (PoS) consensus model that can be thought of in layers. The first layer is powered by [Nakamoto Consensus](https://messari.io/article/nakamoto-consensus), whereby the valid chain is the longest chain with the most accumulated PoW. The second layer is powered by PoS, whereby stakers validate blocks before appending them to the blockchain. The PoS layer acts as a check on miners, ensuring they do not submit deliberately empty or invalid blocks. The PoS layer is also used for Decred's governance process (see governance section for more detail).

In order to participate in PoS consensus one must stake DCR to receive tickets, a non-tradable cryptoasset on the Decred network. Up 20 new tickets are available for purchase each block, with the price of tickets adjusting dynamically every 144 blocks (~12 hours). The price of tickets adjusts in order to keep the Ticket Pool, total number of tickets on the Decred network, near the target pool size of 40,960 tickets. This is done to aid predictability in staking activity, so stakers need not worry about drastically fluctuating parameters that determine how frequently you get to participate in consensus.

Each block 5 tickets are randomly selected by a Poisson distribution to validate blocks produced by POW miners, and vote on Decred governance proposals during voting periods. The average time it takes for a ticket to vote is 28 days, but possibly requiring up to 142 days, with a 0.5% chance of expiring before being chosen to vote (this expiration returns the original Ticket Price without a reward).

__Mining__

Miners solve computational puzzles to generate new blocks using the [BLAKE-256](https://docs.decred.org/research/blake-256-hash-function/) proof-of-work algorithm. In this process, miners compete to generate a [hash](https://messari.io/blog/hash-function) less than the target number set by Decred's [difficulty adjustment algorithm](https://messari.io/resource/difficulty-level). The target difficulty level is adjusted every 144 blocks (~12 hours).

Although open to anyone with a CPU, Decred mining is now dominated by [ASICs](https://messari.io/resource/application-specific-integrated-circuits-asics). In order to smooth individual miner revenue as mining has become more competitive, mining is now done in pools where participants contribute [hash power](https://messari.io/resource/hash-power) to the pool and receive a proportional share of the profits if the pool finds a valid block.

The Decred block reward reduces by a factor of 100/101 every 6,144 blocks (approximately 21.33 days). Furthermore, the Decred block reward is allocated 60% to miners, 30% to stakers, and 10% to the Decred decentralized treasury.
