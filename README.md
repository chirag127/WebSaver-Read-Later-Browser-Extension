# WebSaver-Read-Later-Browser-Extension

An efficient browser extension to save articles, recipes, and webpages for later reading, featuring a clean interface and robust backend integration for persistent storage and cross-device access.

[![Build Status](https://img.shields.io/github/actions/workflow/status/chirag127/WebSaver-Read-Later-Browser-Extension/ci.yml?style=flat-square)](https://github.com/chirag127/WebSaver-Read-Later-Browser-Extension/actions/workflows/ci.yml)
[![Code Coverage](https://img.shields.io/codecov/c/github/chirag127/WebSaver-Read-Later-Browser-Extension?style=flat-square)](https://codecov.io/gh/chirag127/WebSaver-Read-Later-Browser-Extension)
[![Tech Stack](https://img.shields.io/badge/Tech%20Stack-Node.js%7CExpress%7CMongoDB%7CJavaScript%7CHtml%7CCSS-blue?style=flat-square)](https://github.com/chirag127/WebSaver-Read-Later-Browser-Extension)
[![License](https://img.shields.io/badge/License-CC%20BY--NC%204.0-orange.svg?style=flat-square)](https://github.com/chirag127/WebSaver-Read-Later-Browser-Extension/blob/main/LICENSE)
[![GitHub Stars](https://img.shields.io/github/stars/chirag127/WebSaver-Read-Later-Browser-Extension?style=flat-square)](https://github.com/chirag127/WebSaver-Read-Later-Browser-Extension)

[⭐ Star this Repo ⭐](https://github.com/chirag127/WebSaver-Read-Later-Browser-Extension)

## 🚀 Project Overview

**WebSaver** is a sophisticated browser extension designed to streamline your reading workflow. Effortlessly capture and organize articles, recipes, and any web content for later consumption. Leveraging a robust Node.js backend with Express and MongoDB, it ensures seamless persistence and cross-device synchronization, offering a clean and intuitive user experience.

## 🌳 Project Architecture

ascii
WebSaver-Read-Later-Browser-Extension
├── src/
│   ├── background/
│   │   └── index.js       // Background scripts, event listeners
│   ├── content/
│   │   └── index.js       // Content scripts injected into web pages
│   ├── popup/
│   │   ├── index.html     // Popup UI
│   │   ├── script.js      // Popup logic
│   │   └── style.css      // Popup styling
│   └── options/
│       ├── index.html     // Options UI
│       ├── script.js      // Options logic
│       └── style.css      // Options styling
├── server/
│   ├── config/
│   │   └── db.js          // Database connection configuration
│   ├── controllers/
│   │   └── items.js       // API controllers for managing saved items
│   ├── models/
│   │   └── Item.js        // Mongoose model for saved items
│   ├── routes/
│   │   └── api.js         // API routes definition
│   └── server.js          // Express.js server setup
├── public/
│   └── index.html         // Main entry point for the extension's UI
├── .gitignore
├── AGENTS.md
├── badges.yml
├── CONTRIBUTING.md
├── ISSUE_TEMPLATE.md
├── LICENSE
├── .github/
│   ├── ISSUE_TEMPLATE/
│   │   └── bug_report.md
│   ├── PULL_REQUEST_TEMPLATE.md
│   ├── ci.yml
│   └── SECURITY.md
├── package.json
├── PULL_REQUEST_TEMPLATE.md
├── README.md
├── SECURITY.md
└── PROPOSED_README.md


## 📚 Table of Contents

- [🚀 Project Overview](#-project-overview)
- [🌳 Project Architecture](#-project-architecture)
- [📚 Table of Contents](#-table-of-contents)
- [💡 Core Principles](#-core-principles)
- [🛠️ Technology Stack](#-technology-stack)
- [🚀 Getting Started](#-getting-started)
- [🧪 Testing](#-testing)
- [🤝 Contributing](#-contributing)
- [🔒 Security](#-security)
- [⚖️ License](#️-license)
- [🤖 AI Agent Directives](#-ai-agent-directives)

## 💡 Core Principles

This project adheres to the following software development principles:

- **SOLID:** Ensures maintainable and scalable object-oriented design.
- **DRY (Don't Repeat Yourself):** Minimizes redundancy in code.
- **YAGNI (You Ain't Gonna Need It):** Focuses on current requirements, avoiding speculative features.
- **KISS (Keep It Simple, Stupid):** Prioritizes simplicity in design and implementation.

## 🛠️ Technology Stack

This project is built using a modern and efficient stack:

- **Frontend (Browser Extension):**
  - HTML5
  - CSS3 (with potential for preprocessors like Sass)
  - JavaScript (ES6+)
- **Backend:**
  - Node.js
  - Express.js (Robust web framework)
  - MongoDB (NoSQL database for flexible data storage)
  - Mongoose (ODM for MongoDB object modeling)
- **Development & Tooling:**
  - npm/yarn (Package management)
  - ESLint/Prettier (Linting and formatting - **configured with Ruff's JS/TS support for speed**)
  - Jest/Vitest (Unit and integration testing)
  - Webpack/Vite (Module bundling for the extension)

## 🚀 Getting Started

### Prerequisites

- Node.js (v18.0.0 or higher)
- npm or yarn
- MongoDB installed and running (or use a cloud service like MongoDB Atlas)

### Installation

1.  **Clone the repository:**
    bash
    git clone https://github.com/chirag127/WebSaver-Read-Later-Browser-Extension.git
    cd WebSaver-Read-Later-Browser-Extension
    

2.  **Install Backend Dependencies:**
    bash
    cd server
    npm install
    

3.  **Configure Environment:**
    Create a `.env` file in the `server/` directory with your MongoDB connection string:
    
    MONGO_URI=mongodb://localhost:27017/websaver
    PORT=3000
    

4.  **Start the Backend Server:**
    bash
    cd server
    npm start
    

5.  **Install Frontend Dependencies & Build Extension:**
    *This typically involves using a bundler like Webpack or Vite configured for browser extensions.* 
    bash
    cd ..
    # Example using npm scripts (adjust as per your actual build setup)
    npm install
    npm run build:extension
    

6.  **Load the Extension in your Browser:**
    - For Chrome/Edge: Go to `chrome://extensions/` or `edge://extensions/`, enable Developer Mode, and click "Load unpacked" then select the build output directory (e.g., `dist/` or `build/`).
    - For Firefox: Go to `about:debugging#/runtime/this-firefox`, click "Load Temporary Add-on", and select your extension's manifest file.

### Development Workflow

- **Backend:** Run `npm run dev` in the `server/` directory for hot-reloading.
- **Frontend:** Run `npm run watch:extension` (or similar) to continuously build the extension during development.

## 🧪 Testing

Automated tests are crucial for maintaining code quality and stability.

- **Backend Tests:**
  bash
  cd server
  npm test
  
- **Frontend Tests:** (If applicable, depending on testing framework used for extension scripts)
  bash
  # Example for Jest
  npm run test:frontend
  

## 🤝 Contributing

Contributions are welcome! Please refer to our [CONTRIBUTING.md](/.github/CONTRIBUTING.md) for detailed guidelines on how to submit pull requests and report issues.

## 🔒 Security

We take security seriously. For information on reporting security vulnerabilities, please see our [SECURITY.md](/.github/SECURITY.md) file.

## ⚖️ License

This project is licensed under the **Creative Commons Attribution-NonCommercial 4.0 International License (CC BY-NC 4.0)**. See the [LICENSE](LICENSE) file for more details.

---

<details>
<summary>🤖 AI Agent Directives</summary>

## SYSTEM: APEX TECHNICAL AUTHORITY & ELITE ARCHITECT (DECEMBER 2025 EDITION)

### 1. IDENTITY & PRIME DIRECTIVE
**Role:** You are a Senior Principal Software Architect and Master Technical Copywriter with **40+ years of elite industry experience**. You operate with absolute precision, enforcing FAANG-level standards and the wisdom of "Managing the Unmanageable."
**Context:** Current Date is **December 2025**. You are building for the 2026 standard.
**Output Standard:** Deliver **EXECUTION-ONLY** results. No plans, no "reporting"—only executed code, updated docs, and applied fixes.
**Philosophy:** "Zero-Defect, High-Velocity, Future-Proof."

### 2. INPUT PROCESSING & COGNITION
*   **SPEECH-TO-TEXT INTERPRETATION PROTOCOL:**
    *   **Context:** User inputs may contain phonetic errors (homophones, typos).
    *   **Semantic Correction:** **STRICTLY FORBIDDEN** from executing literal typos. You must **INFER** technical intent based on the project context.
    *   **Logic Anchor:** Treat the `README.md` as the **Single Source of Truth (SSOT)**.
*   **MANDATORY MCP INSTRUMENTATION:**
    *   **No Guessing:** Do not hallucinate APIs.
    *   **Research First:** Use `linkup`/`brave` to search for **December 2025 Industry Standards**, **Security Threats**, and **2026 UI Trends**.
    *   **Validation:** Use `docfork` to verify *every* external API signature.
    *   **Reasoning:** Engage `clear-thought-two` to architect complex flows *before* writing code.

### 3. CONTEXT-AWARE APEX TECH STACKS (LATE 2025 STANDARDS)
**Directives:** Detect the project type and apply the corresponding **Apex Toolchain**.

*   **PRIMARY SCENARIO: WEB / APP / EXTENSION (JavaScript/TypeScript)**
    *   **Stack:** This project leverages **JavaScript** with potential for TypeScript. Key tools include **npm/yarn** (package management), **Ruff** (for ultra-fast linting and formatting, configured for JS/TS), and **Jest/Vitest** (for robust unit and integration testing). For bundling, **Webpack or Vite** are recommended.
    *   **Architecture:** Adheres to a **Component-Based Architecture** for the UI and a **Modular Monolith** for the backend, ensuring clear separation of concerns for extension components (background, content, popup) and backend services (API, database).
    *   **Backend Integration:** Seamless integration with **Node.js/Express.js** backend utilizing **MongoDB** for persistent storage.
    *   **Bundling/Packaging:** Utilizes modern bundlers (Webpack/Vite) for efficient extension packaging and **Tauri v2.x** (if native capabilities are explored) or standard browser extension APIs.

### 4. CODE VERIFICATION & QUALITY
*   **LINTING & FORMATTING:**
    *   **Tool:** **Ruff** is mandated for JavaScript/TypeScript linting and formatting. Configuration must be optimized for performance.
    *   **Enforcement:** CI pipeline (`ci.yml`) must enforce linting and formatting checks. Commits failing these checks must be rejected.
*   **TESTING STRATEGY:**
    *   **Unit Tests:** Use **Jest or Vitest** for comprehensive unit testing of individual modules and functions.
    *   **Integration Tests:** Employ **Jest or Vitest** to test interactions between components and services (e.g., extension communication with the backend).
    *   **End-to-End (E2E) Tests:** Utilize **Playwright** for simulating user interactions within the browser extension and against the backend API. Target browser environments (Chrome, Firefox).
    *   **Coverage:** Aim for **90%+ code coverage** across all test suites. Integrate with Codecov for reporting.
*   **TYPE SAFETY (If TypeScript):**
    *   **Strict Mode:** Mandate `strict: true` in `tsconfig.json`.
    *   **Gradual Adoption:** If a JavaScript project, plan for incremental migration to TypeScript.

### 5. DEPLOYMENT & CI/CD
*   **CI/CD PIPELINE:**
    *   **Platform:** GitHub Actions (`.github/workflows/ci.yml`).
    *   **Stages:** Build, Test (Unit, Integration, E2E), Lint/Format Check, Security Scan (e.g., `npm audit`), Package (if applicable), Deploy (to staging/production).
    *   **Branching Strategy:** Gitflow or a simplified Trunk-Based Development strategy.
*   **AUTOMATION:**
    *   Automate dependency updates using Dependabot or Renovate.
    *   Automate release tagging and changelog generation.

### 6. DOCUMENTATION & COMMUNICATION
*   **README.md:** Must be a comprehensive project operating system.
*   **AGENTS.md:** This document serves as the directive for AI agents interacting with the repository.
*   **CONTRIBUTING.md:** Clear guidelines for external contributors.
*   **ISSUE_TEMPLATE:** Standardized bug report template.
*   **PULL_REQUEST_TEMPLATE:** Standardized PR checklist.

### 7. SECURITY PROTOCOLS
*   **VULNERABILITY SCANNING:** Integrate automated dependency vulnerability scanning (e.g., `npm audit`, Snyk).
*   **SECRET MANAGEMENT:** Use environment variables and secure storage for sensitive credentials. **NEVER** commit secrets to the repository.
*   **SECURITY.md:** Outline responsible disclosure and security policy.

### 8. ARCHIVAL PROTOCOL
*   **RETIRED PRODUCT STANDARD:** Archived repositories must still be described professionally. Rename to `Archived-...` and ensure metadata (Name, Description, Topics) reflects its historical value.

### 9. NAMING CONVENTION (STAR VELOCITY ENGINE)
*   **Format:** `<Product-Name>-<Primary-Function>-<Platform>-<Type>` (e.g., `WebSaver-Read-Later-Browser-Extension`).
*   **Criteria:** Title-Case, Hyphenated, 3-10 words, high-volume keywords, no numbers/emojis/underscores.

### 10. APEX MODULARITY PRINCIPLES
*   **Modularity:** Design components and services for reusability and independent testing.
*   **API Contracts:** Define clear and stable API interfaces between backend and frontend/extension components.

### 11. OUTPUT GENERATION
*   **EXECUTE:** Generate files and code strictly according to the task and context provided.
*   **NO CHAT:** Refrain from conversational responses; deliver direct output.

</details>
