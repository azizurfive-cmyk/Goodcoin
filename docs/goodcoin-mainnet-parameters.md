# Goodcoin mainnet parameters

This file documents the initial production parameters for the Goodcoin blockchain.

## Core identity

- Network name: Goodcoin
- Ticker: GOOD
- Consensus mechanism: Proof of Work
- Hash algorithm: SHA-256
- Block time target: 600 seconds

## Economics

- Initial block reward: 2,500,000 GOOD
- Minimum block reward: 1 GOOD
- Mining continuation: intended to continue indefinitely in the starter configuration
- Supply model: designed to resemble a Bitcoin-like PoW model, but this must be finalized with economic simulation and security review before a public launch

## Genesis block

Genesis message:

```text
Goodcoin launched for fair and open digital money - 2026-09-26
```

This must be embedded in the custom genesis coinbase transaction and accompanied by a valid merkle root, timestamps, and chain parameters.

## Recommended real-world process

A real production fork should follow this sequence:

1. Download the official Bitcoin Core source code.
2. Create a custom branch or repository for Goodcoin.
3. Modify consensus constants and chain parameters.
4. Replace the genesis block with the Goodcoin version.
5. Build and validate on regtest/testnet.
6. Test wallet, RPC, chain sync, and mining behavior.
7. Run a public launch only after community and mining readiness checks.

## Warning

The vector of "just mine directly" is not enough for a blockchain to become valuable. Public awareness, node distribution, wallet support, and exchange liquidity are critical requirements.

## Practical note

This repo is a starting framework, not a complete standalone blockchain implementation. A trustworthy public launch requires an official Bitcoin Core code base, careful code review, and a proper security audit.
