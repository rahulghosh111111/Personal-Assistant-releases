 <div align="center">

<!-- Animated Header -->
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:020617,40:0F172A,100:2563EB&height=230&section=header&text=IRA%20ASSISTANT&fontSize=65&fontColor=FFFFFF&fontAlignY=36&animation=fadeIn&desc=PRIVATE%20RELEASES%20%E2%80%A2%20SECURE%20OTA%20DISTRIBUTION&descSize=17&descAlignY=57" width="100%" />

<!-- Typing Animation -->
<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=700&size=19&duration=3000&pause=1000&color=38BDF8&center=true&vCenter=true&width=750&height=55&lines=Your+Personal+Desktop+Intelligence.;Voice-Locked+%7C+Privacy-First+%7C+Offline.;Secure+Over-The-Air+Update+Infrastructure.;No+External+AI+API+Keys+Required.;Coming+Soon+New Year+2027.;...Microsoft Store..." alt="Typing Animation" />

<br/>

<!-- Main Badges -->
<p>
<img src="https://img.shields.io/badge/ACCESS-INVITE%20ONLY-F59E0B?style=for-the-badge&logo=github&logoColor=black"/>
<img src="https://img.shields.io/badge/SECURITY-ENCRYPTED%20%26%20SIGNED-10B981?style=for-the-badge&logo=letsencrypt&logoColor=white"/>
<img src="https://img.shields.io/badge/PLATFORM-WINDOWS%2010%20%7C%2011-0078D6?style=for-the-badge&logo=windows&logoColor=white"/>
</p>

<p>
<img src="https://img.shields.io/badge/TEST%20SUITE-1%2C900%2B%20PASSING-6366F1?style=flat-square"/>
<img src="https://img.shields.io/badge/ARCHITECTURE-LOCAL--FIRST-06B6D4?style=flat-square"/>
<img src="https://img.shields.io/badge/AI%20API%20KEY-NOT%20REQUIRED-22C55E?style=flat-square"/>
</p>

<br/>

**A private release infrastructure for Ira Assistant.**

*Secure distribution. Verified updates. Privacy-focused desktop intelligence.*

</div>

---

## 🔐 Restricted Access Notice

> [!CAUTION]
> **PRIVATE DISTRIBUTION — AUTHORIZED USERS ONLY**
>
> The release binaries hosted in this repository are not intended for public consumption.
>
> Release artifacts are encrypted at rest and cryptographically signed. Decryption and installation require an authenticated Ira Assistant installation and a personal cryptographic invite key issued by the owner.
>
> Downloading individual release artifacts manually will not provide a usable application.

---

## ⚡ 01. About Ira Assistant

**Ira Assistant** is a private, local-first, voice-locked desktop assistant engineered for Windows.

Designed to provide intelligent desktop interaction without depending on external cloud AI services or paid AI API keys.

It combines offline voice recognition, command execution, local intelligence, computer vision, and desktop automation into one unified assistant.

### ✨ Core Capabilities

| Feature | Description |
|:---|:---|
| 🎙️ Voice Intelligence | Offline wake-word detection, voice activity detection and speech recognition |
| 🌐 Multilingual Support | English, Hindi, Bengali, Hinglish and Banglish |
| 🔐 Voice Authentication | Owner-specific voiceprint verification |
| 🧠 Local Intelligence | Rules-first command processing with optional local SLM through Ollama |
| 🖥️ Desktop Automation | Application launching, browser workflows and desktop interactions |
| 👁️ Computer Vision | Local OCR and screen-based interaction |
| 🛡️ Security Engine | Risk-based action execution and encrypted audit logs |
| ↩️ Undo System | Reversible action journal for supported operations |
| 📦 Native Desktop Client | Python, PySide6, Qt and ONNX Runtime |
| 🔄 Auto Updates | Automated OTA update checking and installation |

<br/>

<div align="center">

<img src="https://img.shields.io/badge/01-VOICE%20INTELLIGENCE-38BDF8?style=for-the-badge"/>
<img src="https://img.shields.io/badge/02-LOCAL%20INTELLIGENCE-8B5CF6?style=for-the-badge"/>
<img src="https://img.shields.io/badge/03-SECURE%20EXECUTION-10B981?style=for-the-badge"/>

</div>

---

## 🧬 02. Technology Stack

<div align="center">

### Core Technologies

<img src="https://skillicons.dev/icons?i=python,qt,windows,github,git&theme=dark" />

### Intelligence & Processing

<img src="https://img.shields.io/badge/ONNX%20Runtime-005CED?style=for-the-badge&logo=onnx&logoColor=white"/>
<img src="https://img.shields.io/badge/Ollama-111111?style=for-the-badge&logo=ollama&logoColor=white"/>
<img src="https://img.shields.io/badge/Whisper-412991?style=for-the-badge&logo=openai&logoColor=white"/>

</div>

| Layer | Technology |
|:---|:---|
| Programming Language | Python |
| Desktop Interface | PySide6 / Qt |
| Machine Learning Runtime | ONNX Runtime |
| Speech Recognition | Whisper |
| Local Intelligence | Ollama (Optional) |
| Computer Vision | Local OCR and vision components |
| Distribution | GitHub Releases |
| Security | Cryptographic signing and encrypted artifacts |
| Testing | Automated test suite |

---

## 🔄 03. Automated OTA Update Architecture

This repository serves as the **private OTA update upstream** for authorized Ira Assistant installations.

Installed clients periodically check for new releases, validate update signatures, verify authorization and apply eligible updates.

### Update Lifecycle

```mermaid
flowchart TD
    A([GitHub Releases]) --> B[Release Manifest]
    B --> C[Installed Ira Client]
    C --> D{New Update Available?}

    D -->|No| E[Continue Normal Operation]
    D -->|Yes| F[Download Encrypted Artifact]

    F --> G[Cryptographic Signature Verification]
    G --> H{Signature Valid?}

    H -->|No| I[Reject Update]
    H -->|Yes| J[Verify Invite Authorization]

    J --> K{Authorized?}
    K -->|No| L[Reject Installation]
    K -->|Yes| M[Decrypt Payload]

    M --> N[Validate Package]
    N --> O[Atomic Update Installation]
    O --> P([Restart Updated Application])

    style A fill:#1e293b,color:#fff
    style P fill:#065f46,color:#fff
    style I fill:#7f1d1d,color:#fff
    style L fill:#7f1d1d,color:#fff
```

### Update Security Pipeline

| Stage | Operation | Purpose |
|:---|:---|:---|
| 01 | Release Detection | Detect available versions |
| 02 | Signature Verification | Validate artifact authenticity |
| 03 | Invite Verification | Confirm installation authorization |
| 04 | Payload Decryption | Decrypt authorized artifacts |
| 05 | Package Validation | Check package integrity |
| 06 | Atomic Installation | Apply the verified update |
| 07 | Application Restart | Launch the updated client |

> [!IMPORTANT]
> **For Invited Users**
>
> If you have received an official Ira Assistant invitation, do not download release artifacts directly from the Releases tab.
>
> Your initial installation must use the dedicated bootstrap ZIP package and personal `.invite` certificate provided by the owner.
>
> After installation, the application can retrieve eligible future updates automatically.

---

## 🛡️ 04. Security & Privacy Architecture

Security is a fundamental part of Ira Assistant's distribution infrastructure.

### Security Principles

- **Private Distribution:** Access to installation packages is restricted to authorized recipients.
- **Cryptographic Verification:** Release packages must pass signature verification before installation.
- **Encrypted Artifacts:** Release payloads are encrypted at rest.
- **Invite-Based Authorization:** Personal invite certificates control installation authorization.
- **Local Processing:** Voice processing and supported intelligence operations run locally.
- **Privacy-Focused Design:** No personal voice recordings or machine identifiers are intentionally transmitted through the update-checking process.
- **Action Safety:** Risk-based execution controls protect sensitive desktop operations.

### Zero-Cloud AI Philosophy

<div align="center">

<img src="https://img.shields.io/badge/VOICE%20PROCESSING-LOCAL-22C55E?style=flat-square"/>
<img src="https://img.shields.io/badge/COMMAND%20ENGINE-LOCAL-22C55E?style=flat-square"/>
<img src="https://img.shields.io/badge/EXTERNAL%20AI%20API-NOT%20REQUIRED-22C55E?style=flat-square"/>

</div>

Ira Assistant is designed to minimize external dependencies and keep supported intelligence workflows on the user's device.

---

## 📦 05. Release Distribution

<div align="center">

<img src="https://img.shields.io/badge/RELEASE%20CHANNEL-PRIVATE-7C3AED?style=for-the-badge"/>
<img src="https://img.shields.io/badge/UPDATE%20SYSTEM-AUTOMATED-0EA5E9?style=for-the-badge"/>

</div>

### Distribution Model

| Component | Distribution |
|:---|:---|
| Bootstrap Installer | Private distribution |
| Personal Invite Certificate | Individually issued |
| Encrypted Release Artifacts | GitHub Releases |
| Update Manifest | OTA endpoint |
| Update Verification | Client-side verification |
| Installation | Authorized client |

### Release Workflow

```text
DEVELOPMENT
    |
    v
TESTING & VALIDATION
    |
    v
RELEASE PACKAGE GENERATION
    |
    v
ENCRYPTION & SIGNING
    |
    v
GITHUB RELEASE PUBLICATION
    |
    v
AUTHORIZED CLIENT UPDATE
```

---

## 📊 06. Project Quality

<div align="center">

<img src="https://img.shields.io/badge/Automated%20Tests-1%2C900%2B%20Passing-6366F1?style=for-the-badge&logo=pytest&logoColor=white"/>

<br/><br/>

<img src="https://img.shields.io/badge/Design-Privacy%20First-0EA5E9?style=flat-square"/>
<img src="https://img.shields.io/badge/Architecture-Modular-8B5CF6?style=flat-square"/>
<img src="https://img.shields.io/badge/Distribution-OTA-10B981?style=flat-square"/>

</div>

---

## ⚖️ 07. Copyright & Proprietary License

**Copyright © 2026 Rahul Ghosh. All Rights Reserved.**

Ira Assistant and its associated source code, architecture, encrypted release artifacts, and distribution infrastructure are proprietary.

```text
PROPRIETARY SOFTWARE NOTICE

No permission is granted to use, copy, reproduce, reverse-engineer,
decompile, modify, merge, publish, distribute, sublicense, or share
this software or its encrypted release artifacts, in whole or in part,
without explicit written authorization from the copyright holder.

A cryptographically signed invite file issued by the owner constitutes
a non-transferable, revocable license solely for the individual named
within that invite, strictly for their personal, non-commercial use.

Unauthorized redistribution or use is prohibited.
```

---

## 👨‍💻 08. Project Maintainer

<div align="center">

<img src="https://img.shields.io/badge/DEVELOPED%20BY-RAHUL%20GHOSH-38BDF8?style=for-the-badge"/>

<br/><br/>

**Rahul Ghosh**

*Developer & Creator of Ira Assistant*

<br/>

<a href="https://github.com/rahulghosh111111">
<img src="https://img.shields.io/badge/GitHub-Visit%20Profile-181717?style=for-the-badge&logo=github&logoColor=white"/>
</a>

<br/><br/>

**Building private, intelligent and secure desktop experiences.**

<br/>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:020617,50:0F172A,100:2563EB&height=120&section=footer" width="100%"/>

</div>
