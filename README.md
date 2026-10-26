<div align="center">

<img src="assets/images/logo/logo.png" alt="Journeo Logo" width="100" height="100" />

# Journeo

### **Private, Offline-First Mood Journaling for Android**

[![Flutter](https://img.shields.io/badge/Flutter-3.x-02569B?logo=flutter)](https://flutter.dev)
[![Dart](https://img.shields.io/badge/Dart-3.x-0175C2?logo=dart)](https://dart.dev)
[![Platform](https://img.shields.io/badge/Platform-Android-3DDC84?logo=android)](https://play.google.com/store)
[![License](https://img.shields.io/badge/License-Proprietary-red)](LICENSE)

**Your thoughts stay yours — always on-device. No cloud. No tracking.**

</div>

---

## 🧠 Overview

Journeo is a **privacy-first mood journaling app** designed for users who want complete control over their data.

* No accounts
* No syncing
* No servers

Everything is stored **locally on your device**, ensuring speed, reliability, and true privacy.

---

## ✨ Features

### 🆓 Free Tier

* 📝 Daily journaling (title, content, mood score)
* 😊 Mood tagging (up to 3 tags)
* 📅 Mood calendar heatmap
* 📊 7-day mood chart
* 🔥 Streak tracking
* 📱 Home screen widgets
* 🔐 App lock (biometric)
* ⏰ Reminders
* 📡 Fully offline

---

### 💎 Pro Tier

| Feature           | Description                        |
| ----------------- | ---------------------------------- |
| 📄 PDF Export     | Export journal as a shareable file |
| 📈 Analytics      | 30/90-day trends, yearly stats     |
| ☁️ Word Cloud     | Most-used words                    |
| 🎨 Themes         | Custom fonts & UI                  |
| 🏷 Unlimited Tags | No limits                          |
| 🏆 Milestones     | Track progress                     |

---

## 📄 PDF Export

Export flow:

```
Journal Data → PDF Builder → Uint8List → File → Share / Save / Print
```

* Default: **Share file**
* Optional: Print using `printing`

---

## 🏗 Tech Stack

| Layer        | Tech               |
| ------------ | ------------------ |
| Framework    | Flutter            |
| Language     | Dart               |
| Architecture | Clean Architecture |
| State        | Bloc               |
| Storage      | Hive / Isar        |
| DI           | get_it             |
| FP           | fpdart             |
| Monetization | RevenueCat         |

---

## 🧱 Architecture

```
features/
 ├── journal/
 ├── profile/
 ├── subscription/
 ├── notifications/
 └── analytics/
```

### Principles

* Local-first (no backend)
* Domain layer is pure Dart
* Uses `Either<Failure, T>`
* No SDK leakage into domain

---

## ⚙️ Setup

### Clone

```bash
git clone <repo>
cd journeo
```

### Install

```bash
flutter pub get
```

### Run

```bash
flutter run
```

---

## 🔑 Environment

```bash
flutter run \
--dart-define=REVENUE_CAT_API_KEY=your_key
```

---

## 📦 Build

```bash
flutter build appbundle --release \
--dart-define=REVENUE_CAT_API_KEY=your_key
```

---

## 🎯 Philosophy

* Privacy-first
* Offline-first
* User-owned data

---

## 🚧 Roadmap

* [ ] Deep analytics
* [ ] Word cloud
* [ ] Theme system
* [ ] Export improvements
* [ ] Backup system

---

## 🤝 Contributing

Private repository. Access by invitation.

---

<div align="center">

Built with Flutter · Designed for privacy · Made in India

</div>
