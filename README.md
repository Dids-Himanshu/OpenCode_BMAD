# BMAD Agent System for OpenCode

A comprehensive AI agent system built on OpenCode, providing specialized personas for the complete software development lifecycle using the BMAD (Business, Method, Architecture, Development) methodology.

## 🚀 Quick Start

### Prerequisites

- **Node.js** 18+ or **Bun** runtime
- **Git** for version control
- An AI provider account (OpenAI, Anthropic, Google, or GitHub Copilot)

### Install OpenCode

```bash
# One-line installation (recommended)
curl -fsSL https://opencode.ai/install | bash

# Or using npm
npm install -g opencode

# Or using bun
bun install -g opencode
```

### Clone and Setup

```bash
# Clone this repository
git clone <your-repo-url>
cd demoAgent

# Start OpenCode in the project directory
opencode
```

## 🤖 Available Agent Skills

This project includes 7 specialized AI agent personas:

| Agent | Command | Description |
|-------|---------|-------------|
| **Business Analyst** | `/analyst` | Market research, competitive analysis, requirements elicitation |
| **Software Architect** | `/architect` | System design, cloud infrastructure, API design |
| **Software Developer** | `/dev` | Story implementation, test-driven development |
| **Product Manager** | `/pm` | PRD creation, user interviews, stakeholder alignment |
| **QA Engineer** | `/qa` | Test automation, API testing, E2E test generation |
| **Quick Flow Solo Dev** | `/quick-flow-solo-dev` | Rapid tech specs and lean implementation |
| **Scrum Master** | `/sm` | Sprint planning, story preparation, agile ceremonies |

## 📁 Project Structure

```
demoAgent/
├── .opencode/
│   ├── skills/           # Agent skill definitions
│   │   ├── analyst/SKILL.md
│   │   ├── architect/SKILL.md
│   │   ├── dev/SKILL.md
│   │   ├── pm/SKILL.md
│   │   ├── qa/SKILL.md
│   │   ├── quick-flow-solo-dev/SKILL.md
│   │   └── sm/SKILL.md
│   ├── command/          # Slash commands
│   └── opencode.json     # OpenCode configuration
├── _bmad/                # BMAD methodology files
│   ├── bmm/              # Business Method Materials
│   │   ├── workflows/    # Workflow definitions
│   │   ├── data/         # Templates and data files
│   │   └── config.yaml   # User configuration
│   └── core/             # Core BMAD functionality
└── _bmad-output/         # Generated outputs
```

## 🎯 Using the Agents

### 1. Start OpenCode

```bash
cd demoAgent
opencode
```

### 2. Activate an Agent

Type any agent command to activate its persona:

```
/analyst    # Activate Business Analyst
/architect  # Activate Software Architect
/dev        # Activate Developer
/pm         # Activate Product Manager
/qa         # Activate QA Engineer
/sm         # Activate Scrum Master
```

### 3. Follow the Agent Menu

Each agent displays a menu of available actions. For example, the **Business Analyst** offers:

| Cmd | Action |
|-----|--------|
| **MH** | Redisplay Menu Help |
| **CH** | Chat with the Agent |
| **BP** | Brainstorm Project |
| **MR** | Market Research |
| **DR** | Domain Research |
| **TR** | Technical Research |
| **CB** | Create Product Brief |
| **DA** | Dismiss Agent |

### 4. Get Help Anytime

Use `/bmad-help` followed by your question:

```
/bmad-help where should I start with an idea I have?
```

## 🔧 Configuration

### User Settings

Edit `_bmad/bmm/config.yaml` to customize:

```yaml
user_name: "Your Name"
communication_language: "English"
output_folder: "_bmad-output"
```

### AI Provider Setup

OpenCode supports multiple AI providers:

- **GitHub Copilot** - Log in with your GitHub account
- **ChatGPT Plus/Pro** - Use your OpenAI subscription
- **Claude** - Connect your Anthropic API key
- **Gemini** - Use Google AI models
- **Local Models** - Run models locally via Ollama

## 📋 Workflow Examples

### Starting a New Project

1. `/analyst` → **BP** (Brainstorm Project)
2. `/analyst` → **CB** (Create Product Brief)
3. `/pm` → **CP** (Create PRD)
4. `/architect` → **CA** (Create Architecture)
5. `/pm` → **CE** (Create Epics and Stories)
6. `/sm` → **SP** (Sprint Planning)
7. `/dev` → **DS** (Dev Story)

### Quick Development Flow

1. `/quick-flow-solo-dev` → **QS** (Quick Spec)
2. `/quick-flow-solo-dev` → **QD** (Quick Dev)
3. `/quick-flow-solo-dev` → **CR** (Code Review)

## 🔗 Resources

- [OpenCode Documentation](https://opencode.ai/docs)
- [OpenCode GitHub](https://github.com/anomalyco/opencode)
- [OpenCode Discord Community](https://opencode.ai/discord)
## Inspiration 
 - BMAD (https://github.com/bmad-code-org/BMAD-METHOD?tab=readme-ov-file)
## 📄 License

MIT License - See [LICENSE](LICENSE) for details.
