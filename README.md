# Algorand Certificate Verifier

A blockchain-based system to issue and verify certificates on the Algorand network.

## Problem
Fake and tampered certificates are hard to detect. Employers and institutions often have no quick, trustworthy way to verify authenticity.

## Solution
When a certificate is issued, its SHA-256 hash is recorded on the Algorand blockchain. Anyone can later upload the certificate (or enter its ID), the app recomputes the hash and checks it against the on-chain record. If the hashes match, the certificate is genuine.

## Planned Features
- Issue a certificate (store its hash on-chain)
- Verify a certificate by file or certificate ID
- Revoke a certificate (issuer only)
- Simple web interface for issuers and verifiers

## Tech Stack
- Algorand TestNet
- AlgoKit
- Algorand Python (algopy) for the smart contract
- TypeScript / React for the frontend

## Project Structure
```
.
├── README.md
├── .gitignore
└── docs/
    └── project-plan.md
```
More folders (`smart_contracts/`, `frontend/`, `tests/`) will be added as development progresses during the course.

## Status
🚧 In progress. Built step by step as part of the Algorand course.

## Getting Started
Setup instructions will be added once the first smart contract is ready.

## License
MIT
