<div align="center">
  <img src="https://avatars.githubusercontent.com/u/247997814?s=200&v=4" alt="Fabricked Logo" width="150"/>

  # Fabricked Attack
  **Misconfiguring Infinity Fabric to Break AMD SEV-SNP**

  [![Website](https://img.shields.io/badge/Website-fabricked--attack.github.io-blue?style=flat-square)](https://fabricked-attack.github.io/)
  [![CVE](https://img.shields.io/badge/CVE-2025--54510-red?style=flat-square)](https://fabricked-attack.github.io/)
  [![Conference](https://img.shields.io/badge/USENIX_Security-2026-success?style=flat-square)](https://fabricked-attack.github.io/)
</div>

---

## 🚨 Overview

**Fabricked** is a novel, software-based attack that manipulates memory routing to compromise **AMD SEV-SNP** (Secure Encrypted Virtualization-Secure Nested Paging). By redirecting memory transactions via the Infinity Fabric, a malicious hypervisor can deceive the AMD Secure Processor (PSP) into improperly initializing SEV-SNP. 

This enables an attacker to perform arbitrary read and write operations within the Confidential Virtual Machine's (CVM) address space, completely breaking SEV-SNP's core security guarantees.

* **Deterministic**: 100% success probability.
* **Software-Only**: Requires no physical access to the hardware.
* **Independent**: Does not rely on any code execution inside the victim CVM.

## 🗂️ Organization Repositories

This organization hosts the code, research data, and documentation associated with the Fabricked vulnerability.

* [**`fabricked-attack.github.io`**](https://github.com/Fabricked-Attack/fabricked-attack.github.io): The source code for our informational landing page.
* [**`fabricked-poc`**](https://github.com/Fabricked-Attack/PoC): Proof-of-concept exploit code demonstrating the Infinity Fabric misconfiguration on AMD Zen 5 EPYC processors.

## 📖 The Paper

Our research has been accepted at the **35th USENIX Security Symposium (USENIX Security '26)**.

```bibtex
@inproceedings{schlueter2026fabricked,
  title={{Fabricked: Misconfiguring Infinity Fabric to Break AMD SEV-SNP}},
  author={Benedict Schl{\"u}ter and Christoph Wech and Shweta Shinde},
  booktitle={35th USENIX Security Symposium (USENIX Security 26)},
  year={2026},
  month = aug,
  address = {Baltimore, MD},
  publisher = {USENIX Association},
}