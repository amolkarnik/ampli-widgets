---
title: Privacy Policy — AmpliWidgets
---

# Privacy Policy

**Effective Date:** October 2026

**AmpliWidgets** ("the App") is an independent utility developed for controlling Marantz and Denon AV receivers via local Wi-Fi and interactive iOS widgets. Your privacy and local network security are paramount.

---

## Summary

**The App collects no personal data, tracks nothing, contains no analytics, and operates zero external servers.** All network communication is strictly confined to your local Wi-Fi network between your Apple device and your AV receiver.

---

## What We Do Not Do

- We do **not** collect, store, or transmit your name, email address, IP address, device identifier, location, or usage analytics.
- We do **not** include third-party SDKs, tracking pixels, telemetric reporting tools, or advertising frameworks.
- We do **not** contact any proprietary remote server, cloud backend, or database.
- We do **not** sell, share, or monetize any data, because no data is ever collected in the first place.

---

## Local Network Access

- **Direct Socket Communication:** The App uses Apple's official `Network.framework` to communicate directly with your AV receiver over your local Wi-Fi network using standard ASCII control protocols on TCP port 23.
- **Bonjour / mDNS Discovery:** On initial setup, the App scans your local network for compatible receiver services (`_heos-audio._tcp`, `_raop._tcp`, `_http._tcp`) to automatically discover your receiver's IP address.
- **Local Network Permission:** Local network access is requested through Apple's native system authorization prompt (`NSLocalNetworkUsageDescription`). No network data or packet traffic is ever transmitted outside your local area network.

---

## Local Storage

- The App stores your receiver's local IP address, custom input labels, volume step preferences, and volume safety ceilings on-device using standard `UserDefaults` and secure Keychain storage (`KeychainStateBridge`).
- In accordance with Apple requirements, our system usage of `UserDefaults` is declared in the app bundle under Apple's reason code `CA92.1` for user preference persistence. No personal information or tracking identifiers are stored.

---

## Children's Privacy

The App does not collect any data from anyone, regardless of age. It is rated **4+** (Made for Everyone).

---

## Changes to This Policy

If this policy ever changes, updates will be published at this same URL with a revised effective date. Because the App operates with zero data collection, any future changes can only maintain or narrow this scope.

---

## Contact & Questions

If you have questions about this Privacy Policy or AmpliWidgets, you may open an issue at:
<https://github.com/amolkarnik/ampli-widgets/issues>
