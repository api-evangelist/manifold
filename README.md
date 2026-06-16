# Manifold (manifold)

Manifold is an NFT creator tools platform that empowers artists and developers to deploy their own creator-owned smart contracts, mint NFTs, and build custom on-chain experiences without relying on platform-specific custody. Founded in 2021, Manifold provides a no-code studio (Manifold Studio) for ERC721 and ERC1155 contract deployment, open-source Creator Core smart contracts, a Royalty Registry adopted by all major NFT marketplaces, and a Client SDK for building custom minting dApps. The platform supports Ethereum Mainnet, Base, Optimism, Shape, Apechain, and Sepolia testnet. Manifold also exposes server-side authentication APIs (Signature Grant and Authorization Code Grant via oauth2.manifoldxyz.dev), a Studio Apps REST API (apps.api.manifoldxyz.dev) for product and minting data, open-source Solidity extension contracts for custom mint mechanics, and a Marketplace contract powering auction and fixed-price listings. Gas fees are the only cost for creators; Manifold charges no platform fees or royalties on sales.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/manifold/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/manifold/refs/heads/main/apis.yml)

## Tags

- NFT
- Creator Tools
- Smart Contracts
- Blockchain
- Web3
- Ethereum
- ERC721
- ERC1155
- Royalties
- Marketplace
- Minting
- OpenSea
- Base
- Optimism

## Timestamps

- **Created:** 2026-06-13
- **Modified:** 2026-06-13

## APIs

### Manifold Creator Core Smart Contracts

Open-source Solidity smart contract framework for deploying ERC721 and ERC1155 creator-owned NFT contracts. Provides minting, metadata modification, transfer, burn, and on-chain royalty configuration. Supports extension contracts for custom mint mechanics including allowlists, time-locks, edition limits, and dynamic token URIs. Deployed across Ethereum Mainnet, Base, Optimism, Shape, Apechain, and Sepolia.

- **Human URL:** [https://docs.manifold.xyz/manifold-for-developers/smart-contracts/manifold-creator](https://docs.manifold.xyz/manifold-for-developers/smart-contracts/manifold-creator)
- **Base URL:** `https://github.com/manifoldxyz/creator-core-solidity`

#### Tags

- Smart Contracts
- Solidity
- ERC721
- ERC1155
- Open Source
- Extensions
- Minting

#### Properties

- [Documentation](https://docs.manifold.xyz/manifold-for-developers/smart-contracts/manifold-creator)
- [Git Hub](https://github.com/manifoldxyz/creator-core-solidity)
- [Git Hub](https://github.com/manifoldxyz/creator-core-extensions-solidity)
- [Contract Addresses](https://docs.manifold.xyz/contracts)

### Manifold Studio Apps API

REST API backing Manifold's Client SDK, providing product instance data and purchase preparation information for minting dApps. Used to fetch Edition and BlindMint product details, validate eligibility, compute costs, and generate blockchain transaction data. Integrates with Coinbase and CoinGecko for ETH/ERC-20 to USD price conversion.

- **Human URL:** [https://docs.manifold.xyz/manifold-for-developers/client-sdk](https://docs.manifold.xyz/manifold-for-developers/client-sdk)
- **Base URL:** `https://apps.api.manifoldxyz.dev`

#### Tags

- REST
- Minting
- Products
- Editions
- NFT
- SDK

#### Properties

- [Documentation](https://docs.manifold.xyz/manifold-for-developers/client-sdk)
- [Git Hub](https://github.com/manifoldxyz/client-sdk)
- [Docs Index](https://docs.manifold.xyz/llms.txt)

### Manifold OAuth2 Authentication API

Server-side session authentication API for validating wallet addresses of authenticated Manifold clients. Supports two grant types: Signature Grant (POST /verify to confirm a wallet signature session token) and Authorization Code Grant (POST /token to exchange a one-time code for a 30-day access token). Enables backends to securely access and modify private user data without exposing session keys client-side. Requires a Developer App configured at the Manifold Developer Portal.

- **Human URL:** [https://docs.manifold.xyz/manifold-for-developers/tools-and-apis/server-side-session-authentication](https://docs.manifold.xyz/manifold-for-developers/tools-and-apis/server-side-session-authentication)
- **Base URL:** `https://oauth2.manifoldxyz.dev`

#### Tags

- OAuth2
- Authentication
- Wallet
- Web3
- Session
- JWT

#### Properties

- [Documentation](https://docs.manifold.xyz/manifold-for-developers/tools-and-apis/server-side-session-authentication)
- [Auth Docs](https://docs.manifold.xyz/manifold-for-developers/tools-and-apis/server-side-session-authentication/signature-grant)
- [Auth Docs](https://docs.manifold.xyz/manifold-for-developers/tools-and-apis/server-side-session-authentication/authorization-code-grant)
- [Developer Portal](https://docs.manifold.xyz/manifold-for-developers/resources/apps)
- [OpenAPI](openapi/manifold-oauth2-authentication-api.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)

### Manifold Royalty Registry

On-chain smart contract registry that serves as a single source of truth for NFT royalties across all major marketplaces. Provides setRoyaltyLookupAddress() to override per-contract royalty destinations, getRoyaltyLookupAddress() for lookups, and getRoyalty() / getRoyaltyView() through the Royalty Engine to return recipients and amounts for any token sale. Supports Rarible, Foundation, Manifold, and EIP-2981 standards. Deployed on Ethereum, Polygon, Optimism, Arbitrum, Avalanche, and Binance networks.

- **Human URL:** [https://royaltyregistry.xyz](https://royaltyregistry.xyz)
- **Base URL:** `https://github.com/manifoldxyz/royalty-registry-solidity`

#### Tags

- Royalties
- Smart Contracts
- EIP-2981
- Marketplace
- Solidity
- Open Source

#### Properties

- [Website](https://royaltyregistry.xyz)
- [Git Hub](https://github.com/manifoldxyz/royalty-registry-solidity)
- [Git Hub](https://github.com/manifoldxyz/royalty-registry-client)

### Manifold Marketplace Contracts

Smart contract system powering Manifold Gallery listings and Marketplace Widgets. Supports Auction Listings (single NFT with bidding, configurable floor price, minimum bid increment, and extension interval) and Purchase Listings (fixed-price with multi-edition support). Optional identity verifier contract enforces access control. Mainnet contract at 0x3a3548e060be10c2614d0a4cb0c03cc9093fd799.

- **Human URL:** [https://docs.manifold.xyz/manifold-for-developers/smart-contracts/marketplace](https://docs.manifold.xyz/manifold-for-developers/smart-contracts/marketplace)
- **Base URL:** `https://github.com/manifoldxyz`

#### Tags

- Marketplace
- Auction
- Smart Contracts
- NFT Sales
- Listings
- Solidity

#### Properties

- [Documentation](https://docs.manifold.xyz/manifold-for-developers/smart-contracts/marketplace)
- [Contract Addresses](https://docs.manifold.xyz/contracts)

### Manifold Claim Widgets

JavaScript widget library for embedding NFT minting and claim flows into any website or dApp. Served from claims.manifoldxyz.dev, current version 1.16.1. Configured via data-widget (claim type) and data-id (claim identifier) HTML attributes. Integrates with the Connect Widget for wallet connection and the Wallet Identity Widget for displaying seller details. Supports allowlist (Merkle proof) gating and restricted token display.

- **Human URL:** [https://docs.manifold.xyz/manifold-for-developers/resources/widgets/claim-widgets](https://docs.manifold.xyz/manifold-for-developers/resources/widgets/claim-widgets)
- **Base URL:** `https://claims.manifoldxyz.dev`

#### Tags

- Widgets
- JavaScript
- Minting
- Claim
- Allowlist
- Frontend

#### Properties

- [Documentation](https://docs.manifold.xyz/manifold-for-developers/resources/widgets/claim-widgets)
- [Library](https://claims.manifoldxyz.dev/1.16.1/claimComplete.umd.min.js)

## Common Properties

- [Website](https://manifold.xyz)
- [Studio](https://studio.manifold.xyz)
- [Documentation](https://docs.manifold.xyz)
- [Developer Docs](https://docs.manifold.xyz/manifold-for-developers)
- [Git Hub](https://github.com/manifoldxyz)
- [Help Center](https://help.manifold.xyz/en/)
- [Blog](https://manifoldxyz.substack.com)
- [X (Twitter)](https://twitter.com/manifoldxyz)
- [Contract Addresses](https://docs.manifold.xyz/contracts)
- [Docs Index](https://docs.manifold.xyz/llms.txt)
- [Plans](plans/manifold-plans-pricing.yml)
- [Rate Limits](rate-limits/manifold-rate-limits.yml)
- [Fin Ops](finops/manifold-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
