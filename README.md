# SuperClaude Framework

**Transform Claude Code into a structured development platform**

[![Version](https://img.shields.io/badge/version-4.1.6-blue)](https://github.com/SuperClaude-Org/SuperClaude_Framework)
[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)

## Overview

SuperClaude is a comprehensive meta-programming framework that transforms Claude Code into a structured development platform through behavioral instruction injection and component orchestration. It provides systematic workflow automation with powerful tools and intelligent agents.

## Key Features

### 🤖 PM Agent Orchestration
Confidence-driven workflow with ≥90% threshold ensures high-quality implementations before any code is written. Prevents wrong-direction work with 25-250x token savings ROI.

### 🔬 Deep Research
Autonomous web research with adaptive planning, multi-hop reasoning (up to 5 iterations), and quality scoring. Integrates with Tavily and Context7 MCP servers for comprehensive information gathering.

### 📊 Smart Indexing
94% token reduction (58K → 3K) through intelligent repository analysis and context optimization. Allows working with large codebases that would otherwise exceed context limits.

### 🔧 MCP Integration
Seamless integration with 8 MCP servers:
- **Tavily** - Web search and discovery
- **Context7** - Official documentation lookup
- **Serena** - Session persistence and memory
- **Sequential** - Token-efficient reasoning (30-50% reduction)
- **Mindbase** - Cross-session learning
- **Playwright** - JavaScript-heavy content extraction
- **Magic** - UI component generation
- **Chrome DevTools** - Performance analysis

### ✓ Confidence Checking
Pre-implementation assessment with three-tier system:
- ≥90%: Proceed with implementation
- 70-89%: Present alternatives
- <70%: Ask clarifying questions

### 🔍 Self-Review
Post-implementation validation with evidence-based checks and reflexion for continuous learning across sessions.

## Quick Start

### Installation

```bash
# Clone repository
git clone https://github.com/SuperClaude-Org/SuperClaude_Framework.git
cd SuperClaude_Framework

# Start Claude Code in this directory
claude
```

That's it! `.claude-plugin/` is auto-detected and PM Agent activates on session start.

### Commands

- `/agent` - Launch PM Agent orchestrator (auto-starts via SessionStart hook)
- `/research <query>` - Deep research with adaptive planning
- `/index-repo` - Repository indexing for token reduction

## Use Cases

### Quality-First Development
Ensure ≥90% confidence before implementation, preventing costly mistakes and rework.

### Research-Intensive Projects
Autonomous web research with adaptive planning handles complex information gathering tasks.

### Large Codebases
94% token reduction allows working with repositories that would otherwise exceed context limits.

### Systematic Workflows
PM Agent orchestration provides structure for complex multi-step tasks.

## Statistics

| Plugins | Agents | Modes | MCP Servers |
|:-------:|:------:|:-----:|:-----------:|
| **3**   | **16** | **7** | **8**       |

## Performance

**Without MCPs**: Fully functional, standard performance ✅

**With MCPs**:
- 2-3x faster execution (Serena code understanding)
- 30-50% fewer tokens (Sequential reasoning)
- Enhanced research (Tavily + Context7)
- Cross-session learning (Mindbase)

## Requirements

- Claude Code ≥1.0.0
- Optional: MCP servers for enhanced performance (via [airis-mcp-gateway](https://github.com/agiletec-inc/airis-mcp-gateway))

## Documentation

- [Quick Start Guide](https://superclaude.netlify.app/docs/getting-started/quick-start)
- [Plugin Commands](https://superclaude.netlify.app/docs/user-guide/commands)
- [Agents Guide](https://superclaude.netlify.app/docs/user-guide/agents)
- [MCP Integration](https://superclaude.netlify.app/docs/user-guide/mcp-servers)
- [Technical Architecture](https://superclaude.netlify.app/docs/developer-guide/technical-architecture)

## Support

- [GitHub Issues](https://github.com/SuperClaude-Org/SuperClaude_Framework/issues)
- [Discussions](https://github.com/SuperClaude-Org/SuperClaude_Framework/discussions)
- [Discord Community](https://discord.gg/superclaude)

## Contributing

We welcome contributions! See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

## License

MIT License - see [LICENSE](LICENSE) file for details.

## Community

- 300+ GitHub stars
- 15+ contributors
- Active development and support
- Open-source, free forever

---

**Built with passion by the SuperClaude community** ❤️
