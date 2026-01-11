# Ticker Scanner 🏛️

**Ticker Scanner** is an institutional-grade stock market analysis tool developed for Android. It leverages real-time price action logic and proprietary volatility algorithms to identify high-probability trading setups across US and European markets.
``
<img width="996" height="2048" alt="image" src="https://github.com/user-attachments/assets/c089bf74-345c-4e01-a0af-a14b881bb4ee" />

## ⚡ Core Technologies

*   **Logic**: Proprietary algorithms for "Smart Momentum" (breakout detection) and "Missile" (volatility spikes).
*   **Architecture**: MVVM with Jetpack Compose.
*   **Performance**: Coroutine-based concurrent scanning for multi-region support.
*   **UI/UX**: Institutional "Terminal" aesthetic with custom vector cartography for region navigation.
*   **Persistence**: Room Database for offline result caching and detailed history tracking.

## 🚀 Key Features

*   **Multi-Region Scanning**: Independent state management for USA (s&p 500/Nasdaq) and Europe. Scan both markets simultaneously without data loss.
*   **Institutional Signals**:
    *   **Smart Momentum**: Detects pure price accumulation before the breakout.
    *   **Missile**: Identifies explosive volatility expansion.
    *   **Early Movers**: Catches trends at inception.
*   **Visual Precision**: 
    *   "NBA-Style" High-Contrast Palette (Slate Blue / Red / White).
    *   Custom vector-drawn maps for crisp navigation at any DPI.
*   **Intelligent Caching**: Prevents redundant scanning by checking daily cache validity.

## 🛠️ Build & Installation

1.  Clone the repository.
2.  Open in Android Studio Ladybug or newer.
3.  Sync Gradle (Kotlin DSL).
4.  Run on Emulator or Physical Device.

```bash
./gradlew assembleDebug
```

## 📜 License

Copyright © DoctorDiaz. All Rights Reserved.
Proprietary trading logic and code structure.
