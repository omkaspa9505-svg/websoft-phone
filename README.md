# Websoft Phone

A professional, browser-based softphone client built for high-performance telecommunications and seamless agent workflows. Engineered using modern web standards, this application connects directly with the Twilio Voice SDK, facilitating bidirectional voice communication natively within the browser and completely eliminating the need for hardphones.

## 🚀 Key Features

* **WebRTC Built-in**: Full native integration with Twilio Voice SDK for crystal-clear browser-based communication.
* **Dual-Line Management**: Intuitive interface for dynamic switching between caller ID representation and line statuses.
* **Rich Call Controls**: Interactive dialpad, mute, hold, transfer, and end-call states built strictly for rapid agent interactions.
* **Comprehensive Activity Log**: Maintains real-time tracking of outbound events and system network hooks.
* **Call History & Recordings**: Integrated side-drawers tracking localized call histories, durations, timestamps, and one-click playback/download of recorded sessions.
* **SMS Messaging Portal**: Threaded, persistent SMS chat views baked directly into the phone interface with localized contact searching.
* **Intelligent UI Design**: Minimalist and deeply integrated aesthetic adhering strictly to `dark-mode` spatial and ergonomic design languages.

## 🛠️ Technology Stack

* **Frontend**: Native HTML5, CSS3 (Modern Variablized CSS), Vanilla JavaScript (ES6+).
* **Telecom Provider**: Twilio Voice SDK (`twilio.min.js`).
* **Design Paradigm**: No-build, dependency-free spatial glassmorphism and modern gradient overlays via custom CSS properties.

## 🏗️ Architecture & Concepts

This project showcases several advanced engineering concepts:

1. **State Machine UI**: The core DOM dynamically repaints relying on `data-state` mapping to prevent race conditions during high-speed calling environments.
2. **Web Audio Contexts**: Safely scopes and manages real-time streaming media across diverse micro-components.
3. **Modular CSS**: Component-isolated stylesheets ensuring zero-bleed and easily extensible dark/light themes.

## ⚙️ Running Locally

1. Clone this repository.
2. Host the folder via a local server (e.g., `python -m http.server 8000` or `npx serve`).
3. Navigate to `http://localhost:8000/login.html`.
4. *(Note: Complete operational capabilities require a connected Twilio backend server to authorize WebRTC tokens).*

## 🔒 Security

* Secure authentication boundary (`login.html`) ensuring only authenticated tokens hit the WebRTC initialization flow.
* Stateless DOM interactions that never store access tokens inside accessible components.

---
> *This repository highlights proficiency in orchestrating deeply integrated third-party SDKs within completely native, highly accessible browser environments.*
