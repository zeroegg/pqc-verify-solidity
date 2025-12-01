# QLabs PQC Verify - Solidity

**Status**: 🚧 Coming Soon (Beta: Q2 2026)

Solidity library for on-chain verification of PQC signatures.

## Features

- ✅ Verify Dilithium3 signatures on-chain
- ✅ Gas-optimized implementation
- ✅ Compatible with EVM chains
- ✅ Foundry & Hardhat support

## Installation

```bash
npm install @qlabs/pqc-verify-solidity
```

## Usage

```solidity
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.20;

import "@qlabs/pqc-verify-solidity/contracts/PQCVerifier.sol";

contract MyContract {
    function verify(bytes memory message, bytes memory signature, bytes memory publicKey)
        public pure returns (bool)
    {
        return PQCVerifier.verifyDilithium3(message, signature, publicKey);
    }
}
```

## Beta Access

👉 [Join the waitlist](https://api.qlabsai.com) for early access.

---

© 2025 QLabs. MIT License.
