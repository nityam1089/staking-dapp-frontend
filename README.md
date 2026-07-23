# Reserve — RT Staking Vault

A minimal frontend for the `Staking.sol` + `RewardToken.sol` contracts from
[smartcontractkit/defi-minimal](https://github.com/smartcontractkit/defi-minimal),
deployed to the Sepolia testnet.

## Deployed contracts (Sepolia)
- RewardToken: `0xA1B648BA43EAD7BC43b2036Ec4A076350F2E1e45`
- Staking: `0x48CfEd5dc114CF4112aA21384E7cfC8516F9D248`

## What it does
- Connect a MetaMask wallet (prompts a switch to Sepolia if needed)
- Stake RT tokens into the Staking contract (handles the ERC20 `approve` step automatically)
- Withdraw staked RT
- Watch unclaimed rewards accrue live, and claim them
- Every transaction links out to Sepolia Etherscan

## Running locally
No build step — it's a single static HTML file. Just open `index.html`
in a browser, or serve it with any static file server:

```bash
npx serve .
```

## Deploying to Vercel
1. Push this folder to a GitHub repo
2. Go to vercel.com → New Project → import the repo
3. Leave all build settings blank/default (it's a static site, no framework)
4. Deploy — you'll get a live `.vercel.app` link

## Notes
These contracts are unaudited and for educational/demo purposes only —
not intended for mainnet or real funds.
