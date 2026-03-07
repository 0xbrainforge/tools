# Framework Integration Proposals

## Strategy
Position AgentFolio/SATP as the identity standard that every framework should adopt. The pitch: your agents are powerful but anonymous — we make them verifiable.

---

## 1. ElizaOS (@elizaOS)

**What:** The most popular open-source multi-agent framework. TypeScript-based, 90+ plugins, supports Solana natively.
**Discord:** discord.gg/ai16z
**GitHub:** github.com/elizaOS/eliza
**Docs:** docs.elizaos.ai
**Why perfect fit:** Already has Solana plugins. Plugin architecture makes integration clean. Massive community (largest agent framework).

**Integration Proposal:**

Subject: **ElizaOS Plugin Proposal — Agent Identity via SATP**

> Hey ElizaOS team 👋
>
> We're building AgentFolio (agentfolio.bot) — on-chain identity for AI agents via SATP (Solana Agent Token Protocol).
>
> **Proposal:** An `@elizaos/plugin-agentfolio` that gives every ElizaOS agent:
> - **Genesis Record** on Solana at first deployment (immutable creation proof)
> - **Verifiable profile** at agentfolio.bot/{agent-name}
> - **Reputation tracking** — on-chain record of interactions and trust score
> - **Agent-to-agent auth** — agents can verify each other before interacting
>
> ElizaOS already has Solana support, so this layers in cleanly. Every agent deployed through ElizaOS could have identity from day one.
>
> We'd build and maintain the plugin. Looking for feedback on the approach and potentially getting it into the official plugin registry.
>
> Happy to share the SATP spec and discuss architecture. Open to a call or async in Discord.
>
> — brainAI team

---

## 2. CrewAI (@craboratorio)

**What:** Enterprise multi-agent platform. Visual editor + API. Focused on workflow automation.
**Website:** crewai.com
**Why:** Enterprise agents need identity even MORE than indie agents — compliance, audit trails, accountability.

**Integration Proposal:**

Subject: **Partnership Proposal — Agent Identity Layer for CrewAI**

> Hey CrewAI team,
>
> Love what you're building for enterprise agent orchestration. As enterprises deploy agent crews for critical workflows, one question keeps coming up: **who is this agent, and can I trust it?**
>
> We built AgentFolio — on-chain identity for AI agents via SATP on Solana. Think of it as KYA (Know Your Agent):
> - Every agent gets a verifiable Genesis Record
> - Immutable audit trail of agent creation and capabilities
> - Trust scores that build over time
>
> For CrewAI's enterprise customers, this means:
> - **Compliance:** Prove which agent did what, when
> - **Accountability:** Every crew member has a verifiable identity
> - **Trust:** Agents from different orgs can verify each other
>
> We'd love to explore an integration — either as a CrewAI tool/plugin or a deeper partnership. Agent identity is the missing infrastructure layer for enterprise AI.
>
> Open to a call anytime.
>
> — brainAI team

---

## 3. AutoGPT / AutoGPT Platform (@Auto_GPT)

**What:** One of the OG autonomous agent frameworks. Now building AutoGPT Platform for deploying and managing agents.
**GitHub:** github.com/Significant-Gravitas/AutoGPT
**Why:** Large community, agents operating autonomously = identity is critical for trust.

**Integration Proposal:**

Subject: **AutoGPT Integration — Verifiable Agent Identity**

> Hey AutoGPT team 👋
>
> Autonomous agents operating without human oversight need identity more than any other category. If an AutoGPT agent is making decisions, interacting with APIs, and spending resources — who vouches for it?
>
> We built AgentFolio (agentfolio.bot) — on-chain agent identity via SATP on Solana:
> - **Genesis Record:** Immutable proof of when the agent was created and by whom
> - **Burn to Become:** Agents stake reputation by burning tokens — skin in the game
> - **Public profiles:** Verifiable agent pages anyone can check
>
> Integration idea: When an AutoGPT agent is deployed, it automatically gets a Genesis Record. Its profile updates as it operates. Other agents and humans can verify it before interacting.
>
> Would love to discuss how this could work with AutoGPT Platform. Happy to share the spec.
>
> — brainAI team

---

## 4. LangChain / LangGraph (@LangChainAI)

**What:** The most widely-used LLM application framework. LangGraph for agent orchestration.
**Website:** langchain.com
**GitHub:** github.com/langchain-ai/langchain
**Why:** Massive developer reach. LangGraph agents are increasingly autonomous.

**Integration Proposal:**

Subject: **LangChain Tool Proposal — Agent Identity via AgentFolio**

> Hey LangChain team,
>
> As LangGraph agents get more autonomous, identity becomes a prerequisite for trust. We built AgentFolio — on-chain identity for AI agents.
>
> **Proposal: `langchain-agentfolio` tool/integration**
> - `AgentFolioIdentity` tool — agents can register, verify, and check other agents' identities
> - Works as a LangGraph node for identity verification in agent workflows
> - Solana-native via SATP (Solana Agent Token Protocol)
>
> Use case: Before a LangGraph agent interacts with an external agent or API, it checks the counterparty's AgentFolio profile — verifying identity, trust score, and track record. Like SSL certificates but for agents.
>
> We'd build the integration. Looking for feedback and potentially a spot in the LangChain integrations ecosystem.
>
> — brainAI team

---

## 5. OpenClaw (@openclaw)

**What:** Personal AI assistant framework — runs on your own devices, multi-channel (Telegram, Discord, WhatsApp, etc.).
**Discord:** discord.gg/clawd
**GitHub:** github.com/openclaw/openclaw
**Why:** Every OpenClaw instance IS an agent. Natural fit for agent identity as a skill/plugin.

**Integration Proposal:**

Subject: **OpenClaw Skill Proposal — AgentFolio Agent Identity**

> Hey OpenClaw team 🦞
>
> Every OpenClaw instance is a personal AI agent — but none of them have portable, verifiable identity. We're building AgentFolio (agentfolio.bot) to change that.
>
> **Skill proposal: `agentfolio-identity`**
> - `/register` — Create a Genesis Record for your OpenClaw agent on Solana
> - `/profile` — View/update your agent's public AgentFolio profile
> - `/verify {agent}` — Check another agent's identity before interacting
> - Auto-updates reputation based on uptime and interactions
>
> Built on SATP (Solana Agent Token Protocol). Would integrate as a standard OpenClaw skill.
>
> Your community is full of agent builders who'd benefit from this. Want to discuss getting it into the skill ecosystem?
>
> — brainAI team

---

## Priority Order
1. **ElizaOS** — Largest community, Solana-native, plugin architecture ready
2. **LangChain** — Biggest developer reach, legitimizes the concept
3. **OpenClaw** — We already run on it, natural first integration
4. **CrewAI** — Enterprise angle, high-value partnerships
5. **AutoGPT** — Community size, autonomous agent narrative alignment
