# PriestyAI - Terms of Service & End User Agreement (EULA)

Last Updated: August 2026

By installing the **PriestyAI GitHub App**, inviting the **PriestyAI Discord Bot**, granting collaborator access to the `@PriestyAI` machine account, or utilizing the hosted service, you agree to these Terms. If you do not agree, do not install or use the service.

---

### 1. Nature of the Service & Zero SLA
* **Community Project:** PriestyAI is an experimental, autonomous AI developer and community companion service provided free of charge on an **"AS-IS"** and **"AS-AVAILABLE"** basis.
* **No Uptime Guarantees:** The service operates without a Service Level Agreement (SLA). The operator reserves the right to restart, modify, rate-limit, pause, or permanently discontinue the service at any time without notice or liability.

---

### 2. Machine User & GitHub Repository Modification
* **Programmatic Write Access:** Granting the `@PriestyAI` machine account write access authorizes the bot to create branches, push commits, open pull requests, and manage issue workflows programmatically.
* **Human-in-the-Loop Review Requirement:** PriestyAI utilizes probabilistic generative AI (Google Gemini). Output code may contain bugs, hallucinated packages, or syntax errors. **You are solely responsible for independently auditing, testing, and approving all code, patches, and commands prior to merging or deploying to production.**
* **Sandbox Verification:** Containerized test execution runs inside ephemeral Docker sandboxes. You acknowledge that automated test execution may fail or produce unexpected results based on your repository configuration.

---

### 3. Discord Community Features & Media Processing
* **Server News & Broadcasts:** By activating Server News or chatting in public channels where PriestyAI is present, server administrators and members grant PriestyAI permission to analyze public text logs, presences, and announcements to generate recap summaries, charts, and video media.
* **Third-Party Video Hosting:** Rendered daily broadcast clips may be uploaded to third-party hosting providers (e.g., Streamable) and are subject to their respective content and retention policies.

---

### 4. Acceptable Use & Prohibited Conduct
You agree not to use or prompt PriestyAI to:
1. Generate, test, or distribute malware, exploits, or malicious payloads via GitHub sandboxes or chat.
2. Perform prompt injection, jailbreaking, or adversarial testing against backend API tools.
3. Intentionally spam, flood, or bypass rate limits on GitHub webhooks, Discord gateways, or LLM endpoints.
4. Harass users or impersonate official project creators or maintainers.

---

### 5. API Quotas & Access Termination
To protect infrastructure and API quotas from abuse:
* The operator reserves the right to immediately block, rate-limit, blacklist, or remove the bot from any Discord server or GitHub repository without explanation or notice.

---

### 6. Disclaimer of Warranties & Limitation of Liability
TO THE MAXIMUM EXTENT PERMITTED BY APPLICABLE LAW:
* PRIESTYAI IS PROVIDED WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE, OR NON-INFRINGEMENT.
* IN NO EVENT SHALL THE OPERATOR, CREATOR, OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING LOSS OF DATA, CORRUPTION OF REPOSITORIES, CI/CD CHARGES, SERVICE DOWNTIME, OR BUSINESS INTERRUPTION) ARISING OUT OF OR IN CONNECTION WITH THE USE OF THIS SERVICE.