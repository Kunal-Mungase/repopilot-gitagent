# RepoPilot – Git Repo Understanding Agent

## Overview
RepoPilot is an AI agent built for the GitAgent Hackathon.
It helps developers understand unfamiliar repositories, generate better README files, and debug common setup or code issues.

## Problem
Developers often waste time understanding project structure, missing documentation, and common setup errors when working with unfamiliar repositories.

## Solution
RepoPilot reads a repository and helps by:
- Summarizing what the project does
- Explaining important folders and files
- Creating or improving README documentation
- Helping debug project issues in simple language

## Why this matters
This solves a real developer productivity problem and makes onboarding into new repositories faster and easier.

## GitAgent Structure
This project follows the GitAgent standard:
- \`agent.yaml\` – manifest
- \`SOUL.md\` – identity and communication style
- \`RULES.md\` – hard constraints
- \`skills/\` – core capabilities

## Skills
### 1. summarize-repo
Explains the purpose, structure, and key parts of a repository.

### 2. generate-readme
Creates a simple and useful README for a project.

### 3. debug-helper
Reads errors and suggests likely fixes in a clear way.

## Tech Used
- GitAgent standard
- gitclaw runtime
- Node.js
- Markdown
- YAML

## Project Structure
repopilot-gitagent/
├── agent.yaml
├── SOUL.md
├── RULES.md
├── README.md
├── package.json
├── demo.js
└── skills/
    ├── summarize-repo/
    │   └── SKILL.md
    ├── generate-readme/
    │   └── SKILL.md
    └── debug-helper/
        └── SKILL.md
        
## How to Run Locally
1. Clone the repository
2. Run `npm install`
3. Review `agent.yaml`, `SOUL.md`, `RULES.md`, and the `skills/` folder
4. Run `npm start`
5. Use gitclaw as the runtime for integrating this GitAgent-defined agent

## Future Improvements
- Add codebase Q&A
- Add issue triage
- Add clawless deployment later
