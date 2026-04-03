# x402HQS — High Quality Standards for x402 + IBA

**Safe Agentic Payments Stack**

- **x402**: The open payment rail (HTTP 402) — see official [coinbase/x402](https://github.com/coinbase/x402)
- **IBA (Intent Bound Authorization)**: The cryptographic gate — signed intent certificates with hard bounds, payee lists, spend caps, and shard token delegation
- **WitnessBound**: Immutable audit records (SHA3-256 + blockchain anchor)

### Why this repo?
This is the governance & safety layer on top of x402. It answers: "What did the human actually authorize the agent to pay?"

Live HTML demos (no login needed):
- Core x402 + IBA: https://aipayhq.com/402-html/
- Full MCP + x402 + IBA: https://aipayhq.com/triple-html/
- Shard tokens (sub-agent delegation): https://intentbound.com/shard-html/
- Voice agents: https://aipayhq.com/voice-html/
- Quantum defense & trading floor: See x402hqs.com/x402-html/

### What's coming next (v0.1 soon)
- IBA spec (intent certificate format, shard tokens, WitnessBound integration)
- Simple SDK starters (TypeScript for web/HTML, Python for agents)
- Example code from the live demos
- Tools: certificate generator + budget simulator

Patent pending: GB2603013.0  
IETF draft: draft-williams-intent-token-00  
Contact: IBA@intentbound.com

Built for developers who want agentic commerce that is **safe by default**.
