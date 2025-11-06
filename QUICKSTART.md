# SuperClaude Marketplace - Quick Start Guide

Get started with the SuperClaude Framework in minutes.

## Installation

### Option 1: Add Marketplace (Recommended)

```bash
# Add the SuperClaude marketplace
claude plugin marketplace add caiomioto2/SuperClaude_MarketplacePlugin

# Install the plugin
claude plugin install superclaude
```

### Option 2: Clone Repository

```bash
# Clone the repository
git clone https://github.com/caiomioto2/SuperClaude_MarketplacePlugin.git

# Navigate to the plugin directory
cd SuperClaude_MarketplacePlugin/plugins/superclaude

# Start Claude Code (auto-detects plugin)
claude
```

## First Steps

Once installed, the SuperClaude plugin automatically activates via SessionStart hook.

### Available Commands

1. **PM Agent Orchestrator**
   ```bash
   /agent
   ```
   Launches the PM Agent with confidence-driven workflow (≥90% threshold required before implementation).

2. **Deep Research**
   ```bash
   /research <your research query>
   ```
   Autonomous web research with adaptive planning, multi-hop reasoning (up to 5 iterations).

3. **Repository Indexing**
   ```bash
   /index-repo
   ```
   Smart repository indexing for 94% token reduction (58K → 3K).

### Available Skills

Use the confidence check skill before major implementations:

```
@confidence-check
```

This ensures ≥90% confidence before proceeding, preventing costly mistakes.

## Quick Examples

### Example 1: Research-Driven Development

```bash
# Start Claude Code
claude

# Research a topic
/research "best practices for Next.js 15 server actions with authentication"

# Review results and implement with confidence
```

### Example 2: Large Codebase Optimization

```bash
# Index your repository
/index-repo

# Now work with reduced token usage
# Ask questions about your codebase efficiently
```

### Example 3: Quality-First Implementation

```bash
# Before implementing a complex feature
@confidence-check

# PM Agent will assess and ensure ≥90% confidence
# Only proceed when confidence threshold is met
```

## MCP Server Integration (Optional)

For enhanced performance, install MCP servers:

### Via airis-mcp-gateway (Recommended)

```bash
npm install -g airis-mcp-gateway

# Configure in Claude Code settings
# Add Tavily, Context7, Serena, Sequential, etc.
```

### Benefits with MCP Servers

- **2-3x faster** execution (Serena code understanding)
- **30-50% fewer tokens** (Sequential reasoning)
- **Enhanced research** (Tavily + Context7)
- **Cross-session learning** (Mindbase)

## Configuration

### SessionStart Hook

The plugin automatically activates on session start. To disable:

Edit `plugins/superclaude/hooks/hooks.json` and remove or comment out the SessionStart hook.

### Custom Workflows

Modify commands and agents in:
- `plugins/superclaude/commands/` - Command definitions
- `plugins/superclaude/agents/` - Agent behaviors

## Troubleshooting

### Plugin Not Loading

1. Verify installation:
   ```bash
   claude plugin marketplace list
   ```

2. Update marketplace:
   ```bash
   claude plugin marketplace update
   ```

3. Reinstall plugin:
   ```bash
   claude plugin uninstall superclaude
   claude plugin install superclaude
   ```

### Commands Not Available

Ensure the plugin is enabled:
```bash
claude plugin enable superclaude
```

### MCP Integration Issues

Check MCP server status in Claude Code settings:
- Tools → MCP Servers
- Verify servers are running and accessible

## Next Steps

1. **Read Full Documentation**: [README.md](README.md)
2. **Review Architecture**: [MARKETPLACE_STRUCTURE.md](MARKETPLACE_STRUCTURE.md)
3. **Check Updates**: [CHANGELOG.md](CHANGELOG.md)
4. **Join Community**: [Discord](https://discord.gg/superclaude)

## Use Cases

### Quality-First Development
Ensure ≥90% confidence before implementation, preventing costly mistakes and rework.

### Research-Intensive Projects
Autonomous web research with adaptive planning handles complex information gathering.

### Large Codebases
94% token reduction allows working with repositories that would otherwise exceed context limits.

### Systematic Workflows
PM Agent orchestration provides structure for complex multi-step tasks.

## Statistics

| Metric | Value |
|--------|-------|
| Commands | 3 |
| Agents | 3 |
| Skills | 1 |
| MCP Servers | 8 (optional) |
| Token Reduction | 94% |
| Confidence Threshold | 90% |

## Support

- **GitHub Issues**: [Report bugs](https://github.com/SuperClaude-Org/SuperClaude_Framework/issues)
- **Discussions**: [Ask questions](https://github.com/SuperClaude-Org/SuperClaude_Framework/discussions)
- **Discord**: [Join community](https://discord.gg/superclaude)
- **Website**: [Documentation](https://superclaude.netlify.app/)

## License

MIT License - Free and open-source forever.

---

**Version**: 4.1.6 | **Last Updated**: 2025-01-05

**Built with passion by the SuperClaude community** ❤️
