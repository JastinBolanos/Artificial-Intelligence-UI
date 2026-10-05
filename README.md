<div align="center">
  <img src="docs/lopsai.png" alt="LopsAI Logo" width="100" />

  <h1>LopsAI-KMP</h1>
  <p><strong>Native AI Conversational Client built with Compose Multiplatform</strong></p>

[![Kotlin](https://img.shields.io/badge/Kotlin-7F52FF?style=flat-square&logo=kotlin&logoColor=white)](https://kotlinlang.org/)
[![Compose Multiplatform](https://img.shields.io/badge/Compose_Multiplatform-purple?style=flat-square&logo=android)](https://www.jetbrains.com/lp/compose-multiplatform/)
[![iOS & Android](https://img.shields.io/badge/Platform-Android%20%7C%20iOS-black?style=flat-square&logo=apple)]()
[![Clean Architecture](https://img.shields.io/badge/Architecture-Clean%20%2B%20UDF-orange?style=flat-square)]()

<p align="center">
  <a href="https://github.com/JastinBolanos/LopsAI-KMP/releases/download/v1.0.0/lopsai.apk">
    <img src="https://img.shields.io/badge/Download-APK%20Android-success?style=for-the-badge&logo=android&logoColor=white" alt="Descargar APK">
  </a>
</p>
</div>

---

## Overview

**LopsAI-KMP** is a frontend architecture showcase illustrating how complex conversational AI interfaces—featuring dynamic navigation trees, expandable inputs, and rich theming—can be implemented across mobile platforms using a single Kotlin codebase.

---

## App Preview

### 💬 Conversational Engine & Navigation
> Modal navigation, model selectors, and real-time message stream rendering.

| Dashboard (Dark) | Dashboard (Light) | Sidebar Menu |
| :---: | :---: | :---: |
| <img src="docs/01_dashboard_mobile.png" width="220" alt="Dashboard Dark"/> | <img src="docs/15_dashboard_mobile_light.png" width="220" alt="Dashboard Light"/> | <img src="docs/07_sidebar_navigation.png" width="220" alt="Sidebar"/> |

### 🛠️ OmniInput Tools & Interactivity
> Expandable input tray, custom prompt tools, and rich media rendering.

| Model Selector | OmniInput Tools | Rich Media Chat |
| :---: | :---: | :---: |
| <img src="docs/02_model_selection_dropdown.png" width="220" alt="Model Selector"/> | <img src="docs/14_input_tools_menu.png" width="220" alt="Tools Menu"/> | <img src="docs/18_chat_image_response.png" width="220" alt="Rich Media"/> |

### 🧩 Ecosystem (GPT Store & Library)
> Discovery catalogs, workspace libraries, and modal upgrades.

| My Library | GPT Store | Subscription Tiers |
| :---: | :---: | :---: |
| <img src="docs/06_library_gradients.png" width="220" alt="Library"/> | <img src="docs/04_gpt_store_featured.png" width="220" alt="GPT Store"/> | <img src="docs/08_premium_upgrade_modal.png" width="220" alt="Premium Tiers"/> |

---

## Technical Highlights

* **Framework:** Kotlin Multiplatform (KMP) & Compose Multiplatform targeting Native Android and iOS.
* **Architecture:** Clean Architecture + Unidirectional Data Flow (UDF).
* **State Management:** Employs explicit `key()` parameters in `LazyColumn` structures to maintain predictable scroll positions during continuous AI message streaming.
* **Ambient Theming:** Centralized Dark/Light theme management using `CompositionLocal`. Includes custom Canvas shaders (`LivingWallpaperBg`) for subtle ambient lighting effects.

---

## Routing & UI Architecture

* **Dashboard (Chat Module):** `OmniInput Container` ➔ `Tools Tray` ➔ `Message List` ➔ `Rich Media Render`
* **Discovery Module:** `Library Grid` ➔ `GPT Store (Trending/Featured)`
* **Global Modals:** `Search Chats` ➔ `Settings Panel` ➔ `Share Conversation`

---

## Getting Started

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/JastinBolanos/LopsAI-KMP.git](https://github.com/JastinBolanos/LopsAI-KMP.git)
   cd LopsAI-KMP
   ```
**For Android:**
- Open the project in Android Studio.
- Select the `androidApp` configuration.
- Press *Run*.
