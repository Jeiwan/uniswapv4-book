# Uniswap V4 Development Book

🚧🚧🚧🚧🚧🚧🚧🚧🚧 🚨 🚧🚧🚧🚧🚧🚧🚧🚧🚧 🚨 🚧🚧🚧🚧🚧🚧🚧🚧🚧 

🚧🚧🚧🚧🚧🚧🚧🚧🚧&nbsp;&nbsp;&nbsp;&nbsp;WORK IN PROGRESS&nbsp;&nbsp;&nbsp;&nbsp;🚧🚧🚧🚧🚧🚧🚧🚧🚧

🚧🚧🚧🚧🚧🚧🚧🚧🚧 🚨 🚧🚧🚧🚧🚧🚧🚧🚧🚧 🚨 🚧🚧🚧🚧🚧🚧🚧🚧🚧 

## Preliminary Table of Contents
0. Introduction
  - How Markets Work
    - [ ] Copy from V3, improve smth
  - Constant Function Market Maker
    - [ ] Copy from V3, improve smth
  - Concentrated Liquidity
    - [ ] Tell about the innovation V3 brings
  - Uniswap V4
    - [ ] Tell what V4 brings (more engineering, actions grouping, single contract, hooks)
  - Development Environment
    - [ ] Maybe some more info about Ethereum (e.g. some illustrations)
    - [ ] Focus on Foundry/Forge only
  - What We'll Build
    - [ ] Copy from V3, improve smth

1. Providing Liquidity
  - Introduction
    - [ ] Copy from V3, improve smth
  - Calculating Liquidity
    - [ ] Copy from V3, improve smth
  - Providing Liquidity
    - [ ] Copy from V3, improve smth
    - [ ] Use `PoolManager` as the contract, but store only 1 pool
    - [ ] Skip unlock/deltas for now
  - Accounting
    - [ ] Unlock (sequence diagram)
    - [ ] Deltas tracking
    - [ ] Finished liquidity provision (settle debt)
  - Ticks Indexing
    - [ ] Copy from Tick Bitmap Index
    - [ ] Copy from Generalized Minting
    - [ ] Improve illustrations and probably rewrite
    - [ ] Improve wording, mention the LE implementation (there was a lot of confusion)

2. Swapping
  - Introduction
    - [ ] Copy from V3, improve smth
  - First Swap
    - [ ] Copy from V3, improve smth
    - [ ] Maybe not necessary (go to amt calc right away and then implement swap)
  - Output Amount Calculation
    - [ ] Copy from V3, improve smth
    - [ ] Add Math in Solidity
  - Finished Swapping
    - [ ] Copy from Generalized Swapping
    - [ ] Better title, should finish First Swap
    - [ ] Settle debt, take credit
  - Deployment
    - [ ] Copy from V3, improve smth

3. Cross-position Swapping
  - Introduction
    - [ ] Copy from V3, improve smth
  - Different Price Ranges
    - [ ] Copy from V3, improve smth
  - Cross-tick Swaps
    - [ ] Copy from V3, improve smth
  - Slippage Protection
    - [ ] Copy from V3, improve smth
  - Liquidity Calculation
    - [ ] Copy from V3, improve smth
  - A Little Bit More on Fixed-Point Numbers
    - [ ] Copy from V3, improve smth

4. Multi-pool Swapping
  - Introduction
    - [ ] Copy from V3, improve smth
  - Multiple Pools in One Contract
    - [ ] Upgrade PoolManager to support multiple pools
    - [ ] Add/upgrade `initialize()`
  - Router Contract
    - [ ] Build a basic router
    - [ ] Use the router for multi-pool swaps
    - [ ] Settle/take via the router
  - Tick Rounding
    - [ ] Check if still needed, maybe merge with a previous subchapter

5. Swap and Protocol Fees
  - Introduction
    - [ ] Copy from V3, improve smth
  - Swap Fees
    - [ ] Likely full rework
  - Protocol Fees
    - [ ] Copy from V3, improve smth

6. Hooks
  - Introduction
    - [ ] Why hooks are needed
    - [ ] Hook examples (https://github.com/ora-io/awesome-uniswap-hooks)
  - How Hooks Work
    - [ ] Pre/post
  - Hook Contract Address Generation
    - [ ] Security (hook address commits to pool id)
  - Adding Hooks
    - [ ] Static hooks
    - [ ] Hooks that modify swap/liquidity amounts
  - Dynamic LP Fees

7. Periphery Contracts
  - [ ] Probably just an overview of important contracts (PM, Quoter)