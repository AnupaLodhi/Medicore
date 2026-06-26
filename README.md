# 🏥 Medicore

### AI-Powered Early Health Risk Assessment Platform for Underserved Communities

[![Live Demo](https://img.shields.io/badge/Live_Demo-View_App-28a745?style=for-the-badge&logo=githubpages)](https://anupalodhi.github.io/Medicore/)
[![YUKTI Recognized](https://img.shields.io/badge/YUKTI-Submitted-0052cc?style=for-the-badge&logo=gov.uk)](https://yukti.mic.gov.in/)
[![TRL Level](https://img.shields.io/badge/TRL-4_(_Lab_Validated_)-ff69b4?style=for-the-badge)](https://en.wikipedia.org/wiki/Technology_readiness_level)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge)](https://opensource.org/licenses/MIT)

---

## 📌 Overview

**Medicore** is a lightweight, AI-driven web platform that enables early screening for chronic diseases using basic clinical parameters. Designed for **rural and semi-urban India**, it bridges the healthcare gap by providing instant, explainable risk assessments without requiring specialized hardware or high-speed internet.

> 🎯 **Mission:** Make preventive healthcare accessible to the 60% of Indians who lack regular access to diagnostic facilities.

---

## 🔥 Why Medicore?

| Problem | Our Solution |
|---------|--------------|
| India has only **1 doctor per 1,400 people** (WHO recommends 1:1,000) | AI-assisted pre-screening reduces dependency on specialists |
| Diagnostic tests are expensive & centralized in cities | Zero-cost, smartphone-compatible risk assessment |
| Chronic diseases detected late → higher mortality | Early warning system flags high-risk cases proactively |
| Healthcare data is fragmented | Longitudinal tracking & printable health summaries |

---

## ✨ Key Features

- 🧠 **Multi-Disease Risk Matrix** – Assesses risk for diabetes, hypertension, cardiac conditions, and more using ML classification
- 📱 **Mobile-First Design** – Optimized for low-bandwidth networks and basic smartphones
- 🌐 **Offline-Ready (PWA)** – Works even with intermittent connectivity
- 📊 **Explainable AI** – Transparent risk scoring with interpretable outputs (not a black box)
- 🏥 **Frontline Health Worker Ready** – Simple UI designed for ASHA/ANM workers
- 📄 **Printable Reports** – Generate shareable patient summaries for teleconsultation
- 🔄 **Longitudinal Tracking** – Monitor health metrics over time

---

## 🛠️ Tech Stack

| Layer | Technology |
|-------|------------|
| **Frontend** | HTML5, CSS3, JavaScript (Vanilla) |
| **Hosting** | GitHub Pages |
| **ML Backend** | Python, scikit-learn, Pandas, NumPy |
| **Model Type** | Ensemble Classification (Random Forest + Logistic Regression) |
| **API Layer** | Flask (planned for full deployment) |
| **PWA Support** | Service Worker + Manifest.json |

---

## 🚀 Live Demo

👉 **[Click here to try Medicore](https://anupalodhi.github.io/Medicore/)**

*No installation required – works directly in your browser!*

---

## 📊 How It Works

---

## 🧪 Current Status (TRL 4)

- ✅ **Prototype developed** and hosted on GitHub Pages
- ✅ **ML models trained** on publicly available health datasets (PIMA Diabetes, Heart Disease UCI)
- ✅ **Initial validation** with synthetic test cases
- 🔄 **Pilot testing** underway with ~20 users from college health center
- 📝 **YUKTI 2026 Submission** – Ministry of Education, Government of India

---

## 🗺️ Roadmap

| Phase | Milestone | Timeline |
|-------|-----------|----------|
| ✅ Phase 1 | Core ML models + Web MVP | Completed |
| 🔄 Phase 2 | Multilingual UI (Hindi, Tamil, Telugu) | Q3 2026 |
| 📅 Phase 3 | Integration with Ayushman Bharat API | Q4 2026 |
| 📅 Phase 4 | Mobile App (Flutter) | Q1 2027 |
| 📅 Phase 5 | Pilot with 5 Primary Health Centers | Q2 2027 |

---

## 📁 Project Structure
Medicore/
├── index.html # Main landing page
├── css/
│ └── style.css # Responsive styles
├── js/
│ ├── app.js # Core logic & form handling
│ └── riskEngine.js # ML inference (simulated or API call)
├── assets/
│ ├── screenshots/ # UI screenshots
│ └── icons/ # Favicon & PWA icons
├── manifest.json # PWA configuration
├── service-worker.js # Offline support
└── README.md # This file

---

## 👥 Team

| Role | Name |
|------|------|
| **Lead Developer & AI Engineer** | [Your Name] |
| **Domain Expert (Healthcare)** | [Mentor/Professor Name] |
| **UI/UX Designer** | [Your Name / Team Member] |

> 📌 *Currently a solo project – open to collaborators!*

---

## 🤝 Contributing

We welcome contributions! Here's how you can help:

1. 🍴 Fork the repository
2. 🌿 Create a feature branch (`git checkout -b feature/amazing-feature`)
3. 💾 Commit your changes (`git commit -m 'Add some amazing feature'`)
4. 📤 Push to the branch (`git push origin feature/amazing-feature`)
5. 🔁 Open a Pull Request

**Areas where we need help:**
- ML model improvement (larger dataset, better accuracy)
- Multilingual translation
- UI/UX enhancements
- Integration with government health APIs

---

## 📄 License

Distributed under the **MIT License**. See `LICENSE` for more information.

---

## 🙏 Acknowledgments

- **Ministry of Education, India** – YUKTI Initiative
- **UCI Machine Learning Repository** – Public health datasets
- **GitHub Pages** – Free hosting for the prototype
- **Open-source community** – For all the tools that made this possible

---

## 📬 Contact

- **Project Lead:** [Your Name]
- **Email:** [your.email@example.com]
- **GitHub:** [@anupalodhi](https://github.com/anupalodhi)
- **LinkedIn:** [Your Profile]

---

### ⭐ If you find this project useful, please consider giving it a star on GitHub!
