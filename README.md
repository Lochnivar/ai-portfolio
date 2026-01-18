# AI Portfolio

A reference repository showcasing AI applications across **creative**, **analytical**, and **professional** contexts.

## Overview

This repository serves as a documentation and reference hub for 5 AI projects, demonstrating practical applications of artificial intelligence in different domains:

- **Creative**: Artistic and expressive AI applications (image generation, creative writing, music, etc.)
- **Analytical**: Data-driven AI solutions (predictive modeling, machine learning, business intelligence, etc.)
- **Professional**: Enterprise and productivity-focused AI tools (automation, workflow optimization, etc.)

> **Note**: This repository contains project summaries and links to the actual project repositories. The included HTML/CSS/JS files can be deployed to any static hosting service (Netlify, Vercel, etc.) but this repo itself serves as a reference point.

## Local Development

To preview the website locally:

1. Clone this repository
2. Open `index.html` in your web browser, or
3. Serve using a local development server:
   ```bash
   # Using Python
   python -m http.server 8000
   
   # Using Node.js (http-server)
   npx http-server
   ```

## Projects

### Creative Projects

#### Project 01: AshVerse - Alternate History Novel Series
**Description**: An epic 6-book alternate history series set in a timeline where Robert E. Lee dies at Gettysburg in 1863, fundamentally changing the course of American history. The project demonstrates sophisticated AI collaboration through multiple specialized systems:

- **AI Refresher Sheets**: Comprehensive 3,500+ word canon reference documents (`canon-refresher-for-ai.md`, `canon-refresher-for-ai-detailed.md`) designed specifically for AI assistants, containing critical timeline anchors, process rules, plausibility scores, and cross-references to 250+ documentation files
- **Wargaming Simulations**: Turn-based military operation simulation framework (`wargaming-simulation-template.md`, `wargaming-simulation-guide.md`) for modeling campaigns with realistic opposition, anti-bias mechanisms, and multi-phase operations (2-3 day turns, Corps/Army level)
- **Battle Simulations**: Tactical-level simulation templates (`battle-simulation-template.md`, `battle-simulation-guide.md`) for brigade/division engagements with 1-2 hour turns, focusing on positioning, firepower, and morale
- **Plausibility Gate Process**: Formal 70% threshold scoring system (`plausibility-gate-process.md`) for all world-building decisions, ensuring historical accuracy while allowing creative flexibility
- **Consistency Systems**: Hash-based dependency tracking (`calculate-hash.py`, `consistency-checker.py`) for maintaining canon consistency across 250+ markdown files
- **Process Rules**: Structured AI interaction guidelines (Golden Rule, Honesty Rule, Git Operations Rule) ensuring AI never edits original text, always models competent opposition, and maintains historical plausibility

Features extensive AI-assisted world-building, character development, historical analysis, and multi-generational storytelling spanning 1863-1939.

**Repository**: [https://github.com/Lochnivar/ashverse](https://github.com/Lochnivar/ashverse)

**Tags**: Creative, Writing, World-Building, Alternate History, AI-Assisted Writing, Wargaming Simulation, Plausibility Analysis, Historical Research

---

#### Project 02: The Way TTRPG - Tabletop Role-Playing Game System
**Description**: A complete tabletop RPG system design featuring the innovative d20+ die mechanic, Path Matrix™ character progression system, and universal Strain resource management. The project demonstrates extensive AI-assisted game design, mechanics development, and system documentation across 60+ files. Features open development philosophy with tiered release strategy supporting 7,776 unique character builds at full release. Includes comprehensive rules for combat, magic, martial techniques, character progression, and equipment systems.

**Repository**: [https://github.com/Lochnivar/theway](https://github.com/Lochnivar/theway)

**Tags**: Creative, Game Design, TTRPG, RPG System Design, AI-Assisted Development

---

### Analytical Projects

#### Project 04: BattleTech: Material Economy Redesign
**Description**: Procedural generation system that grounds BattleTech's conflicts in material reality rather than abstract honor. The project creates a complete material economy where astrophysical reality constrains strategic options—factions fight because they need specific resources that only exist in specific stellar environments.

**Key Features**:
- **Astrophysical Constraints**: Every strategic resource tied to stellar classification (O, B, A, F, G, K, M types) and planetary characteristics
- **3d6 Probability Distribution**: Uses bell curve distribution familiar to BattleTech players to create realistic resource scarcity
- **Critical Resource Dependencies**: Myomer requires organic polymers (G/K stars), advanced electronics require rare earths, fusion engines require specific isotopes
- **Emergent Strategic Gameplay**: Resource distribution creates natural conflict zones, strategic dependencies, and meaningful trade relationships without DM fiat
- **Python Implementation**: Procedural generation code using 3d6 mechanics with astrophysical constraints
- **YAML System Data**: Generated system files containing complete economic profiles for each star system

**AI Collaboration Methodology**:
- **Astrophysical Research**: Used AI to rapidly gather and synthesize information about stellar classification, planetary chemistry, and resource formation processes
- **Balance Validation**: Tested resource distribution algorithms against AI-generated scenarios to identify edge cases and ensure no faction could achieve resource monopolies
- **Code Generation**: AI assisted in implementing 3d6 probability distributions and stellar constraint logic, with human oversight ensuring game design goals
- **Documentation**: Collaborated with AI to create clear technical documentation explaining both scientific rationale and gameplay implications

**Key Insight**: AI excels at exploring the possibility space of complex systems—suggesting edge cases, identifying balance issues, and generating test scenarios. Human judgment remains essential for deciding which realistic constraints create interesting gameplay versus which create tedium.

**Technologies**: Python, YAML, Procedural Generation, Statistical Modeling, Astrophysics Research

**Status**: Feature Complete

**Repository**: Private/In Development

**Tags**: Analytical, Game Systems, Procedural Generation, Systems Modeling, AI-Assisted Development, Constraint-Based Design

**Detailed Documentation**: See [`battletech-economy.html`](battletech-economy.html) for comprehensive case study with design principles and technical implementation.

---

#### Project 05: [Project Title]
**Description**: Brief description of your analytical AI project.

**Repository**: [Link to repository](https://github.com/username/repo-name)

**Tags**: Analytical, ML, [other tags]

---

### Professional Projects

#### Project 03: KAMS v2 - Enterprise Monitoring System
**Description**: Enterprise alert monitoring and management system demonstrating sophisticated AI-assisted deployment through a structured **AI Agent Instruction System** with mode-based workflows. The project features:

- **AI Agent Instruction System**: Structured seed documents (🤖 AI AGENT SEED markers) that guide AI agents through specific tasks with checklists, verification steps, and documentation requirements
- **Six Specialized Modes**:
  - **Installation Mode** (`INSTALLATION_VERIFICATION.md`): Automatic detection of Fresh Installation vs V1 Migration, structured verification checklists, installation type-specific workflows, passwordless sudo handling patterns
  - **Upgrade Mode** (`UPGRADE_PROCESS.md`): Sequential version upgrade support, automatic upgrade path detection, backup/recovery procedures, migration script execution, backward compatibility testing
  - **Verification Mode**: Existing installation testing, functionality verification, issue detection and documentation
  - **Reconciliation Mode** (`PRODUCTION_ISSUE_RECONCILIATION.md`): Production-to-dev synchronization, multi-site issue tracking, gap analysis workflows, structured issue categorization (Bug Fix, Feature Addition, Missing File, UI Fix), fix verification procedures
  - **Feature Development Mode** (`FEATURE_DEVELOPMENT.md`): Structured development workflows separated from reconciliation processes, code review checklists, testing requirements
  - **Cleanup Mode** (`RECONCILIATION_COMPLETE.md`): Reconciliation cycle completion, archival workflows, protection analysis to prevent accidental deletion
- **Structured Process Management**: Systematic checklists for each mode, issue documentation templates, status tracking (✅ FIXED, ⚠️ WORKAROUND, 🔴 PRODUCTION ISSUE), cross-reference mapping between production and dev
- **Anti-Pattern Prevention**: "Do Not Fix" rules preventing common mistakes (manual sudoers files, chmod 777 workarounds, DEV_ENVIRONMENT flags), write-to-temp-then-copy patterns for sudo file operations
- **Multi-Site Support**: Site header parsing (`## Site: [identifier]`), sequential issue numbering across sites, site-specific reconciliation workflows
- **Process Improvement Framework**: Standing invitation for AI agents to suggest process improvements, structured documentation of enhancements, automation hints for verification steps

Demonstrates practical AI integration for enterprise software lifecycle management with structured workflows ensuring consistency, quality, and maintainability across deployment environments.

**Repository**: Private Repository (Internal/Proprietary)

**Tags**: Professional, Enterprise, DevOps, AI-Assisted Development, Production Management, Structured Workflows, Process Automation

---

## Website Files

This repository includes HTML/CSS/JS files that can be deployed to any static hosting service:

- **Netlify**: Drag and drop the `index.html`, `styles.css`, and `script.js` files
- **Vercel**: Connect this repository and deploy
- **Any other static host**: Upload the files to your hosting provider

### Customization

To customize the website:

1. Edit `index.html` and update the project cards with your actual project information
2. Update `styles.css` to customize colors, fonts, and styling
3. Modify `script.js` for additional interactive features if needed

## Project Structure

```
ai-portfolio/
├── index.html      # Main HTML structure
├── styles.css      # Styling and responsive design
├── script.js       # Interactive features
└── README.md       # Project documentation
```

## Technologies

- HTML5
- CSS3 (with CSS Grid and Flexbox)
- Vanilla JavaScript
- Google Fonts (Inter)

## Purpose

This repository serves as:
- 📚 A reference hub with summaries of AI projects
- 🔗 A centralized location for links to individual project repositories
- 📄 Documentation of AI work across different contexts
- 🌐 Source files for a portfolio website (deployable elsewhere)
