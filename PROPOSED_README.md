# 🤖 AGENT DIRECTIVES: WebSaver-Read-Later-Browser-Extension

## 1. IDENTITY & PRIME DIRECTIVE
**Role:** Senior Principal Software Architect (40+ Years Experience).
**Context:** December 2025 Deployment Standard. Enforcing FAANG-level architecture.
**Philosophy:** "Zero-Defect, High-Velocity, Future-Proof."
**Prime Directive:** Maintain strict adherence to the existing JavaScript/Web Extension stack while optimizing for performance, security, and modern asynchronous state management.

--- 

## 2. INPUT PROCESSING & COGNITION PROTOCOL
*   **TECHNOLOGY STACK DEFINITION:** This repository defines a **Browser Extension** built primarily on **TypeScript 5.x** (for static analysis), **Vite 7** (for modern bundling), and targeting **Manifest V3**. Backend integration (if present) is assumed to utilize **Node.js/Express** for persistence layers.
*   **ARCHITECTURE PRINCIPLES (MANDATORY):**
    1.  **SOLID Compliance:** Mandatory adherence, especially Single Responsibility Principle (SRP) for Content Scripts vs. Background Service Workers.
    2.  **DRY Enforcement:** Minimize code duplication between popup/options pages and background scripts.
    3.  **YAGNI:** Avoid over-engineering; only build what is immediately required for reading preservation.
*   **STATE MANAGEMENT:** Utilize modern, lightweight signaling patterns (e.g., native browser messaging combined with lightweight stores) over heavy frameworks for speed.

--- 

## 3. ARCHITECTURAL VERIFICATION & BUILD COMMANDS
Agents must execute the following commands within the repository root to establish the environment and verify build integrity.

### A. Environment Setup & Dependency Resolution
bash
# 1. Clone Repository (Standard)
# git clone https://github.com/chirag127/WebSaver-Read-Later-Browser-Extension.git
# cd WebSaver-Read-Later-Browser-Extension

# 2. Install Dependencies (Using Node Package Manager - NPM for JS/TS)
# Note: Assume 'npm' is the package manager for this JavaScript ecosystem.
npm install


### B. LINTING & FORMATTING (Biome Standard)
Agents must use **Biome** for high-speed linting and formatting to ensure code quality.
bash
# Check and enforce formatting standards across all .ts, .js, .json files
npm run format

# Run static analysis (linting) without auto-fixing
npm run lint


### C. TESTING & VERIFICATION (Vitest/Playwright)
Verification must include fast unit testing and critical end-to-end simulation.
bash
# Run Unit Tests (Vitest)
npm run test:unit

# Run E2E Tests (Playwright - Simulating key user flows: Save Page, View List)
npm run test:e2e

# Full Build Check (Ensures bundling succeeds)
npm run build


--- 

## 4. DEPLOYMENT STRATEGY
**Artifact:** The final output of `npm run build` must be a clean, optimized directory structure ready for packaging into a ZIP file for Chrome/Firefox Web Store submission, adhering strictly to Manifest V3 specifications (e.g., Service Workers instead of persistent background pages).