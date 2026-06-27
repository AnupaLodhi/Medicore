<div align="center">

<img src="https://img.shields.io/badge/License-MIT-blue.svg" alt="MIT License">
<img src="https://img.shields.io/badge/Release-v1.0.0-green.svg" alt="v1.0.0">
<img src="https://img.shields.io/badge/Stack-React%20%7C%20Node.js%20%7C%20TypeScript-informational" alt="Stack">
<img src="https://img.shields.io/badge/Deployed-Vercel-black" alt="Vercel">

# MediBridge AI

**Connecting Doctors, Pharmacies, and Patients Through Intelligent Healthcare Communication**

[🌐 Live Demo](https://medi-bridge-ai-nu.vercel.app) &nbsp;·&nbsp; [📖 Docs](#installation) &nbsp;·&nbsp; [🐛 Report Bug](https://github.com/AnupaLodhi/medi-bridge-ai/issues) &nbsp;·&nbsp; [✨ Request Feature](https://github.com/AnupaLodhi/medi-bridge-ai/issues)

</div>

---

## What is MediBridge AI?

India faces a critical healthcare communication gap. Handwritten prescriptions are often illegible, over 60% of rural populations lack English fluency, and there is no unified digital channel connecting doctors, pharmacies, and patients. This leads to medication errors, dispensing delays, and poor health outcomes — especially for elderly and low-literacy populations.

**MediBridge AI** solves this with a single platform that:

- Lets doctors generate **QR-signed digital prescriptions** and send them directly to pharmacies
- Lets patients **upload or photograph prescriptions** and receive plain-language AI explanations in their own language
- Lets pharmacies **verify prescriptions by QR scan**, check drug interactions, and manage a live dispensing queue
- Provides **emergency medicine delivery** — when a patient can't reach a pharmacy, nearby pharmacies receive the order and a gig delivery person brings the medicine to their door

---

## Screenshots

| Home | Patient Portal |
|------|----------------|
| ![Home](https://private-user-images.githubusercontent.com/171830819/604434437-347d0a0d-eeba-46b3-8df9-4de2dd7e11f4.png) | ![Patient](https://private-user-images.githubusercontent.com/171830819/604434767-dc093c85-68c3-43dd-bf67-f2085d469b22.png) |

| Doctor Portal | Pharmacy Portal |
|---------------|-----------------|
| ![Doctor](https://private-user-images.githubusercontent.com/171830819/604434927-766eaf00-1a93-401b-9f73-4e3ba51e01ca.png) | ![Pharmacy](https://private-user-images.githubusercontent.com/171830819/604435090-b9f7c51c-5576-450f-8274-3ad0923f3ffa.png) |

---

## Features

### Patient Portal
- Upload prescriptions via **camera, gallery, or file** (JPG, PNG, PDF)
- AI-powered **plain-language explanation** of every medicine, dosage, and instruction
- View full **prescription history** with dispensing status
- **Medication reminders** — never miss a dose
- One-tap **emergency medicine delivery** when you can't reach a pharmacy

### Doctor Portal
- Create **structured digital prescriptions** with patient details and multiple medicines
- **QR code generation** — signed, verifiable, tamper-proof
- **Send to pharmacy** — packages prescription + patient notes + AI safety alerts in one click
- Upload **lab reports, X-rays, and patient documents** (camera, gallery, or file)
- Automatic **AI drug interaction check** before prescription is finalised

### Pharmacy Portal
- **Verify prescriptions** by scanning QR codes or uploading images — AI confirms authenticity instantly
- **Incoming queue** — receive prescriptions sent directly by doctors with full patient context
- **AI safety alerts** — flagged drug interactions and allergy warnings before dispensing
- **Generic medicine suggestions** — cheaper alternatives shown automatically
- **Emergency order queue** — real-time SOS orders from patients with 2-minute response window

### Emergency Medicine Delivery
- Patient uploads medicine image or prescription and shares location
- System **broadcasts to all nearby pharmacies** simultaneously (within 5 km radius)
- If first pharmacy declines → **automatically forwarded** to the next nearest
- Accepted pharmacy confirms stock → **gig delivery person assigned**
- Patient gets **live tracking** — packed → picked up → on the way → delivered
- If all nearby pharmacies decline → search **auto-expands to 10 km**

### AI & Accessibility
- **Multilingual voice assistant** — 10 Indian languages (Hindi, Tamil, Marathi, Bengali, Telugu, Kannada, Malayalam, Gujarati, Punjabi, Odia)
- **Accessibility mode** — large text, high contrast, voice-first navigation, simplified language
- **AI safety layer** — detects missing dosages, unclear handwriting, and dangerous drug combinations
- **HCI research documentation** — design principles and user research methodology included

---

## Tech Stack

| Layer | Technology |
|---|---|
| Frontend | React 18, TypeScript, TailwindCSS, React Router |
| Backend | Node.js, Express, TypeScript |
| AI | OCR (prescription reading), LLM-based parsing, Speech-to-Text, Text-to-Speech |
| Deployment | Vercel (frontend), Node.js server |

---

## Installation

### Prerequisites

- [Node.js](https://nodejs.org/) v18 or higher
- npm v9 or higher
- Git

### 1. Clone the repository

```bash
git clone https://github.com/AnupaLodhi/medi-bridge-ai.git
cd medi-bridge-ai
```

### 2. Install dependencies

```bash
# Root
npm install

# Frontend
cd client && npm install

# Backend
cd ../server && npm install
cd ..
```

### 3. Set up environment variables

```bash
cp server/.env.example server/.env
```

Open `server/.env` and fill in your API keys (AI provider, etc.).

### 4. Start development servers

```bash
npm run dev
```

| Service | URL |
|---|---|
| Frontend | http://localhost:5173 |
| Backend API | http://localhost:3001 |

To run individually:

```bash
npm run dev:client   # Frontend only
npm run dev:server   # Backend only
```

### 5. Build for production

```bash
npm run build
```

### Reproducibility check

A clean install should work with:

```bash
git clone https://github.com/AnupaLodhi/medi-bridge-ai.git
cd medi-bridge-ai
npm install && cd client && npm install && cd ../server && npm install && cd ..
npm run dev
```

---

## Project Structure

```
medi-bridge-ai/
├── client/                     # React frontend
│   └── src/
│       ├── components/         # Shared UI components
│       │   ├── ImageUpload.tsx # Camera / gallery / file upload
│       │   └── SendToPharmacy.tsx
│       ├── context/            # Accessibility context
│       ├── pages/              # Portal pages
│       │   ├── PatientPortal.tsx
│       │   ├── DoctorPortal.tsx
│       │   ├── PharmacyPortal.tsx
│       │   └── EmergencyDelivery.tsx
│       ├── services/           # API client
│       └── types/              # TypeScript types
├── server/                     # Node.js / Express backend
│   └── src/
│       ├── routes/             # API route handlers
│       ├── services/           # Prescription parser, voice assistant
│       └── index.ts            # Server entry point
├── CITATION.cff                # Citation metadata (GitHub auto-detects)
├── CHANGELOG.md                # Version history
├── CODE_OF_CONDUCT.md          # Community standards
├── CONTRIBUTING.md             # How to contribute
├── LICENSE                     # MIT License
└── package.json                # Root workspace scripts
```

---

## Design System

| Token | Value | Usage |
|---|---|---|
| Primary | `#0F2D52` | Navy blue — headers, buttons, navigation |
| Secondary | `#FFFFFF` | Backgrounds, cards |
| Accent | `#EAF3FF` | Light blue — highlights, badges |
| Success | `#22C55E` | Verified, positive states |
| Warning | `#F59E0B` | Alerts, pending states |
| Danger | `#D32F2F` | Emergency, errors |

Typography: **Inter** (UI), **SF Pro Display** (headings)

---

## Testing

See [TESTING.md](TESTING.md) for the full guide.

```bash
# Frontend tests
cd client && npm test

# Backend tests
cd server && npm test
```

---

## Contributing

Contributions are welcome! Please read [CONTRIBUTING.md](CONTRIBUTING.md) before submitting a pull request.

1. Fork the repo
2. Create a feature branch: `git checkout -b feat/your-feature`
3. Commit with a clear message: `git commit -m "feat: add your feature"`
4. Push and open a pull request against `main`

Please follow our [Code of Conduct](CODE_OF_CONDUCT.md).

---

## Citation

If you use MediBridge AI in research or academic work, please cite:

```bibtex
@software{medi_bridge_ai_2026,
  author  = {Lodhi, Anupa},
  title   = {{MediBridge AI}},
  year    = {2026},
  version = {1.0.0},
  url     = {https://github.com/AnupaLodhi/medi-bridge-ai},
  license = {MIT}
}
```

Machine-readable citation metadata is in [CITATION.cff](CITATION.cff) — GitHub shows a **"Cite this repository"** button automatically.

---

## Roadmap

- [ ] Multilingual voice assistant (10 Indian languages) — in progress
- [ ] Drug interaction checker — in progress
- [ ] Handwriting OCR for prescription reading
- [ ] Generic medicine suggester for pharmacies
- [ ] Telemedicine video consultation
- [ ] Doctor appointment booking
- [ ] PDF export for prescriptions
- [ ] WhatsApp / SMS medication reminders

---

## License

This project is licensed under the [MIT License](LICENSE) © 2026 Anupa Lodhi.

---

<div align="center">
  <sub>Built with ❤️ for better healthcare in India</sub>
</div>
