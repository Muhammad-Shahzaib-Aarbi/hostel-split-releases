# Changelog

All notable public releases of **HostelSplit** are documented in this file.

---

## [v1.4.45] — Build 48 (2026-10-10)
- **Download**: [HostelSplit-v1.4.45.apk](https://hostelsplit-app.surge.sh/HostelSplit-v1.4.45.apk)
- Added optional 4-Digit App Lock PIN (salted SHA-256) with 60-second background auto-lock for shared hostel phones.
- Enforced server-side anti-self-verification and upper amount/title bounds in Firestore Rules + new Firebase Cloud Storage security rules (`storage.rules`).
- Hardened Android WebView & Network Security Config (`network_security_config.xml`, disabled file/content access, disabled release WebView debugging, system-only CAs).
- Upgraded OTA Update System: `minRequiredVersion` mandatory update enforcement, foreground resume check, live PWA cache refresh, post-update confirmation toast, and GitHub Releases mirror links.
- Removed redundant bottom floating APK banner and added Splitwise-style per-bill share breakdown & instant `Settle Cash` button in Friend History.

---

## [v1.4.44] — Build 47 (2026-10-10)
- **Download**: [HostelSplit-v1.4.44.apk](https://hostelsplit-app.surge.sh/HostelSplit-v1.4.44.apk)
- Hardened Firestore Security Rules with participant-only expense reads, field-restricted updates, and non-anonymous auth enforcement.
- Removed Guest Login & anonymous session fallback; added full user-scoped local cache cleanup on logout and account deletion.
- Fixed equal-split rupee remainder allocation (exact sum without Rs 5 rounding drift) and blocked scientific notation in amount inputs.
- Eliminated loose first-name/substring matching collisions and added atomic `writeBatch` + automatic rollback on failed writes.
- Upgraded Groups & Friend History per-bill settled badges with chronological FIFO waterfall calculation.

---

## [v1.4.43] — Build 46 (2026-10-10)
- **Download**: [HostelSplit-v1.4.43.apk](https://hostelsplit-app.surge.sh/HostelSplit-v1.4.43.apk)
- Full 39-file stability & precision update: fixed group split manual share calculation and removed duplicate `'You'` participant bug.
- Fixed Friend History & Settle Modal badge accuracy so owed debts never display as Settled prematurely.
- Fixed Recently Settled incoming/outgoing sign indicators and Friends Directory Hostel IDs.
- Restored Edit & Delete options for unsettled personal/group/loan expenses while keeping paid settlements locked.
- Improved CSV Report export, Profile photo compression, and Service Worker caching.
