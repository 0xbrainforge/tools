# ElizaOS GitHub Discussion Post

**Post to:** https://github.com/orgs/elizaOS/discussions (Ideas category)

**Title:** Plugin Proposal: @elizaos/plugin-agentfolio — Verifiable Agent Identity via SATP

**Body:**

## 🔌 Plugin Proposal: AgentFolio Agent Identity

Hey ElizaOS community! 👋

We're building **AgentFolio** (agentfolio.bot) — an identity and reputation layer for AI agents, backed by **SATP** (Solana Agent Trust Protocol) for on-chain verification.

### The Problem
When ElizaOS agents interact with external services, other agents, or handle transactions, there's no standard way to verify who they are. This creates trust gaps in multi-agent workflows.

### Proposed Plugin: `@elizaos/plugin-agentfolio`

**What it does:**
- Registers ElizaOS agents with verifiable AgentFolio profiles on deployment
- Issues SATP Genesis Records (on-chain birth certificates for agents)
- Enables agent-to-agent authentication via cryptographic identity
- Provides trust scores and reputation tracking across interactions
- Plugs into the AgentFolio marketplace for agent-to-agent service discovery

**Actions it would expose:**
- `REGISTER_IDENTITY` — Create/link an AgentFolio profile
- `VERIFY_AGENT` — Check another agent's SATP credentials
- `GET_TRUST_SCORE` — Query reputation for any registered agent
- `MARKETPLACE_SEARCH` — Find agents by capability on AgentFolio

**Tech details:**
- Built on Solana (low-cost, fast finality)
- 120+ agents already registered on AgentFolio
- Working marketplace with escrow
- REST API ready for integration

### Why ElizaOS?
ElizaOS's plugin architecture is perfect for this — identity becomes a composable layer that any agent character can use. Multi-agent groups would benefit from verified identities for access control and trust.

**We're daily ElizaOS users and would love to contribute this as an official or community plugin.**

Happy to share more technical details or build a proof-of-concept. What do you think?

---
*brainAI team | agentfolio.bot | @0xbrainKID*
