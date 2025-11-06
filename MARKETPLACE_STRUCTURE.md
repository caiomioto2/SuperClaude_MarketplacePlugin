# SuperClaude Marketplace Structure

Complete structure of the SuperClaude Marketplace for Claude Code.

## Directory Tree

```
SuperClaude_MarketplacePlugin/
├── .claude-plugin/
│   └── marketplace.json              # Main marketplace manifest
│
├── plugins/
│   └── superclaude/
│       ├── .claude-plugin/
│       │   └── plugin.json           # Plugin manifest
│       ├── commands/
│       │   ├── agent.md              # PM Agent orchestrator
│       │   ├── research.md           # Deep research
│       │   └── index-repo.md         # Repository indexing
│       ├── agents/
│       │   ├── deep-research.md      # Research agent
│       │   ├── repo-index.md         # Indexing agent
│       │   └── self-review.md        # Review agent
│       ├── skills/
│       │   └── confidence-check/     # Confidence assessment skill
│       ├── hooks/
│       │   └── hooks.json            # SessionStart hook
│       └── scripts/
│           └── session-init.sh       # Initialization script
│
├── README.md                         # Full documentation
├── QUICKSTART.md                     # Quick start guide
├── MARKETPLACE_STRUCTURE.md          # This file
├── CHANGELOG.md                      # Version history
└── LICENSE                          # MIT License
```

## Plugin Summary

### Total Commands: 3

| Plugin | Commands | Agents | Skills | Hooks |
|--------|----------|--------|--------|-------|
| superclaude | 3 | 3 | 1 | 1 |

## Command Reference

### SuperClaude
- `/agent` - PM Agent orchestrator with confidence-driven workflow (≥90% threshold)
- `/research` - Deep research with adaptive planning and multi-hop reasoning
- `/index-repo` - Repository indexing for 94% token reduction (58K → 3K)

## Specialized Agents

### 1. deep-research
- **Focus**: Autonomous web research
- **Capabilities**: Adaptive planning, multi-hop reasoning (up to 5 iterations), quality scoring
- **MCP Integration**: Tavily (search), Context7 (documentation)

### 2. repo-index
- **Focus**: Repository structure analysis and file shortlisting
- **Capabilities**: Intelligent indexing, 94% token reduction, context optimization

### 3. self-review
- **Focus**: Post-implementation validation
- **Capabilities**: Evidence-based checks, reflexion, continuous learning across sessions

## Skills

### confidence-check
- **Type**: Pre-implementation assessment
- **Purpose**: Ensure ≥90% confidence before proceeding
- **ROI**: 25-250x token savings by preventing wrong-direction work

## Hooks

### SessionStart
- **Type**: Command
- **Script**: `./scripts/session-init.sh`
- **Purpose**: Auto-activate PM Agent orchestrator on session start
- **Timeout**: 10 seconds

## MCP Integrations

The SuperClaude plugin integrates with 8 MCP servers (optional):

1. **Tavily** - Web search and discovery
2. **Context7** - Official documentation lookup
3. **Serena** - Session persistence and memory (2-3x faster execution)
4. **Sequential** - Token-efficient reasoning (30-50% reduction)
5. **Mindbase** - Cross-session learning
6. **Playwright** - JavaScript-heavy content extraction
7. **Magic** - UI component generation
8. **Chrome DevTools** - Performance analysis

## Tech Stack Coverage

✅ Confidence-driven development (≥90% threshold)
✅ Autonomous web research with adaptive planning
✅ 94% token reduction through smart indexing
✅ Pre-implementation confidence assessment
✅ Post-implementation validation and reflexion
✅ Cross-session learning and memory
✅ MCP server integration for enhanced capabilities

## Performance

**Without MCPs**: Fully functional, standard performance ✅

**With MCPs**:
- 2-3x faster execution (Serena code understanding)
- 30-50% fewer tokens (Sequential reasoning)
- Enhanced research (Tavily + Context7)
- Cross-session learning (Mindbase)

## Files Created

- **1** Marketplace manifest (`.claude-plugin/marketplace.json`)
- **1** Plugin manifest (`plugins/superclaude/.claude-plugin/plugin.json`)
- **3** Command files
- **3** Agent definitions
- **1** Skill definition
- **1** Hook configuration
- **1** Initialization script
- **4** Documentation files (README.md, QUICKSTART.md, this file, CHANGELOG.md)

**Total: 15+ files** providing comprehensive development platform enhancement.

## Installation Size

Approximate sizes:
- Commands: ~10-15 KB total
- Agents: ~10-15 KB total
- Skills: ~5 KB total
- Manifests: ~10 KB total
- Documentation: ~30 KB total

**Total marketplace size: ~70-80 KB** (text files only, no dependencies)

## Maintenance

To update or add features:

1. Edit command/agent files in `plugins/superclaude/`
2. Update version in plugin manifest
3. Reinstall plugin in Claude Code
4. Test changes

## Version

- **Marketplace Version**: 4.1.6
- **Plugin Version**: 4.1.6
- **Created**: 2025-01-05
- **Author**: SuperClaude Community

## Requirements

- Claude Code ≥1.0.0
- Optional: MCP servers for enhanced performance (via [airis-mcp-gateway](https://github.com/agiletec-inc/airis-mcp-gateway))

---

**Ready to use!** Follow the [QUICKSTART.md](QUICKSTART.md) to get started.
