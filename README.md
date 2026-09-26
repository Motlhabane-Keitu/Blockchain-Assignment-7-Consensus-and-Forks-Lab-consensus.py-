# Blockchain-Assignment-7-Consensus-and-Forks-Lab-


## Overview of the assignment

This group assignment examines how blockchain nodes choose which chain to follow and how confirmations help determine when a cross-border payment can be accepted.

The assignment consists of three parts, weighted **60% / 20% / 20%**.

## Part A: Three-Node Simulation and Fork Resolution (60%)

For this part we create a three-Node simulation then create and resolve a Fork. The simulation demonstrate how nodes resolve the fork using either:
- **Longest-chain rule:** Select the valid chain containing the most blocks.
- **Heaviest-work rule:** Select the valid chain with the greatest cumulative proof of work, if cumulative PoW is implemented.
Candidate chains are validated before they are compared. 

We then do edge cases. We document the following situations:
- **Ties:** Explain how a node chooses between chains with equal length or equal cumulative work.
- **Delayed block arrival:** Demonstrate how nodes may temporarily disagree because they receive blocks at different times.
- **Chain reorganisation:** Explain what happens when a node switches to a competing branch, including the effect on payments in the losing branch.
- **Confirmation depth:** Explain how confirmations are counted and what they mean for a payment of **R10 000 equivalent**.


## Part B: Block Relay Time and Confirmation Policy (20%)

This part use **Mastering Bitcoin, Chapter 11**, to explain how blocks propagate through the network. 

The discussion cover:
- How a newly mined block reaches other nodes.
- How propagation delays can produce different local views of the blockchain.
- How temporary forks affect confidence in a payment.
- How waiting for additional confirmations affects payment processing time.

Part B also distinguish **block relay time**, which concerns the spread of a block, from **confirmation waiting time**, which concerns additional blocks being mined above a payment.

## Part C: Cross-Border Retail Payment Memo (20%)
The memo discuss:
- The trade-off between payment speed and reversal risk.
- The effects of network delays and competing branches.
- A reasoned confirmation policy for a R10 000 equivalent payment.
- The assumptions and limitations behind the proposed policy.
- Differences between probabilistic finality in PoW systems and finality under a BFT protocol’s assumptions.

## Deliverables

What is included in this respiratory is

- One group PDF of 4–6 pages covering Parts A–C and also short statement from each group member.
- A python code 


