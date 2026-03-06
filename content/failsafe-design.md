---
title: "Failsafe Design"
subtitle: "Solutions designed to survive any level of compromise."
---

![United Airlines Flight 328, a Boeing 777 with one engine on fire](/images/ua328.jpg)

United Airlines Flight 328 took off from Denver International Airport heading to Honolulu, Hawaii on February 20, 2021. Shortly after takeoff it suffered a catastrophic engine failure, as shown above. Despite this, the plane returned to Denver and landed safely with no injuries.

## What does it mean for a design to be failsafe?

Traditionally, cybersecurity has focused on building impenetrable walls to prevent any compromise. Even "security in depth" or "layered" security focussing on putting as many barriers between the attacker and any asset. The system is designed to resist compromise, but once a compromise happens it can be catastrophic.

We take a different philosophy, inspired by the aerospace industry. In aircraft design, engineers assume that components *will* fail and build systems that remain operational despite those failures. We apply this same "failsafe" logic to digital assets. Instead of assuming devices or services are perfectly secure, we assume they will eventually be compromised and design systems that maintain security despite these failures.

## How do we achieve failsafe designs?

At Ammit we apply advanced cryptographic techniques, such as Multi-Party Computation (MPC) and threshold signatures (TSS) to ensure failsafe designs. In these systems, secrets are split into multiple "shares" and distributed across devices and services such that no single unit is fully trusted. Devices and services then work together to achieve the desired results without ever consolidating secret information in one place.

## Benefits of failsafe designs using MPC

* Security by design
* Enhanced user privacy
* Easier recovery from lost but not compromised devices
* Easier device or service rollover
* Easier and more secure backups
