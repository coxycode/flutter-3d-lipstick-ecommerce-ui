# 🌹 Rouvelle™ — Cinematic Haute Couture & One-Tap Checkout

<div align="center">

[![Flutter](https://img.shields.io/badge/Flutter-3.44+-02569B?logo=flutter&logoColor=white)](https://flutter.dev)
[![Dart](https://img.shields.io/badge/Dart-3.12+-0175C2?logo=dart&logoColor=white)](https://dart.dev)
[![Platforms](https://img.shields.io/badge/Platforms-Android%20%7C%20iOS%20%7C%20Web%20%7C%20Desktop-4CAF50)](#-supported-platforms)
[![License: MIT](https://img.shields.io/badge/License-MIT-purple.svg)](LICENSE)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)
[![Design](https://img.shields.io/badge/Aesthetics-Haute%20Couture%20Rouge-B3122D)](https://flutter.dev)

**A high-fashion luxury commerce experience built with pure Flutter.**  
*240-frame bloom cinematography • Instant one-tap checkout • Zero third-party dependencies.*

[**Live Visual Showcase**](#-cinematic-visual-showcase) • [**App Flow**](#-architecture--user-flow) • [**Quickstart**](#-getting-started) • [**Contribute**](CONTRIBUTING.md) • [**Play Store Kit**](PLAY_STORE_LISTING.md) • [**Legal Disclaimer**](#️-legal-disclaimer--limitation-of-liability)

<br/>

<img src="./assets/store/feature_graphic.png" alt="Rouvelle Feature Graphic" width="100%" style="border-radius: 12px; margin-top: 10px;" />

<br/>

<img src="./assets/store/app_icon_512.png" alt="Rouvelle App Icon" width="120" height="120" style="border-radius: 24px; box-shadow: 0 8px 24px rgba(179,18,45,0.35);" />

</div>

---

## 🌟 Cinematic Visual Showcase: From Bloom to Rouge

Rouvelle delivers a fashion-film intro directly inside a mobile interface. 240 high-resolution photographic frames seamlessly decode in real-time at 24fps, taking the viewer through a botanical red tulip awakening into the **Velours No. 07** satin lipstick.

### 🎬 The 240-Frame Transformation Sequence

| Act 1: Tulip in Bloom | Act 2: Petal Awakening | Act 3: Composition |
| :---: | :---: | :---: |
| ![Frame 030](./assets/bloom_frames/frame_030.jpg) | ![Frame 070](./assets/bloom_frames/frame_070.jpg) | ![Frame 105](./assets/bloom_frames/frame_105.jpg) |
| *Frame 030 — "Begin in bloom"* | *Frame 070 — Petals unfurl* | *Frame 105 — Pigment extraction* |

| Act 4: Velours No. 07 | Act 5: Satin Texture | Act 6: Haute Portrait |
| :---: | :---: | :---: |
| ![Frame 130](./assets/bloom_frames/frame_130.jpg) | ![Frame 180](./assets/bloom_frames/frame_180.jpg) | ![Frame 240](./assets/bloom_frames/frame_240.jpg) |
| *Frame 130 — "Colour, composed"* | *Frame 180 — Rich satin rouge* | *Frame 240 — "Wear your own red"* |

---

## ✨ Key Architectural Highlights

### 🎞️ 24fps Rolling Pre-Cache Engine
- **Pre-Cache Optimization**: Preloads an initial buffer of 36 frames before triggering playback, then maintains a rolling 36-frame lookahead window so decoding never drops frames.
- **Enlarged Memory Budget**: Automatically allocates a 400MB image cache budget (`maximumSizeBytes = 400 << 20`) for buttery 60fps rendering without memory thrashing.
- **Responsive Skip Gesture**: Instant tap-anywhere and dedicated top-right **Skip** action with smooth 700ms cross-fade transition.

### 🛍️ Minimalist One-Tap Checkout
- **Zero Friction**: No lengthy text fields or forms. Pick a saved payment method (UPI, Card, Cash on delivery) and press **Pay**.
- **Tactile Haptic Feedback**: Integrated medium haptics on payment initiation.
- **Seamless State Animation**: Simulated checkout state with loading indicator transitioning into an elastic spring checkmark voucher.

### ⚡ Pure Flutter (Zero External Packages)
- Built entirely with core Flutter SDK primitives (`Image.asset`, `GestureDetector`, `Timer`, `PageRouteBuilder`, `SystemChrome`).
- Extremely lightweight repository, ultra-fast compile times, and complete multi-platform stability.

---

## 🚀 Getting Started

### Prerequisites
- [Flutter SDK](https://flutter.dev) (v3.3.0 or higher)
- Android Studio / Xcode / Chrome

### Run the App
```bash
# 1. Fetch dependencies
flutter pub get

# 2. Run on Web
flutter run -d chrome

# 3. Run on Android or iOS
flutter run
```

---

## 🤝 Open Source & Contributing

We love open-source contributions! Whether you want to add:
- Real payment gateway adapters (Stripe, Razorpay, Apple Pay, Google Pay)
- Multi-product carousel selectors
- Audio soundtrack synchronization with the 240 frames
- 3D interactive bottle/lipstick inspect shaders

Please see our [CONTRIBUTING.md](CONTRIBUTING.md) guide for how to fork, develop, and submit pull requests.

---

## 📱 Google Play Store Kit

Ready to publish Rouvelle to the Google Play Console? Check out [PLAY_STORE_LISTING.md](PLAY_STORE_LISTING.md) for:
- Verified App Title (<30 chars) and Short Description (<80 chars)
- Rich Long Description (<4000 chars)
- AI Prompts for seasonal Feature Graphics and App Icons
- Bundle build command: `flutter build appbundle --release`

---

## ⚖️ Legal Disclaimer & Limitation of Liability

> [!IMPORTANT]  
> **Open Template & Modification Terms:**  
> Anyone is free to use, copy, modify, distribute, or adapt this project, its code, and its assets for personal, educational, or commercial projects.

> [!WARNING]  
> **No Responsibility / Disclaimer of Liability:**  
> THIS SOFTWARE IS PROVIDED **"AS IS"**, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE, AND NONINFRINGEMENT.  
> **IN NO EVENT SHALL THE ORIGINAL AUTHORS, CREATORS, OR CONTRIBUTORS BE LIABLE FOR ANY CLAIM, DAMAGES, FINANCIAL LOSS, MOCK OR REAL PAYMENTS, TRANSACTIONS, OR OTHER LIABILITIES ARISING FROM THE USE, MODIFICATION, OR DEPLOYMENT OF THIS SOFTWARE.**  
> Anyone who modifies, forks, rebrands, or deploys this software does so entirely at their own discretion, risk, and legal responsibility.

---

<div align="center">
Crafted with passion for cinema, couture, and clean Flutter engineering. 🌹
</div>
