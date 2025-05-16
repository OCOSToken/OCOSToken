# OCOS UK – Bug & Security Tracker

This repository contains the official GitHub Project configuration for managing bugs, vulnerabilities, and infrastructure issues across the OCOS UK decentralized ecosystem.

## Purpose

This `project.yml` file defines a standardized board for tracking all technical issues related to:

- Smart contract logic (ERC-20, BEP-20, TRC-20)
- Wallet UI/UX bugs (Trust Wallet, MetaMask, Binance Web3)
- Staking, airdrop, and liquidity pool discrepancies
- Audit findings from CertiK, Skynet, or other third-party security reviews
- Metaverse and OCOS AI platform functionality

## Board Structure

The project board includes the following columns:

- **New Reports** – Freshly submitted bugs and findings  
- **Confirmed & Triaged** – Verified issues with assigned priority/severity  
- **In Progress** – Items currently under investigation or being resolved  
- **Ready for Testing** – Fixes waiting for QA or audit review  
- **Resolved / Patched** – Issues that have been successfully fixed  
- **Closed / No Action Needed** – Invalid, duplicate, or declined reports

## Labels Used

This board uses a consistent labeling system to streamline filtering and prioritization:

- `status:new`, `status:in-progress`, `status:resolved`, `status:closed`
- `priority:high`, `priority:medium`, `priority:low`
- `severity:critical`, `severity:medium`, `severity:low`
- `component:smart-contract`, `component:wallet-ui`, `component:airdrops`
- `source:internal`, `source:community`, `source:CertiK`

## How to Use

If you're contributing or reporting bugs:

1. Open a GitHub Issue with a descriptive title and clear reproduction steps.
2. Assign the issue with appropriate labels (`component`, `severity`, etc.).
3. Our team will triage the issue and update its progress through the board.
4. Once resolved, the issue will be closed with documentation of the fix.

## Optional: CLI-Based Project Creation

To create this board automatically from the YAML file, use GitHub CLI:

```bash
gh project create --config .github/project.yml
