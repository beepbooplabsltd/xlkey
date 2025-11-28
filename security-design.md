**XL**key™ security design
==========================

## Overview

The **XL**key is a physical adapter device that is designed to convert between the TIA-102.AACD-A KFD protocol at standard 5V levels and Harris 3.3V levels.

| OSI model | TIA-102.AACD-A KFD protocol | Harris protocol             | Notes |
|-----------|-----------------------------|-----------------------------|-------|
| Layer 1   | Three Wire Interface (5V)   | Three Wire Interface (3.3V) |
| *Layer 2* | *Exchange session*          | *Exchange session*          | *Passed transparently*
| *Layer 3* | *Key Management Messages*   | *Key Management Messages*   | *Passed transparently*

It is **not** a cryptographic device: it does not generate keys, store keys, encrypt or decrypt data, or perform any other function of a cryptographic device.

## Details

| Component                  | Notes |
|----------------------------|-------|
| **Algorithms**             | The **XL**key does not implement or use any encryption algorithms in hardware or firmware.
| **Cryptographic boundary** | The **XL**key does not have a cryptographic boundary, as it does not perform any cryptographic operations.
| **Development**            | The **XL**key is designed and tested in the United States by US nationals.
| **FIPS validation**        | The **XL**key is not FIPS validated.
| **Firmware security**      | The **XL**key does not contain any firmware.
| **Keys**                   | The **XL**key does not contain any CSPs or keys.
| **Logging**                | The **XL**key does not perform any logging.
| **Other attacks**          | The **XL**key is not designed to mitigate any specific attacks outside of those listed in this table, including but not limited to power consumption, timing, fault induction, or TEMPEST attacks.
| **Physical security**      | The **XL**key does not include any physical anti-tamper features. All components are general-purpose commodity components; no custom components are used.
| **Ports**                  | The **XL**key provides two physical ports, both of which are used for data input/output. TWI is used for TIA-102.AACD-A KFD protocol. USB-C is additionally used for power.
| **RNG**                    | The **XL**key does not implement or use any random number generators in hardware or firmware.
| **Roles**                  | The **XL**key supports one role: user.
| **Software**               | The **XL**key does not interact with any software.
| **Storage: non-volatile**  | The **XL**key does not contain any non-volatile memory.
| **Storage: volatile**      | The **XL**key does not contain any volatile memory.

## Disclaimer

The above security details apply to a **XL**key as manufactured, using original hardware provided by beep boop labs.

Unauthorized physical access to the **XL**key or radios being keyloaded could result in malicious modifications by a third-party.

⚠️ It is the user's responsibility to maintain physical and electronic control of their **XL**key device, radios they connect it to, and their encryption key material, at all times to prevent tampering.
