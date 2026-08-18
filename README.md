# PriestyAI

[![Install GitHub App](https://img.shields.io/badge/GitHub_App-Install-blue?logo=github)](https://github.com/apps/priestyai)
[![Machine Account](https://img.shields.io/badge/Machine_User-@PriestyAI-181717?logo=github)](https://github.com/PriestyAI)
[![Add to Discord](https://img.shields.io/badge/Discord-Add_to_Server-5865F2?logo=discord&logoColor=white)](https://discord.com/oauth2/authorize?client_id=1509364708476452894)
[![User App](https://img.shields.io/badge/User_App-Install_to_Account-eb459e?logo=discord&logoColor=white)](https://discord.com/oauth2/authorize?client_id=1509364708476452894)

PriestyAI is an autonomous AI ecosystem that brings intelligent developer and community workflows natively to your chosen workspace. Whether acting as a transparent pair programmer on **GitHub** or an interactive, multi-modal companion on **Discord**, PriestyAI operates alongside your team rather than as an opaque black box.

---

## QuickStart

Get PriestyAI running in your workspace:

### On GitHub (Pair Programmer)
1. **Install the App:** Add [PriestyAI](https://github.com/apps/priestyai) to your repository or organization.
2. **Invite the Machine User:** Go to repository **Settings** &rarr; **Collaborators** and invite `@PriestyAI` with write access *(auto-accepted within 30 seconds)*.
3. **Assign an Issue:** Assign `@PriestyAI` to any issue (or comment `@PriestyAI work on this`). PriestyAI will open a Draft PR with a step-by-step implementation plan.

### On Discord (AI Companion)
1. **Invite PriestyAI:** Add [PriestyAI](https://discord.com/oauth2/authorize?client_id=1509364708476452894) to your Discord server, or install it to your personal account as a **User App**.
2. **Configure Features:** Run `/config` to customize active tool pipelines, system instructions, or Server News.
3. **Start Chatting:** Mention `@PriestyAI` in channels, reply to messages, or run `/chat`.

---

## GitHub Workflows

PriestyAI integrates directly into your native GitHub development lifecycle without requiring rigid slash commands.

### 1. Autonomous Issue-to-PR Workflow

> [!TIP]
> The more context provided in an issue (reproduction steps, expected behavior, relevant file paths), the more accurate PriestyAI's plan and execution will be.

```
Assign Issue ──▶ Draft PR Opened ──▶ Review & Approve ──▶ Sandbox Verified ──▶ Ready for Review
```

1. **Assign:** Add `@PriestyAI` under **Assignees** on an issue (or comment `@PriestyAI work on this`).
2. **Review Plan:** PriestyAI creates a clean feature branch and opens a **Draft Pull Request** containing a checklist plan.
3. **Approve:** React with 👍, 🚀, 👀 or comment @PriestyAI `"approved"` / `"LGTM"`.
4. **Autonomous Build & Verification:** PriestyAI implements changes, runs test/linter suites in an isolated Docker container with self-healing passes, creates atomic commits, and publishes a native GitHub Check Run.
5. **Ready for Review:** Once all checks pass, PriestyAI marks the PR **Ready for Review** and requests maintainer sign-off.

### 2. Thoughtful Pull Request Reviews
Add `@PriestyAI` under **Reviewers** on any open PR. PriestyAI inspects diffs against the base branch's `CONTRIBUTING.md`, runs checks, and submits reviews with 1-click native suggestion blocks. Comment `@PriestyAI fix <notes>` or submit *Changes Requested* to trigger autonomous fix commits.

### 3. Discussions & ChatOps
* **Discussions Q&A:** Auto-answers questions in **Q&A**, **Questions**, or **Help** categories using repository files.
* **ChatOps:** Administrators can @mention PriestyAI to execute and chain commands, such as closing PRs or assigning members

---

## Discord Capabilities

PriestyAI serves as a full-featured community companion and server automation platform.

### 1. Transparent Reasoning & Multi-Modal Chat
* **Inner Thoughts:** Click the **`Thought for Xs`** button on any response to inspect PriestyAI's step-by-step logic in a private popup.
* **Document & Image Extraction:** Reads attached images, PDFs, Word documents (`.docx`), Excel sheets (`.xlsx`), audio clips, and source code.
* **LaTeX Formula Rendering:** Automatically renders math and physics equations into clean 150 DPI graphics.

### 2. Automated Daily Server Newsroom
Compiles fully voiced, multi-scene MP4 news broadcast videos recapping your server's daily chatter, active gaming trends, and scheduled events:
* **Morning Edition:** Data-driven show featuring server activity charts, upcoming event calendars, and interactive Question of the Day (QOTD) polls.
* **Late-Night Edition:** Satirical talk show featuring couch guest interviews, award plaques, community mailbags, and AI vibe art reveals.

### 3. Modern Components V2 Message Builder
PriestyAI compiles custom Python layout specifications into modern Discord UI Components V2 (borderless containers, column-based sections with accessories, buttons, and custom modal forms).

### 4. Autonomous Research Agents (`/agent`)
Launch autonomous multi-step reasoning agents in private workspace threads. Ground them with saved message context snapshots or user profiles to perform investigations and data synthesis.

---

## Command Cheatsheet

### GitHub Commands

| Goal | Example Command / Action | Context |
| :--- | :--- | :--- |
| **Start Issue** | Assign `@PriestyAI` or `@PriestyAI work on this` | Issues |
| **Approve Plan** | React with 👍, 🚀, 👀 or comment `"approved"` | Draft PRs |
| **Decompose Epic** | `@PriestyAI split this into sub-issues` | Issues |
| **Request Review** | Add `@PriestyAI` to **Reviewers** | Pull Requests |
| **Apply Fixes** | `@PriestyAI fix <instructions>` or *Changes Requested* | Pull Requests |
| **Resolve Conflicts** | `@PriestyAI resolve conflicts` | Pull Requests |
| **Run Tests** | `@PriestyAI run tests` | Pull Requests |
| **ChatOps Actions** | `@PriestyAI assign @alice`, `@PriestyAI squash and merge` | Issues & PRs |
| **Spin Off Issue** | `@PriestyAI create an issue to track <task>` | Discussions, Issues, PRs |

### Discord Commands & Context Menus

| Command / Action | Description | Type |
| :--- | :--- | :--- |
| `/chat` | Starts an interactive conversation session | Slash Command |
| `/config` | Configures active tools, prompt rules, or Server News | Slash Command |
| `/generate` | Forces generation of Images, Components V2, or Legacy UI | Slash Command |
| `/agent` | Launches an autonomous research agent thread | Slash Command |
| **Re-run** | Generates an alternative response version with pagination | Context Menu (Right-Click) |
| **Branch** | Creates an isolated conversation branch thread from a message | Context Menu (Right-Click) |
| **Save Context** | Archives a message transcript or user profile as an agent snapshot | Context Menu (Right-Click) |
| **Reset AI Memory** | Clears long-term vector memory records for a user | Context Menu (Right-Click) |

---

## Security and Sandboxing 

* **Isolated Docker Execution:** GitHub test runs and automated fixes execute in ephemeral Docker containers with strict timeouts and memory boundaries.
* **External Fork Protection:** Automated container execution is skipped on external untrusted forks unless explicitly authorized by a maintainer.
---

## Feedback & Bug Reports

Encounter an issue or have a feature request? Please [open an issue](https://github.com/PriestyAI/PriestyAI/issues) in this repository!
