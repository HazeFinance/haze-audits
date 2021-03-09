# Haze Audits

Haze Finance is a private transaction protocol utilizing zkSNARKs to acheive anonymity.

The core contracts that utilize zkSNARK for mixing is built on-top of the well known Tornado.cash contracts. We decided to use Tornado's zkSNARK contracts as our base because they have been battled tested in production with hundreds millions of cash flow and audited by well known firms. Since these are the contracts that handle user funds, we wanted to make as little change as possible to avoid introducing unnecessary complexities. Only minor changes were made to allow the implementation of our new frequency mining system. 

## Diff Report

You can check the code diff report line by line between Tornado's mixing contract (left) vs Haze's mixing contract (right). Changes has been highlighted.

https://www.diffchecker.com/mWjq1FZQ

**Changes:**
- Added state variables and functions for protocol fee for HAZE staking rewards.
- Added state variable and function block list.
- Added setters for new state variables
- Name changes

## Reward and Governance 

Haze Finance introduces a new reward and governance system to acheive a self sustaining DAO that incentivizes anounymous transactions as well as HAZE token holders.

You can find the HAZE reward system and governance contracts at https://github.com/HazeFinance/haze-contracts.

## Original Audit
You can find the original audit report for the Tornado contracts here:
- https://tornado.cash/Tornado_cryptographic_review.pdf
- https://tornado.cash/Tornado_solidity_audit.pdf
- https://tornado.cash/Tornado_circuit_audit.pdf
