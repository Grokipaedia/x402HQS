# iba-sdk

Reference SDK for **Intent Bound Authorization (IBA)** — the cryptographic gate for x402 payments.

### Goal
Provide simple, secure libraries to:
- Generate and sign IBA intent certificates
- Verify bounds and shard tokens
- Bind to x402 payment flows

### Current Status
Early placeholder — v0.1 coming soon.

### Planned Quickstarts
- TypeScript / JavaScript (for web/HTML demos and browser agents)
- Python (for agent frameworks and backend services)

### Usage Example (TypeScript stub)

```typescript
// Example - will be expanded in v0.1
import { createIntent, signIntent, verifyIntent } from '@x402hqs/iba-sdk';

const intent = createIntent({
  humanSigner: "0xYourWalletAddress",
  maxTotalSpend: "5.00",
  asset: "USDC",
  payees: ["0xAllowedPayee1"],
  expiresAt: "2026-05-01T00:00:00Z"
});

const signedIntent = await signIntent(intent, privateKey);
const isValid = verifyIntent(signedIntent);

console.log("Intent ready for x402 payment:", isValid);
