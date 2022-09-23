## 🍪 terminology

<br>



* **Block builder**
The agent responsible for assembling the potential contents of a block (i.e. the set of transactions that makes up the “payload” of a block). In Proof of Work Ethereum it’s the miner. In Proof of Stake Ethereum it’s the validator, but this activity can separated from the validator via PBS, in which case builders need to submit bids for blocks to be included to the block proposer for inclusion.

* **Block proposer**
The agent responsible for proposing new blocks in a blockchain. In Proof of Work Ethereum it’s the miner. In Proof of Stake Ethereum it’s the validator.

* **Node Operator**
An organization/entity/person that operates validators.

* **PBS**
Proposer Builder Separation, see: State of research: increasing censorship resistance of transactions under proposer/builder separation (PBS).

* **Staker**: A user/organization/etc. which holds (w)stETH

* `feeRecipient`: field set by the block builder in the block header (coinbase address)

* payment methods on Ethereum:
   - `base_fee`: amount defined by the protocol, always paid from user -> network
   - `priority_fee`: amount defined by the user as `maxPriorityFeePerGas`, paid from user -> coinbase address
   - `block.coinbase transfer`: the EVM has an opcode which allows end user to send fund directly to the coinbase address (same recipient as `priority_fee`
    - `regular transfer`: a transaction created to send eth to other account