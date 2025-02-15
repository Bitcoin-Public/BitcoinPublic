# Bitcoin Public

The goal of Bitcoin Public is to bring enhanced programmability and scalability to Bitcoin's ecosystem while maintaining compatibility with Ethereum Virtual Machine (EVM) standards. To leverage existing developer communities and tooling, we've implemented EVM compatibility through a strategic fork of go-ethereum, while introducing significant improvements to consensus and economic model.

[![API Reference](
https://pkg.go.dev/badge/github.com/ethereum/go-ethereum
)](https://pkg.go.dev/github.com/ethereum/go-ethereum?tab=doc)
[![Discord](https://img.shields.io/badge/discord-join%20chat-blue.svg)](https://discord.gg/YOUR_COMMUNITY_LINK)

Bitcoin Public enhances EVM compatibility with a novel Proof of Staked Threshold (PoST) consensus mechanism featuring:

- 51-node validator network with rotating leadership
- 3-second block times
- Adaptive gas pricing model
- Bitcoin-backed security bonds

**Bitcoin Public** features:

- **Threshold-secured blockchain**: Hybrid Bitcoin script enforcement for validator operations
- **Enhanced EVM compatibility**: Full Ethereum toolchain support with 75% lower average fees
- **Bitcoin-aligned economics**: BPTC token serves as both gas currency and staking asset

## Key Innovations

### Proof of Staked Threshold (PoST)
Combining Bitcoin's security model with modern consensus mechanisms:

1. Validators post Bitcoin-denominated bonds through Taproot commitments
2. Block production follows deterministic validator rotation
3. Slashing conditions enforced through Bitcoin script covenants
4. Fee market dynamically adjusts based on Bitcoin mempool conditions

## Native Token

BPTC (Bitcoin Public Transaction Coin) serves as the network's native currency:

1. Powers smart contract execution (gas)
2. Staking token for validator operations
3. Governance participation

## Building the Source

Follow standard go-ethereum build procedures with enhanced requirements:

```shell
# Requires Go 1.22+ and Rust 1.76+ for threshold cryptography
make bptc
