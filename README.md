# Blockchain-Assignment-7-Consensus-and-Forks-Lab-


## Overview of the assignment

This group assignment examines how blockchain nodes choose which chain to follow and how confirmations help determine when a cross-border payment can be accepted.

The assignment consists of three parts, weighted **60% / 20% / 20%**.

## Part A: Three-Node Simulation and Fork Resolution (60%)

### Three-Node Simulation

Start by simulating at least three nodes, named A, B and C. Each node maintains its own local copy of the blockchain and can temporarily hold a different chain.

### Creating and Resolving a Fork

Create two valid competing blocks or chains that share a common ancestor.

The simulation demonstrate how nodes resolve the fork using either:

- **Longest-chain rule:** Select the valid chain containing the most blocks.
- **Heaviest-work rule:** Select the valid chain with the greatest cumulative proof of work, if cumulative PoW is implemented.

Candidate chains must be validated before they are compared. A longer invalid chain must never replace a shorter valid chain.

### Edge Cases

The assignment document the following situations:

- **Ties:** Explain how a node chooses between chains with equal length or equal cumulative work.
- **Delayed block arrival:** Demonstrate how nodes may temporarily disagree because they receive blocks at different times.
- **Chain reorganisation:** Explain what happens when a node switches to a competing branch, including the effect on payments in the losing branch.
- **Confirmation depth:** Explain how confirmations are counted and what they mean for a payment of **R10 000 equivalent**.


## Part B: Block Relay Time and Confirmation Policy (20%)

This part use **Mastering Bitcoin, Chapter 11**, to explain how blocks propagate through the network. 

It also include a diagram showing the relationship between block relay time and confirmation policy for remittances.

The discussion cover:

- How a newly mined block reaches other nodes.
- How propagation delays can produce different local views of the blockchain.
- How temporary forks affect confidence in a payment.
- How waiting for additional confirmations affects payment processing time.

Part B also distinguish **block relay time**, which concerns the spread of a block, from **confirmation waiting time**, which concerns additional blocks being mined above a payment.

## Part C: Cross-Border Retail Payment Memo (20%)

Write a group memo examining confirmation depth for cross-border retail payments.

Use **Decker and Wattenhofer (2013)** and at least **one Byzantine Fault Tolerance (BFT) paper** to support the analysis.

The memo should discuss:

- The trade-off between payment speed and reversal risk.
- The effects of network delays and competing branches.
- A reasoned confirmation policy for a R10 000 equivalent payment.
- The assumptions and limitations behind the proposed policy.
- Differences between probabilistic finality in PoW systems and finality under a BFT protocol’s assumptions.

The proposed confirmation threshold should be justified rather than treated as a universally safe number.

## Deliverables

What is included in this respiratory is

- One group PDF of 4–6 pages covering Parts A–C and also short statement from each group member.
- A python code 

## Learning Outcomes

In summary for this assignment, the group was able to:

- Distinguish local chain validity from agreement between nodes.
- Explain how competing valid blockchain histories arise.
- Implement and explain a fork-choice rule.
- Describe the effects of delayed blocks and reorganisations.
- Calculate confirmation depth.
- Relate blockchain confirmation policies to cross-border payment risk.
