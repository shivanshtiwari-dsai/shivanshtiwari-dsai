# SHIVI AI

**A modern conversational AI assistant featuring custom voice interaction, dynamic theming, conversational memory, and MongoDB persistence.**

[![Live Demo](https://img.shields.io/badge/Live%20Demo-GitHub%20Pages-2F81F7?style=for-the-badge&logo=githubpages&logoColor=white)](https://shivanshtiwari-dsai.github.io/CHATBOT_SHIVI/)
[![License: MIT](https://img.shields.io/badge/License-MIT-22C55E?style=for-the-badge)](./LICENSE)

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white)

---

## Live Demo & Preview

- **Live App:** [https://shivanshtiwari-dsai.github.io/CHATBOT_SHIVI/](https://shivanshtiwari-dsai.github.io/CHATBOT_SHIVI/)

![App Screenshot](./assets/preview.png)

---

## Key Features

- **Custom Voice Interaction:** Hands-free speech-to-text input and spoken assistant responses using browser speech synthesis and recognition APIs.
- **Dynamic Theme Customization:** Instant light/dark and accent theme switching with persistent user preferences across sessions.
- **Conversational Memory:** Context-aware multi-turn dialogue handling that retains conversation flow for coherent follow-up responses.
- **MongoDB Backend Integration:** Scalable Node.js REST API backed by MongoDB for storing chat sessions, user settings, and message history.
- **Responsive Chat UI:** Clean, accessible, mobile-friendly interface built with semantic HTML5, modern CSS3, and vanilla JavaScript.

---

## Project Folder Structure

```text
CHATBOT_SHIVI/
├── assets/
│   └── preview.png             # Application screenshot for README
├── public/                     # Frontend client files
│   ├── index.html              # Main chat UI markup
│   ├── styles/
│   │   ├── main.css            # Base layout & component styles
│   │   └── themes.css          # Dynamic theme variables
│   └── scripts/
│       ├── app.js              # Core chat & API client logic
│       ├── voice.js            # Speech recognition & TTS handler
│       └── theme.js            # Theme switcher & persistence
├── server/                     # Node.js backend
│   ├── config/
│   │   └── db.js               # MongoDB connection setup
│   ├── models/
│   │   └── Conversation.js     # Mongoose schema for chat history & memory
│   ├── routes/
│   │   └── chat.js             # Chat & memory API endpoints
│   └── server.js               # Express/Node entry point
├── .env.example                # Environment variable template
├── .gitignore
├── package.json
├── LICENSE
└── README.md
```

---

## Local Installation & Setup

### Prerequisites

- [Node.js](https://nodejs.org/) (v18 or higher) & `npm`
- [MongoDB](https://www.mongodb.com/) (local instance or MongoDB Atlas cluster)
- [Git](https://git-scm.com/)

### 1. Clone the Repository

```bash
git clone https://github.com/shivanshtiwari-dsai/CHATBOT_SHIVI.git
cd CHATBOT_SHIVI
```

### 2. Install Dependencies

```bash
npm install
```

### 3. Configure Environment Variables

Create a `.env` file in the project root (or copy `.env.example`):

```bash
cp .env.example .env
```

Update `.env` with your local credentials:

```env
PORT=5000
MONGODB_URI=mongodb://localhost:27017/shivi_ai
AI_API_KEY=your_api_key_here
NODE_ENV=development
```

| Variable | Description |
| :--- | :--- |
| `PORT` | Port on which the Node.js server runs (default: `5000`). |
| `MONGODB_URI` | MongoDB connection string (local or Atlas URI). |
| `AI_API_KEY` | API key for the conversational AI provider (if applicable). |
| `NODE_ENV` | Runtime environment (`development` or `production`). |

### 4. Run the Server

```bash
# Development mode (with auto-reload)
npm run dev

# Production mode
npm start
```

Open `http://localhost:5000` in your browser to interact with **SHIVI AI** locally.

---

## Contributing

Contributions, issue reports, and feature suggestions are welcome!

1. **Fork** the repository.
2. **Create** a feature branch:
   ```bash
   git checkout -b feat/your-feature-name
   ```
3. **Commit** your changes with clear, descriptive messages:
   ```bash
   git commit -m "feat: add custom voice speed controls"
   ```
4. **Push** to your branch:
   ```bash
   git push origin feat/your-feature-name
   ```
5. **Open a Pull Request** describing what changed and why.

---

## License

This project is licensed under the **MIT License** — see the [LICENSE](./LICENSE) file for details.

---

## Author

**Shivansh Tiwari** — [@shivanshtiwari-dsai](https://github.com/shivanshtiwari-dsai) · [shivanshtiw120706@gmail.com](mailto:shivanshtiw120706@gmail.com)
