---
label: Token Program
order: 700
---

# Token Program

In the base level, there are only 2 mains concept which we need to pay attention to: `Mint` and `TokenAccount`

### Mint (token type): eg: USDC, SOL, BTC

- authority: PK, who can mint more tokens
- supply: u64, total ciruclation

### TokenAccount: user metadata, refers to the amount of paticular mint that user has access to.

- amount: u64, amount user has
- owner: PK, needs to sign for amount changes
- mint: PK

When working with tokens, there a few operations we need to support:

### Transfer

### Burn

### Mint