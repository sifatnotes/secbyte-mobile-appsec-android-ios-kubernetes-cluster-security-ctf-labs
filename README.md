# secbyte-mobile-appsec-android-ios-kubernetes-cluster-security-ctf-labs
A practical collection of cybersecurity CTF labs covering Mobile Application Security &amp; Reverse Engineering (Android permissions/data storage, APK decompilation/JADX, iOS security baselines, mobile API security, OTP authentication bypasses, Android banking malware analysis, mobile device forensics) and Cloud-Native Container Security 
# Mobile App Security (Android/iOS), APK Reverse Engineering, Mobile Forensics & Kubernetes Cluster Defense CTF Labs

Welcome to the **Mobile App Security (Android/iOS), APK Reverse Engineering, Mobile Forensics & Kubernetes Cluster Defense CTF Lab Collection**. This repository serves as an organized, searchable catalog of practical cybersecurity labs hosted on Learn SecByte.

This collection focuses on mobile ecosystem defense (Android & iOS) and cloud-native container security—spanning **Mobile Security Fundamentals, Android & iOS Architecture (Android permissions model, protected storage, sandbox isolation, iOS security controls)**, **APK Decompilation, Mobile Reverse Engineering & Banking Malware Triage (JADX decompilation, Smali code modification, static analysis, Android banking malware casefiles)**, **Mobile API, OTP & Device Forensics (Mobile API traffic interception, OTP/biometric authentication bypasses, mobile device forensics, forensic log parsing)**, and **Kubernetes Cluster Assessment & Cloud-Native Incident Response (K8s cluster auditing, RBAC privilege escalation, pod escape vectors, container breach incident response)**.

---

## Lab Collection Index

### 1. Mobile Security Fundamentals, Android & iOS Architecture
* **Mobile Security Fundamentals: Android App Defense Lab**  
  *Lab Link:* [https://learn.secbyte.org/ctf/mobile-security-fundamentals-android-app-defense-lab](https://learn.secbyte.org/ctf/mobile-security-fundamentals-android-app-defense-lab)  
  *Focus:* Understanding core mobile security architecture, configuring Android application defense baselines, enforcing secure data storage in shared preferences/SQLite databases, and auditing AndroidManifest.xml components.

* **Android Security Basics: From Permissions to Protected Data**  
  *Lab Link:* [https://learn.secbyte.org/ctf/android-security-basics-from-permissions-to-protected-data](https://learn.secbyte.org/ctf/android-security-basics-from-permissions-to-protected-data)  
  *Focus:* Auditing normal, dangerous, and signature-level Android permissions; identifying exported components (activities, services, broadcast receivers, content providers); and protecting sensitive app data.

* **iOS Security Basics**  
  *Lab Link:* [https://learn.secbyte.org/ctf/ios-security-basics](https://learn.secbyte.org/ctf/ios-security-basics)  
  *Focus:* Understanding iOS security architecture—App Sandbox isolation, Keychain encryption services, Secure Enclave mechanics, ATS (App Transport Security) enforcement, and ASLR/code signing.

<Image src="image_agent_tag_13477674689706763420" alt="Android Multi-Layered Security and Permissions Sandbox Model Diagram" caption="Android Application Security & Sandbox Isolation Architecture" />

---

### 2. APK Decompilation, Mobile Reverse Engineering & Malware Triage
* **APK Under the Hood**  
  *Lab Link:* [https://learn.secbyte.org/ctf/apk-under-the-hood](https://learn.secbyte.org/ctf/apk-under-the-hood)  
  *Focus:* Unpacking Android Application Packages (`.apk`), extracting DEX files (`classes.dex`), inspecting binary resources, decompiling bytecode into Java using JADX/apktool, and analyzing native shared libraries (`.so`).

* **Mobile App Analysis: The Vault Courier**  
  *Lab Link:* [https://learn.secbyte.org/ctf/mobile-app-analysis-the-vault-courier](https://learn.secbyte.org/ctf/mobile-app-analysis-the-vault-courier)  
  *Focus:* Reversing hardcoded cryptographic keys, analyzing custom obfuscation schemes, patching Smali bytecode to bypass client-side security checks, and repacking/re-signing APKs.

* **Mobile Penetration Testing: Android App Assessment Lab**  
  *Lab Link:* [https://learn.secbyte.org/ctf/mobile-penetration-testing-android-app-assessment-lab](https://learn.secbyte.org/ctf/mobile-penetration-testing-android-app-assessment-lab)  
  *Focus:* Executing comprehensive mobile application penetration tests—intercepting mobile traffic, dynamic instrumentation using Frida, bypassing SSL pinning, and hooks on runtime methods.

* **Android Malware Analysis: ShadowBank Casefile**  
  *Lab Link:* [https://learn.secbyte.org/ctf/android-malware-analysis-shadowbank-casefile](https://learn.secbyte.org/ctf/android-malware-analysis-shadowbank-casefile)  
  *Focus:* Reverse-engineering malicious Android banking trojans—analyzing overlay attacks, SMS hijacking mechanisms, accessibility service abuse, and command-and-control (C2) communication channels.

### 3. Mobile API Security, Authentication & Forensics
* **Mobile API Security: Clinic Companion Breach**  
  *Lab Link:* [https://learn.secbyte.org/ctf/mobile-api-security-clinic-companion-breach](https://learn.secbyte.org/ctf/mobile-api-security-clinic-companion-breach)  
  *Focus:* Auditing API backends servicing mobile clients—identifying broken object level authorization (BOLA), hardcoded API tokens inside mobile binaries, and unencrypted REST endpoints.

* **Mobile Authentication Security: From OTP Weaknesses to App Binding**  
  *Lab Link:* [https://learn.secbyte.org/ctf/mobile-authentication-security-from-otp-weaknesses-to-app-bo](https://learn.secbyte.org/ctf/mobile-authentication-security-from-otp-weaknesses-to-app-bo)  
  *Focus:* Exploiting weaknesses in mobile multi-factor authentication—bypassing OTP verification routines, rate-limit flaws in mobile auth flows, biometrics bypass, and device-binding token manipulation.

* **Mobile Device Forensics: Signal Secrets & Shadow Logs**  
  *Lab Link:* [https://learn.secbyte.org/ctf/mobile-device-forensics-signal-secrets-shadow-logs](https://learn.secbyte.org/ctf/mobile-device-forensics-signal-secrets-shadow-logs)  
  *Focus:* Extracting digital evidence from mobile physical/logical dumps—analyzing SQLite database files (`/data/data/`), parsing system logcat streams, extracting encrypted chat artifacts, and mapping timeline events.

### 4. Kubernetes Cluster Security & Incident Response
* **Kubernetes Security Assessment: Cluster Under Pressure**  
  *Lab Link:* [https://learn.secbyte.org/ctf/kubernetes-security-assessment-cluster-under-pressure](https://learn.secbyte.org/ctf/kubernetes-security-assessment-cluster-under-pressure)  
  *Focus:* Auditing Kubernetes cluster security configurations—evaluating Role-Based Access Control (RBAC) misconfigurations, identifying vulnerable pod security standards, container escape vectors, and node-level privilege escalations.

<Image src="image_agent_tag_13477674689706766243" alt="Kubernetes Cluster Architecture Diagram including Control Plane and Worker Nodes" caption="Kubernetes Control Plane & Worker Node Infrastructure Architecture" />

---

* **Kubernetes Incident Response: Cluster Breach Triage**  
  *Lab Link:* [https://learn.secbyte.org/ctf/kubernetes-incident-response-cluster-breach-triage](https://learn.secbyte.org/ctf/kubernetes-incident-response-cluster-breach-triage)  
  *Focus:* Triaging containerized environment security incidents—analyzing audit logs (`kube-audit.log`), detecting malicious daemonsets, inspecting compromised pod runtime environments, and executing containment routines.

---

## Learning Path

### Path A: Mobile Application Security & Reverse Engineer
1. **Basics & Architecture:** Start with [Mobile Security Fundamentals](https://learn.secbyte.org/ctf/mobile-security-fundamentals-android-app-defense-lab), [Android Security Basics](https://learn.secbyte.org/ctf/android-security-basics-from-permissions-to-protected-data), and [iOS Security Basics](https://learn.secbyte.org/ctf/ios-security-basics).
2. **Reverse Engineering & Malware:** Recompile and analyze binaries via [APK Under the Hood](https://learn.secbyte.org/ctf/apk-under-the-hood), [Mobile App Analysis](https://learn.secbyte.org/ctf/mobile-app-analysis-the-vault-courier), [Mobile Penetration Testing](https://learn.secbyte.org/ctf/mobile-penetration-testing-android-app-assessment-lab), and [Android Malware Analysis](https://learn.secbyte.org/ctf/android-malware-analysis-shadowbank-casefile).

### Path B: Mobile API, Authentication & Forensic Examiner
1. **API & Auth Security:** Audit mobile backends via [Mobile API Security](https://learn.secbyte.org/ctf/mobile-api-security-clinic-companion-breach) and [Mobile Authentication Security](https://learn.secbyte.org/ctf/mobile-authentication-security-from-otp-weaknesses-to-app-bo).
2. **Mobile Forensics:** Extract mobile artifacts in [Mobile Device Forensics](https://learn.secbyte.org/ctf/mobile-device-forensics-signal-secrets-shadow-logs).

### Path C: Kubernetes & Container Security Specialist
1. **Cluster Security Audit:** Audit cluster boundaries in [Kubernetes Security Assessment](https://learn.secbyte.org/ctf/kubernetes-security-assessment-cluster-under-pressure).
2. **Container Incident Response:** Triage k8s breaches in [Kubernetes Incident Response](https://learn.secbyte.org/ctf/kubernetes-incident-response-cluster-breach-triage).

---

## How to Use the Labs

1. Select a practice scenario from the **Lab Collection Index**.
2. Click the corresponding direct link to launch the exercise environment hosted on Learn SecByte.
3. Review scenario directives, target APK/IPA binaries, mobile SQLite databases, Frida scripts, or Kubernetes manifests (`.yaml`).
4. Decompile APKs with JADX, bypass SSL pinning using Frida hooks, extract mobile device log artifacts, evaluate K8s RBAC bindings, or triage compromised Kubernetes pod logs to capture flags.

---

## Target Audience

* **Mobile Application Security Engineers & Pentesters:** Decompile Android APKs, dynamic hook using Frida, audit iOS Keychain security, and test mobile APIs.
* **Malware Analysts & Mobile Forensics Examiners:** Dissect Android banking trojans, analyze overlay malware, extract SQLite databases, and parse system logcat streams.
* **Cloud Security & Kubernetes Engineers:** Audit k8s RBAC policies, harden pod security standards, and triage containerized environment security incidents.
* **Cybersecurity Students:** Acquire practical hands-on experience in Android/iOS application security, mobile reverse engineering, and cloud-native container security.

---

## Disclaimer

All lab links provided in this repository direct to official training environments hosted on Learn SecByte. All materials and exercises are provided strictly for educational purposes, defensive skill building, and authorized security research. Reverse-engineering commercial apps or unauthorized cluster security testing against production systems without prior consent is strictly prohibited.
