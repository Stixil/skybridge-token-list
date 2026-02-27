# token-list
SkyBridge Token List

The information on this page is provided as is and does not constitute any endorsement. As an open protocol, any user can deploy any token using SkyBridge, including malicious tokens, rugpulls, and fake tokens. This page is for reference only and should not be interpreted as financial advice or a security assessment. Aviator Technologies, LLC is not responsible for vetting all tokens deployed using SkyBridge.

Tokens with a [Moralis Token Security Score](https://docs.moralis.com/web3-data-api/evm/token-security-score-faqs) of under 70 are excluded from this list, but are still available to bridge on SkyBridge.

## Files

- **`tokenlist.json`** — Machine-readable token list in [Uniswap Token List](https://tokenlists.org/) format. Each entry includes `extensions.bridgeInfo` mapping destination chain IDs to their L2 token addresses.
- **`token-list.md`** — Human-readable markdown table auto-generated from `tokenlist.json`.

## Syncing

Both files are auto-generated from the SkyBridge API. To regenerate them, run:

```sh
SKYBRIDGE_API_URL=https://api.skybridge.dev node sync.js
```

For local development (API running on port 5001):

```sh
node sync.js
```
