---
title: "Digital Identity"
subtitle: "The future is already here, it's just not very evenly distributed. — William Gibson, Neuromancer"
---

## What is digital identity?

Individual identities — ID cards, driver's licenses, passports, etc. — are already making the jump to digital with Mobile Driver's Licenses being piloted in several US states, Brazil, and parts of Canada, not to mention the EU's Digital Identity initiative. Singapore has had a national digital identity, Singpass, for years. The question is not *if* digital identities will become mainstream, but how *how quickly*.

## What is a Verifiable Credential (VC)?

[Verifiable Credentials](https://www.w3.org/TR/vc-data-model-2.0/) are a proposed standard by the [W3C](https://www.w3.org) for the secure, portable, and verifiable exchange of digital identity information. They are designed to be secure, temper-evident, and privacy-preserving, in the sense that they can be verified without involving the original issuer or revealing unnecessary information about the holder.

VCs are remarkably flexible; they can represent any claim about an individual, from foundational identity like a passport or residency permit to specific qualifications like a university degree or professional certification. Essentially, any piece of information that can be verified can be issued as a VC.

A core advantage of this model is **selective disclosure**. This means the holder has granular control over what information they share. Instead of handing over a physical card that reveals a full name, address, and birth date, a user can provide a digital proof that only confirms a specific attribute—such as being over 18 or holding a valid license—without disclosing any other personal details.

Beyond flexibility and privacy, VCs are built on a "Trust Triangle" involving the **Issuer** (the authority), the **Holder** (the individual), and the **Verifier** (the entity requesting proof). This architecture ensures that the Verifier can trust the data because it is cryptographically signed by the Issuer, while the Holder remains the central point of control, preventing the Issuer from tracking where the credential is used.

## What is a Mobile Driver's License (mDL)?

A Mobile Driver's License (mDL) is a digital version of a physical driver's license, standardized under [ISO/IEC 18013-5](https://www.iso.org/standard/69084.html). While it shares the same goal as Verifiable Credentials — providing a secure, privacy-preserving way to prove identity — there are key technical and functional differences.

Both standards rely on public-key cryptography to ensure data integrity and authenticity. However, ISO 18013-5 was specifically architected for the unique requirements of a driver's license, such as high-speed offline verification by law enforcement in areas without internet connectivity. It defines specific protocols for proximity-based data exchange using technologies like NFC, Bluetooth Low Energy (BLE), and QR codes.

In contrast, Verifiable Credentials (VCs) are a more generalized framework designed for any type of claim across the web. While VCs are transport-agnostic, mDLs are tightly coupled to the ISO-defined interaction patterns. Furthermore, while VCs often leverage Decentralized Identifiers (DIDs) for key management, mDLs typically rely on more traditional Public Key Infrastructure (PKI) managed by government issuing authorities.

## What is an identity wallet?

An identity wallet is a secure application on a mobile device that acts as a digital container for your credentials. Much like a physical wallet holds plastic cards, an identity wallet allows you to store, manage, and present digital versions of your identity documents.

Modern identity wallets are designed to be interoperable, supporting both **Verifiable Credentials (VCs)** and **Mobile Driver's Licenses (mDLs)** within a single interface. This unified approach allows users to manage diverse data types—from government-issued IDs to professional certifications—without needing separate apps for different standards.

Security is handled through the device's hardware-backed security modules, such as the Secure Enclave or Trusted Execution Environment (TEE), ensuring that private keys never leave the device. By leveraging biometric authentication (like FaceID or fingerprints), the wallet ensures that only the rightful owner can authorize the sharing of their information, effectively turning the smartphone into a personal, privacy-preserving gateway for digital interactions.

## What is Ammit Wallet?

While identity wallets provide many advantages in terms of privacy and security, they suffer from one fundamental flaw: losing the device means losing access to all of your credentials. Whether from theft, damage, forgotten passcodes, or simply not being in the same room, this means loss of access. Even worse, if the device is compromised, whether by malware or physical attacks, attackers could impersonate you with much worse results than with current systems.

**Ammit Wallet** uses our [failsafe design](/failsafe-design/) to produce an identity wallet that spans devices yet provides security in the event that any device is lost or compromised. You can use any of your devices to present your identity, and replacing a device is quick and easy.
