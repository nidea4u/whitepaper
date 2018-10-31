# BSHA3

BSHA3 is a cryptocurrency much alike those before it. It offers a decentralized means of transparent exchange, a problem perfected by Bitcoin and its Bitcoin Core implementation.

This is the first blockchain ever to use `sha3d`, a double hash function analogous to Bitcoin's `sha256d`. Cryptographers today believe that sha256 is sound and secure. But, if sha3 is also indeed secure, it is valuable to have a chain driven by it instead.

Since SHA256 is included in so many parts of Bitcoin, including address creation and transaction id calculation, these were all worth changing to SHA3-256 as a final step. Interestingly, the random oracle model expressed by these hash functions made this swap not only sound, but also very simple.

Aside from this difference, the main goals of this chain are parity with the intentional, good parts of Bitcoin, and omission of its historical errors. BIPs are also carried over in general; any differences are listed in a working document named BIPMAD - Bitcoin Improvement Proposal Modifications and Deletions.

This blockchain is released to the public on block 250, on October 31, 2018, with 0 halvings done - a 50 BSHA3 coinbase reward - the highest, initial amount. This offers a true decentralization opportunity, for miners themselves to innovate on Keccak-1600 and SHA3d mining performance and drive this chain forward by incentive, sooner than later.

This initial release contains a CPU reference miner that uses `getblocktemplate` to solo mine BSHA3d.

There is no difficulty bomb (auto-hardfork) implemented, ensuring a clear future - 21,000,000 BSHA3 ever, under consensus rules. 100,000,000 satoshis each.

Good luck!


### Blockchain Information

- BIP9 is deployed
- BIP65, 66 are activated
- CheckSequenceVerify is activated
- Segwit is activated

- Checkpoints & latest ChainTxData introduced
- `OP_SHA1` removed, `OP_SHA3` added in its place 
- SHA256 replaced by SHA3-256 in all cases besides Tor
- Same average block time (10min) and supply schedule as Bitcoin

### Libs & Code

- pysha3
- arduino/rweather - arduinolibs/libraries/Crypto

### References

- [Bitcoin Whitepaper (Nakamoto)](https://bitcoin.org/bitcoin.pdf)
- [Bitcoin Core implementation](https://bitcoincore.org/en/download)
- [Keccak / SHA3 spec](https://nvlpubs.nist.gov/nistpubs/fips/nist.fips.202.pdf)
- [Keccak / SHA3 test vectors](https://www.di-mgt.com.au/sha_testvectors.html)

