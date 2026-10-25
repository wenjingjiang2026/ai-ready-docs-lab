# Getting started (sample)

Install the SDK, then make one successful call.

## Install

```bash
npm install @example/sdk
```

## First call

```ts
import { Client } from "@example/sdk";
const client = new Client({ apiKey: process.env.API_KEY });
const result = await client.chat({ model: "demo", messages: [{ role: "user", content: "hi" }] });
console.log(result);
```

## Pitfalls

- Wrong cluster / base URL → auth succeeds but calls fail.
- Stale model id → 404 after catalog refresh.
