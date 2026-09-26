# Goodcoin

Goodcoin is a Bitcoin-inspired cryptocurrency project. This repository currently serves as the foundation for a custom Bitcoin Core fork and public mainnet launch plan.

Important: this repository does not contain a complete production BTC implementation by itself. A real Bitcoin fork must start from the official Bitcoin Core source code, then be customized with project-specific consensus parameters, genesis block values, wallet/network settings, and security review.

## Mainnet parameters selected

- Name: Goodcoin
- Symbol: GOOD
- Consensus: Proof of Work (SHA-256)
- Block time: ~600 seconds (10 minutes)
- Initial block reward: 2,500,000 GOOD
- Minimum block reward: 1 GOOD
- Mining model: perpetual PoW with no fixed max supply assumption in the starter plan
- Genesis message: "Goodcoin launched for fair and open digital money - 2026-09-26"
- Network target: production mainnet

## Repository purpose

This repo is intended to hold:

- project metadata and documentation
- custom genesis configuration notes
- consensus parameter definitions
- build/run instructions for a Bitcoin Core-based fork
- planned security and launch checklist

## Recommended approach for a real fork

1. Download the official Bitcoin Core source code.
2. Create a fork branch or a separate repository based on it.
3. Modify consensus parameters and network constants.
4. Replace the genesis block parameters with a custom Goodcoin genesis block.
5. Build and validate on testnet/regtest before any public launch.
6. Conduct security audits, network testing, and wallet validation.
7. Launch mainnet only after community, mining, and economic viability checks.

## Basic project structure

```text
Goodcoin/
├── README.md
├── docs/
│   └── goodcoin-mainnet-parameters.md
└── LICENSE
```

## Genesis block note

The genesis block should carry the exact message:

```text
Goodcoin launched for fair and open digital money - 2026-09-26
```

This message must be encoded correctly in the genesis coinbase transaction and validated against the custom chain parameters.

## Important reality check

Mining alone does not create economic value. For a blockchain to survive and gain traction, you need:

- a real economic model
- a usable wallet
- nodes and miners
- a clear community and release strategy
- market liquidity or exchange support
- security, audits, and long-term maintenance

## Minimal build path

This is the correct high-level process for a production fork:

```bash
# 1. Obtain Bitcoin Core source
# 2. Make your custom chain params changes
# 3. Build the node daemon
# 4. Run a fully synced mainnet node
# 5. Start mining only after network validation
```

## Next step

The next practical step is to create the actual Bitcoin Core fork configuration files and the full deployment checklist inside this repository.
