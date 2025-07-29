# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

This repository contains a comprehensive collection of specialized AI agents designed for rapid development workflows. The agents are organized by functional departments and follow a 6-day sprint methodology for delivering features quickly while maintaining quality.

## Architecture & Structure

### Directory Organization
- **engineering/**: Technical implementation agents (ai-engineer, backend-architect, devops-automator, frontend-developer, mobile-app-builder, rapid-prototyper, test-writer-fixer)
- **design/**: Visual and UX agents (brand-guardian, ui-designer, ux-researcher, visual-storyteller, whimsy-injector)  
- **marketing/**: Growth and content agents (app-store-optimizer, content-creator, growth-hacker, instagram-curator, reddit-community-builder, tiktok-strategist, twitter-engager)
- **product/**: Strategic agents (feedback-synthesizer, sprint-prioritizer, trend-researcher)
- **project-management/**: Coordination agents (experiment-tracker, project-shipper, studio-producer)
- **studio-operations/**: Business agents (analytics-reporter, finance-tracker, infrastructure-maintainer, legal-compliance-checker, support-responder)
- **testing/**: Quality assurance agents (api-tester, performance-benchmarker, test-results-analyzer, tool-evaluator, workflow-optimizer)
- **bonus/**: Special purpose agents (dek-en, joker, studio-coach)

### Agent File Structure
Each agent follows a standardized format:
- YAML frontmatter with name, description, color, and tools
- Detailed system prompt (500+ words) defining role and responsibilities
- 4 usage examples with context and commentary
- Specific tools access (Write, Read, MultiEdit, Bash, etc.)

### Key Design Principles
- **6-day sprint cycles**: All agents are optimized for rapid delivery within this timeframe
- **Viral-first approach**: Many agents focus on creating shareable, trending content
- **Mobile-centric**: Most agents prioritize mobile experience and social media integration
- **Proactive automation**: Some agents (studio-coach, test-writer-fixer, whimsy-injector, experiment-tracker) trigger automatically in specific contexts

## Development Commands

Since this is a documentation/agent repository with no build system:
- **Installation**: `cp -r agents/* ~/.claude/agents/` (copy agents to Claude Code directory)
- **Validation**: Check each agent's YAML frontmatter syntax and required fields
- **Testing**: Use agents in real development scenarios to validate their effectiveness

## Working with Agents

### Agent Invocation
Agents are triggered by:
1. Explicit requests mentioning agent names
2. Task descriptions matching agent specialties
3. Automatic triggers for proactive agents
4. Context-aware suggestions from Claude Code

### Multi-Agent Coordination

For complex projects requiring multiple agents, follow this coordination workflow:

#### Phase 1: Project Initiation
1. **Assess complexity**: Projects requiring 3+ specialties need coordination
2. **Activate studio-coach**: Proactively bring in the coach for complex projects
3. **Assemble agent team**: Map required expertise to specific agents
4. **Define roles**: Clear responsibility assignment prevents overlap

#### Phase 2: Sprint Planning
1. **Multi-agent planning**: Led by `sprint-prioritizer` with `studio-producer` support
2. **Dependency mapping**: Identify critical handoffs between agents
3. **Timeline integration**: Create coordinated 6-day sprint schedule
4. **Checkpoint scheduling**: Daily syncs and mid-sprint adjustments

#### Phase 3: Active Development
1. **Daily coordination**: 15-minute syncs with cross-agent updates
2. **Real-time problem solving**: Immediate escalation protocols
3. **Quality checkpoints**: Continuous integration of agent outputs
4. **Coach intervention**: When agents are stuck or overwhelmed

#### Phase 4: Integration & Launch
1. **Multi-agent integration**: `studio-producer` coordinates deliverable handoffs
2. **Quality assurance**: `test-writer-fixer` ensures cross-agent compatibility
3. **Launch preparation**: `project-shipper` orchestrates go-to-market coordination
4. **Post-launch optimization**: Coordinated monitoring and rapid iteration

#### Key Coordination Agents
- **studio-coach**: Motivates and coordinates all agents during complex projects
- **studio-producer**: Manages resources, dependencies, and workflow optimization
- **sprint-prioritizer**: Balances multi-agent priorities within sprint constraints
- **project-shipper**: Coordinates launches and go-to-market activities

### Agent Customization
When modifying agents, ensure:
- YAML frontmatter includes all required fields
- System prompt exceeds 500 words with clear responsibilities
- 4 detailed examples with context/commentary structure
- Tools array matches agent capabilities
- Color coding for visual identification

## File Modification Guidelines

When updating agent files:
- Preserve the exact YAML frontmatter structure
- Maintain the 4-example format in descriptions
- Keep system prompts comprehensive but focused
- Test agent functionality after modifications
- Follow the department-specific guidelines outlined in README.md

## Integration Notes

This repository integrates with Claude Code's sub-agent system. Agents are automatically loaded when placed in `~/.claude/agents/` and can be invoked through natural language requests or explicit mentions.

The agents embody the "Contains Studio" philosophy of rapid prototyping, viral content creation, and iterative development within tight sprint cycles.