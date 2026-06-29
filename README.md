<div align="center">

# Clew

**A premium, local-first AI IDE for macOS Apple Silicon.**
The privacy-first alternative to Cursor — featuring a built-in local model manager, multi-provider API support, and a stunning native interface. Just download the `.dmg` and go.

[![Platform](https://img.shields.io/badge/platform-macOS%20M1%2B%20(Silicon)-lightgrey.svg)]()
[![Platform](https://img.shields.io/badge/platform-Windows%20(coming%20soon)-blue.svg)]()
[![License](https://img.shields.io/badge/license-Apache%202.0-green.svg)](LICENSE)
[![Status](https://img.shields.io/badge/status-active-success.svg)](#)

**[Download Latest Release](https://github.com/OpenSynapseLabs/Clew/releases)**

</div>

---

> **Clew = Cursor + LM Studio + Multi-API Gateway, wrapped in a single .dmg.** 🚀
> No Python dependencies to install. No telemetry. Absolute privacy for local models, with the flexibility to plug in cloud APIs. 
> Your workflow, supercharged.

## 🌟 Why Clew?

Most AI IDEs force you to choose between local privacy and cloud capabilities. Clew bridges the gap by offering a unified, premium experience natively built for macOS.

**Clew ships everything in one app:**
- 🧠 **Multi-Provider Inference:** Seamlessly switch between local models (GGUF/MLX) and cloud APIs (Anthropic, z.ai, and many others).
- 🛰️ **Built-in API Gateway:** For maximum speed, Clew runs a local server that efficiently handles and routes API requests and responses.
- 📂 **Integrated Code Viewer:** Select a project directory and instantly read any file in the built-in Viewer without leaving the app.
- ✨ **Premium UI/UX:** A breathtakingly polished interface with light, dark, and system themes, complete with ambient background effects simulating neural synapses.
- 🔒 **Absolute Privacy:** Everything local runs entirely on your machine. Zero outbound calls unless you explicitly use a cloud API.

---

## 🖼️ Visual Tour

A meticulously crafted interface built natively for macOS. No Electron. Pure performance, gorgeous aesthetics.

| | |
|:---:|:---:|
| ![Main Workspace](Screenshot%202026-06-29%20at%2018.42.21.png) | ![Desktop Integration](Screenshot%202026-06-29%20at%2018.42.34.png) |
| **Unified Workspace** — Natural language task composer with templates and instant project indexing. | **Native Experience** — Seamlessly integrates into your macOS desktop environment. |
| ![Agent View](agent_2.png) | ![Chat View](chat.png) |
| **Agent Control** — Define tasks, monitor resource usage, and track token consumption in real-time. | **Chat & Terminal** — Converse with your agent and execute commands in a unified space. |
| ![Skills Marketplace](marketplace.png) | *Internal Code Viewer & Themes (Try it live!)* |
| **Skills Marketplace** — Browse and load specialized AI skills. | **Code Viewer** — Open and read your entire project structure effortlessly on the right panel. |

*(Note: The interface now features stunning ambient synapse effects in the background, which can be toggled in settings).*

---

## 🧠 Models & APIs

Clew gives you the ultimate freedom in choosing your inference engine. 

**Local Models (GGUF / MLX):**
Works with any open-source model on Hugging Face. 
*   **Llama 3.1 / 3.2** (Meta) — Excellent general-purpose coding and reasoning.
*   **Mistral / Mixtral** (Mistral AI) — Fast, efficient, great at following instructions.
*   **Qwen 2.5** (Alibaba) — Outstanding performance per parameter size.
*   **Phi-3 / Phi-3.5** (Microsoft) — Incredible speed and logic for small sizes.

**Cloud APIs:**
Don't want to run models locally? Bring your own API keys. Clew natively supports:
*   **Anthropic** (Claude family)
*   **z.ai** and other major providers.
*   *All routed through Clew's high-speed internal API server for minimal latency.*

---

## 🚀 Installation

### Requirements
- **macOS 13+** on **Apple Silicon (M1, M2, M3, M4, M5)**.
- ~4 GB of free RAM for small local models, ~8-10 GB for standard 7B-8B models.

### The Easy Way (Recommended)

Clew comes with a built-in auto-updater. You only need to install it once!

1. Go to the [Releases](https://github.com/OpenSynapseLabs/Clew/releases) page.
2. Download the latest `Clew-vX.X.X-arm64.dmg`.
3. Double-click to mount, drag **Clew** to **Applications**.
4. On first launch: Right-click → **Open** → **Open anyway** (to bypass Gatekeeper).
5. Open **Settings** → Choose your theme, configure your API keys or download a local model.

### From Source (For Developers)

```bash
git clone https://github.com/OpenSynapseLabs/Clew.git
cd Clew
python3 -m venv .venv
source .venv/bin/activate
pip install -e .
clew
```

---

## 🏁 Quick Start

1. **Open a Project:** `File → Open Folder…` (⌘O). Clew indexes your codebase, and the **Code Viewer** opens on the right, letting you read any file instantly.
2. **Configure Inference:** Go to **Settings**. Add an API key (e.g., Anthropic) or go to **My Models** to download a local one.
3. **Pick a Template:** In the main workspace, choose a prompt template (e.g., *Code Project*), select a Skill, and describe your task.
4. **Run Agent:** Watch Clew plan, read, write, and execute code autonomously. Live token counting keeps you informed of context usage.

---

## ✨ Key Features

<details>
<summary><strong>🎨 Premium UI & Customization</strong></summary>

- **Theme Engine:** Switch between Light, Dark, and System themes.
- **Ambient Synapse Effects:** Beautiful background animations mimicking neural pathways. Can be toggled off in settings for a distraction-free environment.
- **Integrated Code Viewer:** A powerful right-panel viewer that lets you read and explore your entire project directory without opening external editors.
- Native macOS integration: custom menus, high-DPI support, and flawless typography.

</details>

<details>
<summary><strong>🧩 Unified Workspace & Templates</strong></summary>

- **Natural Language Task Composer:** Describe what you want to build in plain English.
- **Prompt Templates:** Pre-configured templates for rapid task initiation. Just insert your specific words and go.
- **Agent Skills:** Reusable context profiles to guide the agent's behavior.

</details>

<details>
<summary><strong>⚙️ Advanced Inference & API Gateway</strong></summary>

- **Multi-Provider Support:** Switch between local LLMs and cloud APIs (Anthropic, z.ai, etc.) on the fly.
- **Local API Server:** Clew spins up a lightweight local server to handle API requests and routing, ensuring maximum speed and streaming performance.
- **Detailed Local Settings:** Fine-tune local model parameters (threads, context size, GPU layers) directly in the app.
- **Live Token Counting:** Accurate, real-time tracking of token usage during agent runs and chats.

</details>

<details>
<summary><strong>🤖 Autonomous Agent Runtime</strong></summary>

- ReAct-style loop: The AI thinks, plans, calls tools, and observes results.
- Sandboxed tool execution: Commands run securely without risking your system.
- Live UI trace: Watch the agent's thoughts, file reads, and code writes in real-time.

</details>

---

## 🗺️ Roadmap

We are actively developing Clew. Here is what to expect in upcoming releases:

- **Expanded Templates & Skills:** Introducing specialized modes like *Office Worker* for document tasks and *Heavy Code* for deep, complex repository refactoring.
- **Git Integration:** Branch status, diff viewer, and commit UI.
- **Advanced Debugging:** Deep introspection of agent runs and variable states.
- **Plugin System:** Allow the community to build and share their own tools.
- **Cross-Platform:** Windows and Linux ports.

---

## 📬 Contact & Support

- **Email:** [opensynapselabs@proton.me](mailto:opensynapselabs@proton.me)
- **Issues:** [GitHub Issue Tracker](https://github.com/OpenSynapseLabs/Clew/issues)

---

## 📄 License

Apache License 2.0 — see [LICENSE](LICENSE).

Built with care by **Open Synapse Labs**.

---

<div align="center">

**[Download Latest Release](https://github.com/OpenSynapseLabs/Clew/releases)** ·
**[Report a Bug](https://github.com/OpenSynapseLabs/Clew/issues)**

</div>
