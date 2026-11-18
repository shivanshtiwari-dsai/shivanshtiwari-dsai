# SeaSphere

**Smart India Hackathon 2026 platform for AI-powered freight forecasting and maritime supply-chain optimization.**

[![SIH 2026](https://img.shields.io/badge/Smart%20India%20Hackathon-2026-FF9933?style=for-the-badge)](https://github.com/shivanshtiwari-dsai/my-sih-2026-sea-sphere)
[![License: MIT](https://img.shields.io/badge/License-MIT-22C55E?style=for-the-badge)](./LICENSE)

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white)

---

## Live Demo & Preview

- **Live Demo:** _Deployment link coming soon_ <!-- Replace with your deployed URL, e.g. https://seasphere.vercel.app -->
- **API Docs (Local Swagger UI):** `http://localhost:8000/docs`

![App Screenshot](./assets/preview.png)

---

## Key Features

- **Freight Demand Forecasting:** Predictive analytics models that estimate container volumes, port congestion, and lead-time fluctuations across shipping lanes.
- **Supply-Chain Route Optimization:** Decision-support engine that recommends cost-effective, lower-delay routing and inventory allocation strategies.
- **High-Performance FastAPI Backend:** Async Python REST APIs with automatic OpenAPI/Swagger documentation for forecasting inference and logistics telemetry.
- **Interactive Analytics Dashboard:** Modern React web interface visualizing shipment KPIs, forecast trends, bottleneck alerts, and scenario comparisons.
- **MongoDB Data Layer:** Flexible document storage for port schedules, historical freight datasets, optimization runs, and user scenarios.

---

## Project Folder Structure

```text
my-sih-2026-sea-sphere/
├── assets/
│   └── preview.png                 # Dashboard screenshot for README
├── backend/                        # Python + FastAPI backend
│   ├── app/
│   │   ├── api/
│   │   │   └── routes/
│   │   │       ├── forecast.py     # Freight forecasting endpoints
│   │   │       └── optimize.py     # Supply-chain optimization endpoints
│   │   ├── core/
│   │   │   ├── config.py           # Environment & app settings
│   │   │   └── database.py         # MongoDB client initialization
│   │   ├── models/                 # Pydantic schemas & DB models
│   │   ├── services/               # Forecasting & optimization logic
│   │   └── main.py                 # FastAPI application entry point
│   ├── requirements.txt            # Python dependencies
│   └── .env.example                # Backend environment template
├── frontend/                       # React client application
│   ├── public/
│   ├── src/
│   │   ├── components/             # Charts, tables, and UI widgets
│   │   ├── pages/                  # Dashboard, Forecasting, Optimization views
│   │   ├── services/               # API integration layer
│   │   └── App.jsx
│   ├── package.json
│   └── .env.example                # Frontend environment template
├── .gitignore
├── LICENSE
└── README.md
```

---

## Local Installation & Setup

### Prerequisites

- [Python](https://www.python.org/) (v3.10 or higher) & `pip`
- [Node.js](https://nodejs.org/) (v18 or higher) & `npm`
- [MongoDB](https://www.mongodb.com/) (local instance or MongoDB Atlas cluster)
- [Git](https://git-scm.com/)

### 1. Clone the Repository

```bash
git clone https://github.com/shivanshtiwari-dsai/my-sih-2026-sea-sphere.git
cd my-sih-2026-sea-sphere
```

### 2. Backend Setup (FastAPI & Python)

```bash
cd backend
python -m venv venv

# Activate virtual environment
# Windows (PowerShell):
.\venv\Scripts\Activate.ps1
# macOS / Linux:
# source venv/bin/activate

pip install -r requirements.txt
```

Create a `backend/.env` file:

```env
APP_ENV=development
MONGODB_URI=mongodb://localhost:27017/seasphere
DATABASE_NAME=seasphere
CORS_ORIGINS=http://localhost:5173
```

Start the FastAPI server:

```bash
uvicorn app.main:app --reload --port 8000
```

The API will be available at `http://localhost:8000` (interactive docs at `http://localhost:8000/docs`).

### 3. Frontend Setup (React)

Open a new terminal in the repository root:

```bash
cd frontend
npm install
```

Create a `frontend/.env` file:

```env
VITE_API_BASE_URL=http://localhost:8000
```

Start the React development server:

```bash
npm run dev
```

Open `http://localhost:5173` in your browser to explore **SeaSphere** locally.

---

## Contributing

Contributions, bug reports, and optimization ideas are welcome!

1. **Fork** the repository.
2. **Create** a feature branch:
   ```bash
   git checkout -b feat/your-feature-name
   ```
3. **Commit** your changes with concise, conventional commit messages:
   ```bash
   git commit -m "feat: add port congestion risk scoring"
   ```
4. **Push** to your branch:
   ```bash
   git push origin feat/your-feature-name
   ```
5. **Open a Pull Request** detailing your changes and any setup notes.

---

## License

This project is licensed under the **MIT License** — see the [LICENSE](./LICENSE) file for details.

---

## Author

**Shivansh Tiwari** — [@shivanshtiwari-dsai](https://github.com/shivanshtiwari-dsai) · [shivanshtiw120706@gmail.com](mailto:shivanshtiw120706@gmail.com)
