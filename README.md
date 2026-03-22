# TSwap — DeFi Invariants & Protocol Security Portfolio Project

## Overview
TSwap is a DeFi-focused security project used to study invariant thinking, token edge cases, and AMM-style design assumptions. This repository highlights how protocol logic can fail even when individual functions appear correct.

## Why This Project Matters
TSwap is valuable for showcasing intermediate-to-advanced audit skills:
- Invariant-based reasoning
- Weird ERC20 behavior handling
- AMM / DeFi accounting analysis
- Protocol-level failure modes

## Objectives
- Understand the economic and technical design of the protocol
- Review swap/accounting assumptions
- Test invariant preservation under edge cases
- Document exploitable design flaws and mitigations

## Scope
Primary review areas:
- Swap mechanics
- Reserve/accounting updates
- ERC20 transfer assumptions
- Liquidity and pricing logic
- Protocol invariants under stress

## Security Themes
- Broken core invariants
- Fee/accounting inconsistencies
- Non-standard ERC20 behaviors
- Unsafe assumptions around token transfers
- Design-level weaknesses in DeFi state machines

## What This Repository Shows
- Invariant notes and hypotheses
- Security findings with economic context
- Proof-of-concept or invariant tests
- Design pattern observations
- Protocol risk documentation

## Suggested Repository Structure
```text
TSwap/
├── README.md
├── findings/
│   ├── H-01-invariant-break.md
│   └── M-01-weird-erc20.md
├── invariants/
│   └── invariant-notes.md
├── poc/
│   ├── invariant-break.t.sol
│   └── weird-token.t.sol
└── report/
    └── audit-report.md
```

## Key Learning Outcomes
- Invariants are often more important than line-by-line checks
- Weird ERC20s break naive assumptions quickly
- DeFi bugs are frequently accounting or design bugs
- Economic reasoning is critical in protocol audits

## Run Locally
```bash
forge install
forge build
forge test
forge test --match-test invariant
```

## Portfolio Value
This project demonstrates strong DeFi audit thinking: invariant design, state accounting review, and exploit-focused validation.

## Disclaimer
This repository is for educational, research, and portfolio purposes only.
