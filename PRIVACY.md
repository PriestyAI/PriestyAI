# PriestyAI - Privacy Policy

Last Updated: August 2026

Your privacy and code confidentiality are core priorities. This policy explains what data PriestyAI accesses, how it is processed, and how you can manage or delete your information.

### 1. Information Accessed & Processed

#### On GitHub:
* **Repository Context:** PriestyAI only reads repository files, issue comments, and PR diffs in repositories where the GitHub App is installed and explicitly triggered (via assignees, reviews, or `@PriestyAI` mentions).
* **Test Sandboxes:** Sandboxed container test runs are ephemeral and destroyed immediately upon verification completion.
* **External Forks:** Automated container execution is skipped on external forks unless explicitly authorized by a maintainer.

#### On Discord:
* **Conversational Logs:** Chat messages are held in temporary memory solely to maintain short-term conversational context and are purged after rolling timeouts.
* **Long-Term Memory Journals:** Extracted user facts (e.g. tech stack, preferences) are stored as dense semantic vector records inside a dedicated, private brain storage database.
* **Server News Scrapes:** Daily server activity, gaming stats, and public announcements are processed temporarily to compile broadcast news videos and deleted from local staging caches after rendering.

### 2. Third-Party AI Sub-Processors
PriestyAI routes prompt contexts to **Google Gemini API** to generate responses, plans, and code.
### 3. Data Retention & User Control
You maintain full control over your stored data:
* **Reset Memory:** Right-click any member in Discord $\rightarrow$ **Apps** $\rightarrow$ **Reset AI Memory** to permanently purge all stored memory records for that user.
* **Delete Context Snapshots:** Run `/context delete alias:<name>` to permanently delete saved profile snapshots.
* **Channel Purge:** Remove PriestyAI from your server or uninstall the GitHub App at any time to instantly stop all data processing.

### 4. Contact
For privacy questions, data deletion requests, or security disclosures, please open an issue at [github.com/PriestyAI/PriestyAI/issues](https://github.com/PriestyAI/PriestyAI/issues).