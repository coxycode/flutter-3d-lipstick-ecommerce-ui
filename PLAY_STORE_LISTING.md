# 📱 Rouvelle™ — Google Play Store Listing & Publishing Kit

This document provides all verified metadata, descriptions, graphics specifications, AI generation prompts, and publishing instructions required to publish **Rouvelle** to the **Google Play Console**.

---

## 🏷️ 1. Store Listing Core Metadata

| Field | Limit | Rouvelle Listing Content |
| :--- | :--- | :--- |
| **App Title** | Max 30 chars | `Rouvelle: Luxury Rouge Checkout` |
| **Alternative Title** | Max 30 chars | `Rouvelle — Haute Couture Film` |
| **Package Name** | Format | `com.rouvelle.app` |
| **Primary Category** | — | `Beauty` / `Shopping` |
| **Secondary Category**| — | `Lifestyle` |
| **Content Rating** | — | `Everyone (PEGI 3 / ESRB Everyone)` |
| **Target Audience** | — | `Ages 13+` |
| **Contains Ads** | — | `No` |
| **In-App Purchases** | — | `No (Demo / Free)` |

---

## 📝 2. Short Description (Google Play Store)

> **Limit:** Up to 80 characters.

### Primary (Recommended — 73 characters):
```text
Cinematic 240-frame bloom haute couture app with one-tap luxury checkout.
```

### Alternative A (76 characters):
```text
Experience 240-frame fashion cinematography and one-tap luxury satin rouge.
```

### Alternative B (70 characters):
```text
Haute couture cinema meets effortless one-tap checkout. Wear your red.
```

---

## 📄 3. Full / Long Description (Google Play Store)

> **Limit:** Up to 4,000 characters.

```text
🌹 Welcome to Rouvelle™ — Where Cinematic Haute Couture Meets One-Tap Commerce.

Step into an artistic beauty film experience designed for pure elegance and fluid motion. Rouvelle transforms digital shopping from a cluttered catalog into a hypnotic fashion film, leading into an effortless one-tap checkout for the iconic Velours No. 07 deep red satin lipstick.

✨ THE ROUVELLE EXPERIENCE:

🎬 240-FRAME BLOOM CINEMATOGRAPHY
Witness a seamless 24fps visual transition where a crimson botanical tulip unfurls petal by petal, distilling into pure red pigment and forming the sculptural Velours No. 07 lipstick. Optimized with rolling lookahead decoding for zero frame drops.

⚡ ONE-TAP FRICTIONLESS CHECKOUT
Say goodbye to tedious billing forms, captchas, and multi-step carts. Pick your preferred saved payment method (UPI, Card, or Cash on delivery), feel the tactile haptic confirmation, and complete your reservation in one tap.

💄 VELOURS NO. 07 SATIN ROUGE
A signature deep-red luxury lipstick with high-pigment saturation, velvety hydration, and a feather-light satin finish designed to empower every complexion.

💎 MINIMALIST ARCHITECTURE (PURE FLUTTER)
Crafted entirely using core Flutter primitives with zero external packages. Pure, lightweight 60fps performance across modern mobile displays with deep dark-mode luxury aesthetics.

🔄 REPLAY OR SKIP FREELY
Watch the cinematic poetry as many times as you like, or tap anywhere to skip straight to the checkout suite.

⚖️ OPEN SOURCE TEMPLATE & DISCLAIMER NOTICE:
This application is provided as an open-source demonstration and luxury e-commerce UI template. Anyone is free to explore, fork, adapt, or contribute to this software.

LIMITATION OF LIABILITY & DISCLAIMER:
THE APPLICATION IS PROVIDED "AS IS" WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED. IN NO EVENT SHALL THE AUTHORS, CREATORS, OR CONTRIBUTORS BE LIABLE FOR ANY CLAIMS, DAMAGES, FINANCIAL LOSS, SIMULATED OR REAL TRANSACTIONS, OR LIABILITIES ARISING FROM THE USE, MODIFICATION, OR THIRD-PARTY DEPLOYMENT OF THIS SOFTWARE. USE AND MODIFICATION ARE STRICTLY AT YOUR OWN RISK.

Download Rouvelle™ and experience luxury commerce in motion. 🌹
```

---

## 🎨 4. Store Graphics Assets & Specs

| Asset | Size | Format | Status in Repository |
| :--- | :--- | :--- | :--- |
| **App Icon** | 512 x 512 px | PNG (no alpha, 32-bit) | ✅ `assets/store/app_icon_512.png` |
| **Feature Graphic** | 1024 x 500 px | PNG / JPEG (max 15MB) | ✅ `assets/store/feature_graphic.png` |
| **Master Icon** | 1024 x 1024 px | PNG | ✅ `assets/icon/app_icon.png` |
| **Android Launcher Icons** | 48, 72, 96, 144, 192 px | PNG | ✅ `android/app/src/main/res/mipmap-*/` |
| **Web Icons & Favicon** | 64, 192, 512 px | PNG | ✅ `web/icons/`, `web/favicon.png` |

---

## 🤖 5. AI Image Generation Prompts (Midjourney, DALL-E, Imagen)

Use these engineered prompts whenever you want to generate seasonal campaigns or graphic variants:

### 🌟 Prompt 1: Feature Graphic (1024 x 500)
```text
Google Play Store feature graphic banner for 'Rouvelle', a luxury haute couture cosmetic and lipstick mobile app. Ultra-wide dark cinematic shot featuring an exquisite dark-red tulip in full bloom merging into a sculptural gold-and-black tube of deep rouge satin lipstick with crimson silk ribbons, golden champagne typography reading 'ROUVELLE - Haute Couture Film & One-Tap Checkout', obsidian background with deep red spotlight, hyper-realistic, 8k commercial photography, 16:9 ratio.
```

### 💄 Prompt 2: App Icon (512 x 512)
```text
A luxury mobile app icon for 'Rouvelle'. A glossy, sculptural deep-red satin lipstick tip with subtle gold flakes and a delicate red tulip petal reflection, set inside an obsidian black squircle with a fine champagne gold trim, minimalist haute couture French perfumery aesthetic, raytraced studio lighting, centered, 1:1 ratio.
```

### 📱 Prompt 3: Screenshot 1 — 240-Frame Cinematography Mockup
```text
Smartphone UI mockup showing the Rouvelle intro screen. Dark aesthetic with high-fashion photography of a blooming deep red flower, delicate gold serif brand text 'ROUVELLE' at the top, headline 'Wear your own red', minimal champagne progress line, and subtle 'TAP TO SKIP' text at bottom.
```

### 💳 Prompt 4: Screenshot 2 — One-Tap Checkout Mockup
```text
Modern smartphone mockup showcasing the Rouvelle one-tap checkout screen. Clean obsidian dark theme with a product card showing 'Velours No. 07 Deep Red Satin Lipstick' at ₹1499, sleek payment radio tiles for UPI and Card, and a vibrant crimson 'PAY ₹1499' rounded button.
```

### 🎉 Prompt 5: Screenshot 3 — Payment Success Voucher Mockup
```text
Smartphone app screenshot showing the payment success screen of Rouvelle. Center features an elastic gradient crimson checkmark circle, elegant typography reading 'Payment successful', order confirmation message, and a stylish champagne outlined 'REPLAY INTRO' button.
```

---

## 🚀 6. Step-by-Step Play Store Release Guide

### Step 1: Set Android Application ID & Version
In `android/app/build.gradle`:
```gradle
defaultConfig {
    applicationId "com.rouvelle.app"
    minSdkVersion 21
    targetSdkVersion 34
    versionCode 1
    versionName "1.0.0"
}
```

### Step 2: Build Production Android App Bundle (.aab)
Run in terminal:
```bash
flutter build appbundle --release
```
The output file is generated at:
`build/app/outputs/bundle/release/app-release.aab`

### Step 3: Google Play Console Submission
1. Log into [Google Play Console](https://play.google.com/console).
2. Click **Create app** -> Enter App name `Rouvelle: Luxury Rouge Checkout`.
3. Set Language to English, App type to **App**, Free.
4. Navigate to **Store presence** -> **Main store listing**:
   - Paste **Short Description** from Section 2.
   - Paste **Full Description** from Section 3.
   - Upload `assets/store/app_icon_512.png` as **App Icon**.
   - Upload `assets/store/feature_graphic.png` as **Feature Graphic**.
   - Upload at least 4 screenshots.
5. Complete **App content** declarations (Privacy policy, Target audience 13+, Data safety).
6. Go to **Production** -> **Create new release** -> Upload `app-release.aab`.
7. Review release and submit for Google review!
