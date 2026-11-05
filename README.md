<div align="center">

  <!-- Dynamic Security Header Banner -->
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=12,14,19,24&height=200&section=header&text=Ira%20Assistant%20%E2%80%A2%20Releases&fontSize=50&fontColor=ffffff&animation=fadeIn&fontAlignY=36&desc=Cryptographically%20Signed%20%26%20Encrypted%20OTA%20Distribution%20Channel&descFontSize=17&descAlignY=58" width="100%" alt="Ira Assistant Releases Banner" />

  <!-- Animated Typing SVG -->
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=19&pause=1200&color=38BDF8&center=true&vCenter=true&width=680&lines=Zero-Cloud+Voice-Locked+Desktop+Intelligence;Automated+Over-The-Air+(OTA)+Update+Endpoint;Cryptographically+Signed+%26+Invite-Gated+Payloads;100%25+On-Device+Inference+%E2%80%A2+Zero+External+API+Keys" alt="Ira Telemetry Status" />

  <br/>

  <!-- Security & Platform Badges -->
  <p align="center">
    <img src="https://img.shields.io/badge/DISTRIBUTION-PRIVATE%20%2F%20INVITE--ONLY-F59E0B?style=for-the-badge&logo=github&logoColor=black" alt="Invite Only" />
    <img src="https://img.shields.io/badge/PAYLOADS-ENCRYPTED%20%26%20SIGNED-10B981?style=for-the-badge&logo=letsencrypt&logoColor=white" alt="Encrypted & Signed" />
    <img src="https://img.shields.io/badge/PLATFORM-WINDOWS%2010%2F11%20(x64)-0078D6?style=for-the-badge&logo=windows&logoColor=white" alt="Windows" />
    <img src="https://img.shields.io/badge/TEST%20COVERAGE-1%2C900%2B%20PASSING-6366F1?style=for-the-badge" alt="1900+ Tests" />
  </p>

</div>

---

> [!CAUTION]
> ### 🔒 Restricted Access — Encrypted Binary Artifacts
> **The release binaries hosted in this repository are NOT for public consumption.** 
> All artifacts published here are **encrypted at rest** and **cryptographically signed**. They can only be decrypted and mounted by an existing, authenticated installation of **Ira Assistant** unlocked via a personal cryptographic invite key issued directly by the author. **Downloading these files manually yields nothing executable or usable.**

---

### ⚡ Overview: What is Ira Assistant?

**Ira Assistant** is a private, local-first, voice-locked desktop assistant engineered for Windows. It wakes exclusively to its owner's biometric voiceprint, natively understands **English, Hindi, Bengali, Hinglish, and Banglish**, and orchestrates desktop applications, browser workflows, local files, and screen elements—with **zero cloud AI and no API keys**.

| Core Pillar | Engineering Specification |
| :--- | :--- |
| **🎙️ Acoustic Pipeline** | Offline wake-word detection, Voice Activity Detection (VAD), real-time barge-in, and Whisper STT fine-tuned for Hindi & Bengali accents |
| **🔐 Zero-Trust Security** | Biometric voiceprint lock, risk-rated action execution behind a unified safety gate, reversible undo journal, and encrypted local audit logs |
| **🧠 Hybrid Intelligence** | Deterministic rules-first engine with local SLM (`Ollama`) fallback planning, paired with local OCR & computer vision for screen actuation |
| **📦 Native Client** | Built with `Python`, `PySide6 (Qt)`, and `ONNX Runtime`, featuring a system tray controller, setup wizard, and 1,900+ automated tests |

---

### 🔄 Automated OTA Update Architecture

This repository serves strictly as the **automated Over-The-Air (OTA) update upstream** for authorized client installations. Installed copies poll this endpoint, verify signatures, and apply delta/full updates autonomously in the background.

```text
+-------------------------------------------------------------------------+
|                   IRA ASSISTANT • OTA UPDATE PIPELINE                   |
+-------------------------------------------------------------------------+

  [ GitHub Releases Upstream ]
               |
               |  1. Polls latest release manifest & encrypted artifact
               v
  +-------------------------------------------------------------------+
  |  Local Ira Client (Installed Windows Instance)                    |
  |                                                                   |
  |  ├── Step A: Signature Verification ──> Validates owner's key     |
  |  ├── Step B: Invite Gate Check      ──> Confirms personal license |
  |  ├── Step C: Payload Decryption     ──> Decrypts binary in memory |
  |  └── Step D: Atomic Hot-Swap        ──> Applies self-verified app |
  +-------------------------------------------------------------------+
```

> [!IMPORTANT]
> **For Invited Users:** If the owner shared Ira Assistant with you, **do not download files from the Releases tab.** Always perform your initial installation using the dedicated bootstrap `.zip` package and personal `.invite` certificate sent directly to you. Once installed, your client will fetch future updates from this repository automatically.

---

### 🛡️ Artifact Verification & Security Policy

* **No Public Installer:** Raw bootstrap installers are distributed exclusively through private, out-of-band channels alongside recipient-bound invite files.
* **Tamper Resistance:** Every release package is verified against an embedded public key prior to unpacking. Any modified or unsigned archive is rejected immediately by the updater daemon.
* **Zero Telemetry:** Checking for updates via GitHub's release API transmits zero personal data, voice logs, or machine identifiers.

---

### ⚖️ Copyright & Proprietary License

**Copyright © 2026 [Rahul Ghosh](https://github.com/rahulghosh111111). All rights reserved.**

```text
PROPRIETARY SOFTWARE NOTICE:
No permission is granted to use, copy, reverse-engineer, decompile, modify, merge, 
publish, distribute, sublicense, or share this software or its encrypted release 
artifacts, in whole or in part, without explicit written authorization from the 
copyright holder.

A cryptographically signed invite file issued by the owner constitutes a non-transferable, 
revocable license solely for the individual named within that invite, strictly for their 
personal, non-commercial use.
```

---

<div align="center">
  <a href="https://github.com/rahulghosh111111">
    <img src="https://img.shields.io/badge/←%20Back%20to%20Rahul%20Ghosh's%20Profile-181717?style=for-the-badge&logo=github&logoColor=white" alt="Back to Profile" />
  </a>
</div>
