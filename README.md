# Haze Audits

Haze Finance is an anonymous tokens mixing protocol. The core contracts that utilize zkSNARK for mixing is built on-top of the well known Tornado.cash contracts. We decided to use Tornado's zkSNARK contracts as our base because they have been battled tested in production with hundreds millions of cash flow and audited by well know firms. Since these are the contracts that handles user funds, we wanted to make as little change as possible to avoid introducing unnecessary complexities. Only minor changes were made to allow the implementation of our new frequency mining system. 

## Diff Report Tornado vs Haze

https://www.diffchecker.com/mWjq1FZQ

Changes:
- Added state variables and functions for protocol fee.
- Added state variable and function block list.
- Added setters for new state variables
- Name changes

You can find the original audit report for the Tornado contracts here:
- https://tornado.cash/Tornado_cryptographic_review.pdf
- https://tornado.cash/Tornado_solidity_audit.pdf
- https://tornado.cash/Tornado_circuit_audit.pdf
