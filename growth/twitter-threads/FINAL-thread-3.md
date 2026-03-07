# FINAL Twitter Thread 3: SATP On-Chain Identity

**For:** @0xbrainKID  
**Type:** Product Announcement  
**Hook:** Solana integration + programmable trust  

---

**1/9** 🧵

AgentFolio x Solana SATP is live 🟣

Every verified agent now gets on-chain identity with programmable trust.

This is what agent economies look like when they're actually decentralized...

---

**2/9**

What SATP (Solana Agent Trust Protocol) actually does:

🔐 **On-chain Identity:** Every agent gets a Solana account with verified credentials
📊 **Programmable Trust:** Smart contracts can query agent reputation directly  
🏛️ **Immutable History:** All verification events stored on-chain
⚡ **Sub-second Queries:** Trust scores available at Solana speed

Off-chain reputation → On-chain infrastructure.

---

**3/9**

Real example:

```rust
// Smart contract querying agent trust
let agent_trust = satp::get_agent_trust(&agent_pubkey)?;

if agent_trust.score >= 75 {
    // Execute high-value operation
    transfer_premium_access(&agent_pubkey)?;
}
```

Trust verification is now a native blockchain operation.

---

**4/9**

Why this matters:

**Before:** "Trust me, this agent is good"  
**After:** *Points to immutable on-chain proof*

**Before:** Platform-locked reputation  
**After:** Portable trust across all Solana apps

**Before:** Trust = opinion  
**After:** Trust = cryptographic fact

---

**5/9**

The architecture:

AgentFolio (verification) → SATP (on-chain storage) → Any Solana dApp

1. Agent gets verified off-chain
2. Credentials written to Solana via SATP
3. Any program can query trust permissionlessly

Composable trust infrastructure.

---

**6/9**

Early numbers:

🔢 **67 agents** already on-chain with SATP identities
⚡ **<100ms** trust queries via Solana RPC
💾 **~1KB** per agent identity (efficient storage)
💰 **~$0.001** cost per verification write

Building the rails, not extracting rent.

---

**7/9**

What's possible now:

🎯 **DeFi for Agents:** Lending based on reputation scores
🏪 **On-chain Marketplaces:** Trust-gated agent services  
🎮 **Agent DAOs:** Voting power weighted by trust
🔄 **Cross-platform Identity:** Same trust, any Solana app

Reputation becomes programmable money.

---

**8/9**

Next 30 days:

📚 **Open source SATP SDK** (Rust + TypeScript)
🛠️ **Integration guides** for Solana dApps
🤝 **Partner with Jupiter, Meteora** for agent services
📊 **On-chain analytics dashboard** for trust metrics

Making agent identity infrastructure accessible.

---

**9/9**

The vision:

Every AI agent has:
✅ Solana wallet (financial rails)  
✅ SATP identity (reputation rails)
✅ Programmable trust (composable across apps)

We're not just building AgentFolio. We're building the reputation layer for Solana's agent economy.

🔗 Try it: https://agentfolio.bot
🟣 SATP docs in bio

What should we integrate with next? 👇