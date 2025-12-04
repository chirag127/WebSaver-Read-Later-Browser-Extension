# Contributing to WebSaver-Read-Later-Browser-Extension

Thank you for considering contributing to `WebSaver-Read-Later-Browser-Extension`! We aim to maintain a high standard of quality, velocity, and future-proofing, aligning with the Apex Technical Authority's principles.

## 1. Code of Conduct

This project adheres to the Contributor Covenant Code of Conduct. Please read the full [CODE_OF_CONDUCT.md](https://github.com/chirag127/WebSaver-Read-Later-Browser-Extension/blob/main/CODE_OF_CONDUCT.md) to understand the expected behavior.

## 2. How to Contribute

We welcome contributions in the form of:

*   **Bug Reports:** If you find a bug, please open an issue using the `bug_report.md` template.
*   **Feature Requests:** Suggest new features by opening an issue.
*   **Code Contributions:** Submit pull requests for bug fixes or new features.
*   **Documentation Improvements:** Help us keep our documentation up-to-date.

## 3. Development Workflow

Our development workflow is designed for high velocity and zero defects, utilizing the latest industry standards for late 2025.

### 3.1. Setup

1.  **Fork the repository:** Click the 'Fork' button on the GitHub page.
2.  **Clone your fork:**
    bash
    git clone https://github.com/chirag127/WebSaver-Read-Later-Browser-Extension.git
    cd WebSaver-Read-Later-Browser-Extension
    
3.  **Set upstream remote:**
    bash
    git remote add upstream https://github.com/chirag127/WebSaver-Read-Later-Browser-Extension.git
    
4.  **Create a new branch:** For your feature or fix:
    bash
    git checkout -b feature/your-feature-name
    

### 3.2. Technology Stack (Late 2025 Standards)

This project is built using modern JavaScript, leveraging a robust stack suitable for browser extensions:

*   **Language:** JavaScript (ES2025+)
*   **Build Tool:** Vite (v7+)
*   **Frontend Framework/Libraries:** (Specify if applicable, e.g., React, Vue, or Vanilla JS)
*   **Styling:** TailwindCSS (v4+)
*   **Backend (for storage/sync):** Node.js (LTS), Express.js
*   **Database:** MongoDB
*   **Extension API:** WebExtension APIs

### 3.3. Linting and Formatting

We use **Biome** for ultra-fast linting and formatting to ensure code consistency and quality. All code committed must pass Biome checks.

*   **Install Biome:** (Ensure Biome is installed as per `package.json` dev dependencies)
*   **Run Linter/Formatter:**
    bash
    npm run lint
    # or
    npm run format
    

### 3.4. Testing

Quality is paramount. We use **Vitest** for unit testing and **Playwright** for end-to-end (E2E) testing.

*   **Run Unit Tests:**
    bash
    npm run test:unit
    
*   **Run E2E Tests:**
    bash
    npm run test:e2e
    

### 3.5. Building the Extension

To build the production-ready extension:

bash
npm run build


## 4. Pull Request Process

1.  **Ensure your branch is up-to-date** with the main branch:
    bash
    git fetch upstream
    git merge upstream/main
    
2.  **Run all tests** and ensure they pass.
3.  **Lint and format** your code using `npm run lint` and `npm run format`.
4.  **Commit your changes** with clear and concise messages.
5.  **Open a Pull Request** against the `main` branch of the `chirag127/WebSaver-Read-Later-Browser-Extension` repository.
6.  **Provide a clear description** of your changes, referencing any related issues.

## 5. Architectural Principles

We adhere to the following principles:

*   **SOLID:** Maintainable and scalable code.
*   **DRY:** Don't Repeat Yourself.
*   **YAGNI:** You Ain't Gonna Need It – focus on necessary features.
*   **Zero-Defect:** Strive for bug-free code through rigorous testing and code reviews.
*   **High-Velocity:** Efficient development and deployment cycles.
*   **Future-Proof:** Design for extensibility and maintainability.

## 6. Reporting Security Vulnerabilities

If you discover a security vulnerability, please follow our security policy outlined in [SECURITY.md](https://github.com/chirag127/WebSaver-Read-Later-Browser-Extension/blob/main/SECURITY.md).

---