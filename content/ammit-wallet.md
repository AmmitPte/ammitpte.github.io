---
title: "The Ammit Wallet"
subtitle: "A next-generation MPC wallet for verifiable credentials that survives compromised devices."
---

## What is an MPC Wallet?

Multi-Party Computation (MPC) and threshold cryptography form the foundation of our security architecture. Instead of storing a complete private key on a single device, the key is split into multiple independent "shares" distributed across different parties (e.g., your device, our servers, a backup location).

When a signature is required, these parties participate in a cryptographic protocol to produce the signature *without ever reconstructing the full key on a single device*.

### Why typical wallets fall short
Typical digital wallets store the private key locally on a secure enclave or hardware component on your phone. If your device is compromised, lost, or the OS is exploited, your key and identity are at risk. 

**Ammit is different:** Because your device only holds a share of the credential key, a compromised phone does not equal a compromised identity. Our techniques natively survive compromised devices and services.

---

## Verifiable Credentials Support

The Ammit Wallet is purpose-built for the future of digital identity. We natively support the storage and presentation of **Verifiable Credentials (VCs)**.

- **Mobile Driver's Licenses (mDL)**
- **Digital Passports**
- **Bank Identity Tokens**
- **Any standardized VC**

Combined with our MPC approach, your digital credentials maintain the highest levels of zero-trust security and privacy, ready for use both online and offline without risking widespread identity theft.
