# 📱 Fidelity Corp (B2B Android Merchant App)

[![Platform](https://img.shields.io/badge/Platform-Android%20%28Native%29-3DDC84.svg?style=for-the-badge&logo=android&logoColor=white)](https://developer.android.com/)
[![Java](https://img.shields.io/badge/Java-8%2B-ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white)](https://www.java.com/)
[![Gradle](https://img.shields.io/badge/Gradle-Build-02569B.svg?style=for-the-badge&logo=gradle&logoColor=white)](https://gradle.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge)](https://opensource.org/licenses/MIT)

The corporate management app for the **Fidelity Ecosystem**—a shared loyalty points network designed for small business networks. Written in native Java, this application enables partner businesses (e.g., retail stores, restaurants) to validate transactions, issue loyalty points, and execute customer redemptions in real time.

---

## 🧩 System Architecture & Ecosystem

The overall multi-tier system coordinates across consumer, merchant, and central server components:

| Component | Repository | Tech Stack | Audience & Function |
| :--- | :--- | :--- | :--- |
| **B2B Merchant App** | **This Repo** | Native Java, Android | Merchant mobile app for store staff to process points & redemptions |
| **Full-Stack Core** | [Fidelity-Web-Server](https://github.com/Sadoklaoo/Fidelity-Web-Server) | Node.js, Express, MySQL | Core REST API server & web administrative dashboard |
| **B2C Mobile App** | [Fidelity-App](https://github.com/Sadoklaoo/Fidelity-App) | Flutter, Dart | Consumer mobile app for end-users to collect & track points |

---

## ✨ Features

* **🔐 Corporate Authentication:** Secure login for authorized partner business staff and store managers.
* **💳 Point Issuance & Redemption:** Real-time processing of points awarded or spent during purchases.
* **📜 Transaction History:** Local logging and sync history for store-level operational transparency.
* **🔄 REST API Synchronization:** Asynchronous API connectivity to handle data validation against the central database.
* **⚡ Offline Support:** Basic local caching to queue and sync transactions upon connection re-establishment.

---

## 📂 Project Structure

```text
Fidelity-Corp/
├── app/                  # Android application module (UI activities, network logic, layouts)
├── gradle/               # Gradle wrapper executable binaries
├── build.gradle          # Project-level build configurations
├── settings.gradle       # Module dependencies and project definitions
├── gradle.properties     # Environment execution configurations
└── README.md             # Documentation
```

---

## 🚀 Getting Started

### Prerequisites
* [Android Studio](https://developer.android.com/studio) (latest stable release)
* **JDK 8+**
* Android Physical Device or Emulator (`API Level 21+`)

### Setup

```bash
# Clone the repository
git clone https://github.com/Sadoklaoo/Fidelity-Corp.git
cd Fidelity-Corp
```

1. Open **Android Studio**.
2. Select **Open an Existing Project** and navigate to the cloned `Fidelity-Corp` folder.
3. Allow Gradle to sync and build project dependencies automatically.

### Environment Setup

If connecting to your custom API environment:
* Define your backend URL and client authorization parameters inside your configuration file (e.g., `config.properties` or `gradle.properties`):

```properties
API_BASE_URL=https://your-backend-domain.com/api
CLIENT_ID=your_merchant_client_id
CLIENT_SECRET=your_merchant_client_secret
```

### Running the App

1. Connect your target physical Android device (with **USB Debugging** enabled) or start an AVD emulator.
2. Select the `app` configuration in Android Studio.
3. Click the **Run** button (`Shift + F10`) to compile and deploy.

---

## 🤝 Contributing

Contributions are welcome! Feel free to open an issue or submit a Pull Request.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 👤 Author

* **Sadok Laouissi** — [GitHub](https://github.com/Sadoklaoo) | [LinkedIn](https://www.linkedin.com/in/sadok-laouissi/) | `sadok.laouissi.sl@gmail.com`

---

## 📜 License

Distributed under the MIT License. See `LICENSE` for more information.
