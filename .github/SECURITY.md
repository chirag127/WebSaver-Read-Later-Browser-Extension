# Security Policy

## Supported Versions

We are committed to maintaining the security of the `WebSave-AI-Powered-Read-It-Later-Browser-Extension`. This policy outlines the security support for different versions. For the most up-to-date security, always use the latest release.

| Version           | Supported          |
| ----------------- | ------------------ |
| Latest (`main`)   | :white_check_mark: |
| Previous Release  | :x:                |

## Reporting a Vulnerability

We take all security vulnerabilities seriously. If you discover a security issue in `WebSave-AI-Powered-Read-It-Later-Browser-Extension`, please report it to us promptly via one of the following methods:

1.  **GitHub Issues (Private Report if possible):** The preferred method is to open a GitHub Issue and **request it to be private** if it contains sensitive information. Please include:
    *   A clear description of the vulnerability.
    *   Steps to reproduce the vulnerability.
    *   The impact of the vulnerability.
    *   Any relevant system information (browser, OS, extension version).

2.  **Email:** If you are unable to use GitHub Issues or prefer email, please send your report to `security@example.com` (Note: This is a placeholder email. In a real-world scenario, this would be a dedicated security contact email).

We will acknowledge receipt of your report within **48 hours** and will work with you to address the issue. Please do not disclose the vulnerability publicly until we have had a chance to release a fix.

## Security Practices

*   **Dependency Management:** We regularly scan our dependencies for known vulnerabilities using automated tools integrated into our CI/CD pipeline.
*   **Code Audits:** Regular code reviews and audits are conducted to identify potential security weaknesses.
*   **Least Privilege:** The extension operates on the principle of least privilege, requesting only the necessary permissions to function.
*   **Data Handling:** Sensitive user data is handled with care, encrypted where appropriate, and stored securely.
*   **AI Integration Security:** When interacting with AI services (like potential future backend AI calls), we ensure secure API key management and validate all inputs and outputs to prevent prompt injection or data leakage.

--- 

Thank you for helping keep `WebSave-AI-Powered-Read-It-Later-Browser-Extension` secure!
