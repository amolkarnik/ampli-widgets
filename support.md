---
title: Support — AmpliWidgets
---

# Support & FAQ

AmpliWidgets is an independent application. For questions, feature requests, or bug reports, please refer to the guidance below.

---

## Reporting a Bug or Requesting a Feature

To report an issue or request support, please open a ticket on our public issue tracker:
👉 **[Open an Issue on GitHub](https://github.com/amolkarnik/ampli-widgets/issues)**

When submitting a bug report, please include:
- **Device Model & iOS Version** (e.g. iPhone 16 Pro / iPhone 17 Pro, iOS 18 / iOS 27)
- **AV Receiver Model** (e.g. Marantz Cinema 60, Denon AVR-X2800H)
- **App Version** (found at the bottom of the Settings tab)
- **Steps to reproduce** the issue
- **Observed behavior vs. expected behavior**

---

## Frequently Asked Questions (FAQ)

### How do I connect AmpliWidgets to my AV receiver?
AmpliWidgets uses Bonjour / mDNS network discovery to find your receiver automatically on first launch. Ensure your iPhone is connected to the same Wi-Fi network as your receiver. If your network configuration prevents automatic mDNS discovery:
1. Open the **Settings** tab in the app.
2. Enter your receiver's local IP address manually (e.g., `192.168.1.50`).
3. Tap **Test Connection** or **Save Settings**.

### Why does the app request "Local Network" permission?
AmpliWidgets sends standard ASCII control commands directly to your AV receiver over TCP port 23 and uses Bonjour to discover your receiver on your home Wi-Fi network. iOS requires explicit user authorization (`NSLocalNetworkUsageDescription`) for any app that communicates with devices on your local Wi-Fi. AmpliWidgets never sends any data outside your local network.

### How does the Volume Safety Ceiling work?
The Safety Volume Ceiling allows you to set a hard maximum volume limit (e.g., `-15.0 dB`). Any volume step up command—whether from the app, Home Screen widget, or Control Center—will automatically clamp at this ceiling and refuse to step higher, protecting your ears, family, and speakers from accidental volume jumps.

### How do I change between widget styles?
AmpliWidgets provides 4 distinct interactive widget layouts:
- **AmpliWidgets Hub:** Polarized dual-zone console with a 1-tap Small Widget View Mode switcher between master volume and the 4-input launcher.
- **Porthole Luxe:** Classic circular porthole dial with champagne gold styling.
- **Direct Studio Deck:** Professional mixing console layout with dedicated vertical volume steppers.
- **Ultra-Minimal Pill:** Compact HomeKit-style capsule.

To add or change widgets:
1. Long-press on your iPhone Home Screen until the apps jiggle.
2. Tap the **"+" (plus)** button in the top corner.
3. Search for **AmpliWidgets** and swipe through the available widget sizes and styles.
4. Tap **Add Widget**.

### How do I reset or start from scratch?
If you change your home router, get a new receiver, or want to return the app to initial discovery mode:
1. Open the **Settings** tab.
2. Scroll to the bottom and tap **Reset & Start From Scratch**.
3. Confirm the dialog. All local IP configuration, custom input labels, and cached states will be cleanly wiped from on-device storage and Keychain.

### Does AmpliWidgets collect or transmit any personal data?
**No.** AmpliWidgets operates 100% on-device. There are zero accounts, zero analytics, zero trackers, and zero external servers. All network traffic is strictly between your phone and your receiver on your private local network.

---

## Direct Inquiries

For other inquiries, please contact:
<https://github.com/amolkarnik/ampli-widgets/issues>
