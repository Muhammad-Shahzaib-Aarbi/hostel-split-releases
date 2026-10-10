# 🏠 HostelSplit — Official Releases & Android APK

**HostelSplit** is a real-time hostel expense manager, group bill splitter, and debt settlement app built for hostel roommates and students.

---

## 🚀 Latest Release: **v1.4.45 (Build 48)**

- 📱 **[Download Android APK (v1.4.45 • 6.0 MB)](https://hostelsplit-app.surge.sh/HostelSplit-v1.4.45.apk)**
- 🌐 **Launch Web App (PWA)**: [https://hostelsplit.web.app](https://hostelsplit.web.app)
- ⚡ **Mirror Web App**: [https://hostelsplit-app.surge.sh](https://hostelsplit-app.surge.sh)

---

## 🆕 What's New in v1.4.45 (Build 48)
- **Optional 4-Digit App Lock PIN**: Protect your HostelSplit wallet on shared hostel phones with a salted SHA-256 4-digit PIN and automatic 60-second background re-lock.
- **Anti-Self-Verification & Storage Security Rules**: Enforced server-side recipient-only verification on `settlement_paid` claims, upper amount/title bounds in `firestore.rules`, and UID-prefixed 5 MB image rules in `storage.rules`.
- **Android WebView & Network Security Hardening**: Added `network_security_config.xml` (HTTPS-only + system CA trust anchors) and disabled WebView file/content access and release debugging in `MainActivity.java`.
- **5-Point OTA Update Upgrade**: Added `minRequiredVersion` mandatory update enforcement, foreground resume update checks, live Web/PWA cache refresh, post-update confirmation toast, and official GitHub Releases mirror links.
- **UI & Friend History Polish**: Removed the redundant bottom floating APK banner and added Splitwise-style per-bill share breakdowns plus a 1-tap `Settle Cash` button inside Friend History.

---

## ✨ Key Features
- **Group Bill Splitting**: Split meals, utility bills, and shared hostel expenses equally or with custom manual shares.
- **Personal Loans (Lend / Borrow)**: Record 1-on-1 loans with roommates that automatically sync to both wallets.
- **Verified Debt Settlements**: Settle debts via Cash or Online Transfer (Easypaisa, JazzCash, Raast, SadaPay, NayaPay, HBL, Meezan, etc.) with screenshot proof and receiver verification.
- **100% Offline-Ready**: Works seamlessly on spotty hostel Wi-Fi or mobile data with local IndexedDB caching and automatic background sync.
- **In-App Over-The-Air Updates**: Built-in update checker notifies Android users whenever a new APK version is released.

---

## 📲 How to Install on Android
1. Download the latest **`HostelSplit-v1.4.45.apk`** from the **[Releases](https://github.com/Muhammad-Shahzaib-Aarbi/hostel-split-releases/releases)** section or the direct link above.
2. Open the downloaded `.apk` file on your Android phone.
3. If prompted, tap **Settings ➔ Allow from this source**, then tap **Install**.
4. Sign in with your Google account to sync your hostel room ledger!
