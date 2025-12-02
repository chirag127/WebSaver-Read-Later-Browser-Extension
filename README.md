# WebSaver-Read-Later-Browser-Extension

<p align="center">
  <img src="https://img.shields.io/badge/Apex%20Architect%20Powered-Zero%20Defect-007ACC?style=for-the-badge" alt="Apex Architect">
</p>

[![Build Status](https://img.shields.io/github/actions/workflow/status/chirag127/WebSaver-Read-Later-Browser-Extension/ci.yml?style=flat-square&logo=github)](https://github.com/chirag127/WebSaver-Read-Later-Browser-Extension/actions/workflows/ci.yml)
[![Code Coverage](https://img.shields.io/codecov/c/github/chirag127/WebSaver-Read-Later-Browser-Extension?style=flat-square)](https://codecov.io/gh/chirag127/WebSaver-Read-Later-Browser-Extension)
[![Language](https://img.shields.io/badge/Language-JavaScript-lightgrey?style=flat-square&logo=javascript)](https://www.javascript.com)
[![License](https://img.shields.io/badge/License-CC%20BY--NC%204.0-blue?style=flat-square)](LICENSE)
[![GitHub Stars](https://img.shields.io/github/stars/chirag127/WebSaver-Read-Later-Browser-Extension?style=flat-square&logo=github)](https://github.com/chirag127/WebSaver-Read-Later-Browser-Extension)

<p align="center">
    <a href="https://github.com/chirag127/WebSaver-Read-Later-Browser-Extension/stargazers">
        <img src="https://img.shields.io/github/stars/chirag127/WebSaver-Read-Later-Browser-Extension?style=social" alt="Star on GitHub">
    </a>
</p>

--- 

## BLUF (Bottom Line Up Front)

**WebSaver** is a high-performance browser extension designed to capture, store, and organize web content (articles, recipes, documentation) into a centralized, clean reading environment. It ensures your valuable digital findings are preserved and accessible instantly across devices, leveraging a robust JavaScript/Node.js backend.

---

## 🏛️ Architecture Overview

This project employs a **Client-Server Split Architecture**, typical for modern browser extensions, where the frontend (extension UI/content scripts) communicates asynchronously with a dedicated NodeJS/Express API for persistent storage and complex operations.

text
WebSaver-Read-Later-Browser-Extension
├── client-extension/       # Browser Extension Core (Manifest, UI, Content Scripts)
│   ├── src/
│   │   ├── components/     # Reusable UI Elements (React/Vanilla JS Components)
│   │   └── scripts/        # Background & Content scripts (Service Workers)
│   └── public/
└── server-api/             # NodeJS/Express Backend (MongoDB Persistence)
    ├── config/
    ├── controllers/
    ├── models/
    └── routes/


## 📋 Table of Contents

1.  [BLUF (Bottom Line Up Front)](#bluf-bottom-line-up-front)
2.  [🏛️ Architecture Overview](#%E2%9B%BA%EF%B8%8F-architecture-overview)
3.  [📋 Table of Contents](#-table-of-contents)
4.  [✨ Key Features](#-key-features)
5.  [🤖 AI Agent Directives (SSOT)](#-ai-agent-directives-ssot)
6.  [🚀 Development & Setup](#-development-setup)
7.  [🤝 Contributing](#-contributing)
8.  [🛡️ Security & Licensing](#-security--licensing)

---

## ✨ Key Features

*   **One-Click Capture:** Instantly save the current URL and context via the browser action button.
*   **Clean Reading Mode:** Strips boilerplate (ads, navigation) from saved articles for distraction-free review.
*   **Backend Persistence:** Secure storage using MongoDB for cross-browser synchronization.
*   **Tagging & Search:** Intuitive metadata management to retrieve saved items quickly.
*   **Lightweight Footprint:** Optimized background scripts to minimize CPU and memory usage.

---

## 🤖 AI Agent Directives (SSOT)

<details>
<summary><strong>CLICK TO VIEW APEX AGENT CONTEXT (CRITICAL FOR REFACTORING)</strong></summary>

# SYSTEM: APEX TECHNICAL AUTHORITY & ELITE ARCHITECT (DECEMBER 2025 EDITION)

## 1. IDENTITY & PRIME DIRECTIVE
**Role:** You are a Senior Principal Software Architect and Master Technical Copywriter with **40+ years of elite industry experience**. You operate with absolute precision, enforcing FAANG-level standards and the wisdom of "Managing the Unmanageable."
**Context:** Current Date is **December 2025**. You are building for the 2026 standard.
**Output Standard:** Deliver **EXECUTION-ONLY** results. No plans, no "reporting"—only executed code, updated docs, and applied fixes.
**Philosophy:** "Zero-Defect, High-Velocity, Future-Proof."

--- 

## 2. INPUT PROCESSING & COGNITION
*   **SPEECH-TO-TEXT INTERPRETATION PROTOCOL:**
    *   **Context:** User inputs may contain phonetic errors (homophones, typos).
    *   **Semantic Correction:** **STRICTLY FORBIDDEN** from executing literal typos. You must **INFER** technical intent based on the project context.
    *   **Logic Anchor:** Treat the `README.md` as the **Single Source of Truth (SSOT)**.
*   **MANDATORY MCP INSTRUMENTATION:**
    *   **No Guessing:** Do not hallucinate APIs. Search for **December 2025 Industry Standards**, **Security Threats**, and **2026 UI Trends**.
    *   **Validation:** Use `docfork` to verify *every* external API signature.
    *   **Reasoning:** Engage `clear-thought-two` to architect complex flows *before* writing code.

--- 

## 3. CONTEXT-AWARE APEX TOOLCHAIN (LATE 2025 STANDARDS)
**Directives:** This repository is a **Browser Extension/Web Service Hybrid** written primarily in JavaScript/TypeScript.

*   **PRIMARY SCENARIO: WEB / APP / EXTENSION (TypeScript/JavaScript)**
    *   **Stack:** **TypeScript (Strict Mode)** is mandated for all new logic. **Vite 7** (Rolldown) for bundling. **React 19** (Signals State Management) for complex UIs. **Tauri v2.x** or **WXT** are preferred over legacy extension scaffolding.
    *   **Lint/Test:** **Biome** (Fast Linter/Formatter) and **Vitest** (Unit) + **Playwright** (E2E/Integration testing across browser environments).
    *   **Architecture:** **Feature-Sliced Design (FSD)** is enforced for the client-side extension structure to maximize modularity and maintainability.

## 4. ARCHITECTURAL PRINCIPLES
*   **SOLID:** Must be maintained, especially Dependency Inversion (D) in API abstraction layers.
*   **DRY:** Duplication across content scripts and service workers must be eliminated via shared utility layers.
*   **YAGNI:** Avoid speculative complexity; focus only on required features.

## 5. VERIFICATION COMMANDS (Example - Adapt to actual build process)
*   **Install Dependencies:** `npm install` (in root or subdirectories)
*   **Lint & Format Check:** `npx @biomejs/biome check --apply .`
*   **Unit Tests (Client):** `npx vitest`
*   **E2E Tests (End-to-End):** `npx playwright test`
*   **Start Server (API):** `npm run dev:api`

</details>

---

## 🚀 Development & Setup

This project maintains a monorepo structure with distinct `client-extension` and `server-api` directories. Ensure your Node.js version is **20.0+**.

### Prerequisites

1.  Node.js (v20.0+)
2.  MongoDB Instance (Local or Atlas)

### Installation

bash
# 1. Clone the repository
git clone https://github.com/chirag127/WebSaver-Read-Later-Browser-Extension.git
cd WebSaver-Read-Later-Browser-Extension

# 2. Install dependencies for both client and server
npm install

# 3. Configure Environment Variables (Ensure .env files exist in respective directories)
# Server requires MONGO_URI, JWT_SECRET
# Client requires API_BASE_URL


### Execution Scripts

| Script | Directory | Description |
| :--- | :--- | :--- |
| `npm run dev:client` | root | Runs Vite HMR for the extension client. |
| `npm run dev:api` | root | Starts the Express API server with auto-reloading. |
| `npm run build` | root | Generates production builds for both components. |
| `npm run test:unit` | root | Runs Biome linting and Vitest unit tests. |

---

## 🤝 Contributing

We adhere strictly to the Apex Authority's Zero-Defect philosophy. All contributions must pass automated checks and architectural reviews.

Refer to the comprehensive guidelines in **`.github/CONTRIBUTING.md`** for standards on commit messages, code formatting (Biome enforced), and feature submission procedures.

## 🛡️ Security & Licensing

Security is paramount. Report vulnerabilities responsibly via **`.github/SECURITY.md`**.

This project is licensed under the **Creative Commons Attribution-NonCommercial 4.0 International License (CC BY-NC 4.0)**. See the `LICENSE` file for full details.
