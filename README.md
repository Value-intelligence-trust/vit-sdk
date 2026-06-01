# VIT SDK

**Official TypeScript/JavaScript SDK for the VIT Network API.**

[![npm](https://img.shields.io/badge/npm-vit--network--sdk-red?style=flat-square)](https://npmjs.com)
[![TypeScript](https://img.shields.io/badge/TypeScript-strict-blue?style=flat-square&logo=typescript)](https://typescriptlang.org)

## Install

```bash
npm install vit-network-sdk
```

## Quick Start

```typescript
import { VITClient } from 'vit-network-sdk';

const client = new VITClient({ apiKey: 'your-key' });

// Get AI prediction for a match
const prediction = await client.predictions.get({ matchId: 'EPL_2026_001' });
console.log(prediction.vitScore, prediction.confidence);

// Check wallet balance
const balance = await client.wallet.balance();
```

## Modules

- `client.predictions` — AI match predictions and VIT scores
- `client.wallet` — Multi-currency balances and transfers
- `client.marketplace` — Signal listing and subscription
- `client.blockchain` — VITCoin, DID, and oracle interactions
- `client.agents` — Agent swarm status and intelligence feeds
