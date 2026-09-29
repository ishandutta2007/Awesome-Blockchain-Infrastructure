# Awesome-Blockchain-Infrastructure

## Top Blockchain Infrastructure Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on RPC Access, Node Deployment & Multi-Chain Infrastructure*  

**Last updated: September 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Blockchain Infrastructure**. These tools provide RPC access, node deployment, indexing, and infrastructure management for developers building on Ethereum, Solana, Bitcoin, and other blockchain networks without running their own nodes.



**Examples** include Alchemy, Infura, QuickNode, Ankr, Chainstack, Tatum, Moralis, GetBlock, Blockdaemon, and NOWNodes (the category leaders).



**Open-source emphasis**: This section is expanded with active projects for self-hosting, custom node deployments, and transparent infrastructure management — ideal for developers, node operators, and infrastructure teams building vendor-independent blockchain access. The open-source ecosystem for node clients and RPC proxies is notably mature, with production-grade implementations available for every major blockchain.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-hosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



| Platform | Description | Starting Paid Tier | Free Tier / Free Trial Limit |
|---|---|---|---|
| **[Alchemy](https://www.alchemy.com/)** | Web3 development platform providing RPC access plus enhanced APIs, Notify, and developer tooling across Ethereum and multi-chain networks. | $49/month (Growth Tier) or $0.525 / 1M Compute Units (PAYG) | 30,000,000 Compute Units (CUs)/month (300 CUPS throughput) |
| **[Infura](https://www.infura.io/)** | Consensys-owned Ethereum RPC provider & MetaMask default backend supporting 20+ EVM networks. | $50/month (Developer Plan, 15M credits/day) | 3,000,000 credits/day (~100,000 requests/day, 2,000 credits/sec rate limit) |
| **[QuickNode](https://www.quicknode.com/)** | High-performance multi-chain RPC infrastructure platform supporting 80+ blockchain protocols. | $49/month (Build Plan, 80M credits) | 10,000,000 API Credits/month (15 RPS throughput limit) |
| **[Ankr](https://www.ankr.com/)** | DePIN-based multi-chain RPC infrastructure with globally distributed node network. | $10 for 100M credits (PAYG) or $500/month (Subscription) | 200,000,000 API Credits/month (Public RPC available without signup) |
| **[Chainstack](https://chainstack.com/)** | Multi-chain protocol platform supporting 70+ chains with Hybrid Cloud and dedicated node deployments. | $49/month (Growth Plan, 20M Request Units) | 3,000,000 Request Units (RUs)/month (25 RPS rate limit) |
| **[Tatum](https://tatum.io/)** | Enterprise Web3 infrastructure platform combining RPC endpoints, Wallet SDK, and Data APIs. | $25/month (Starter Plan, 4M credits/month) | 100,000 lifetime credits (3 RPS rate limit) |
| **[Moralis](https://moralis.io/)** | Structured, real-time Web3 data APIs & RPC endpoints across 40+ EVM chains and Solana. | $149/month (Starter Plan, 2M Compute Units/month) | 40,000 Compute Units/day (~1,200,000 CUs/month, 1,000 CU/s rate limit) |
| **[GetBlock](https://getblock.io/)** | Web3 RPC node provider offering JSON-RPC and WebSocket endpoints across 130+ blockchains. | $39/month (Starter Plan, 90M CUs/month) | 50,000 Compute Units/day (~1,500,000 CUs/month, 20 RPS limit) |
| **[Blockdaemon](https://www.blockdaemon.com/)** | Enterprise-grade blockchain node infrastructure, staking API, and institutional access. | Quote-based by sales (Starter tier includes 65M CUs/month) | 3,000,000 Compute Units/month (5 RPS rate limit, 1 Test Key) |
| **[NOWNodes](https://nownodes.io/)** | Node provider offering cost-effective shared and dedicated RPC access to multi-chain nodes. | €20/month (~$22/month starting shared plan) | 100,000 RPC requests/month (1 API key included) |



## Open-Source GitHub Projects



- **[Reth](https://github.com/paradigmxyz/reth)**  

  Modular, high-performance Ethereum execution layer client written in Rust. Functions as a production binary for running nodes or as an SDK for building custom Ethereum-compatible nodes. Used by Coinbase's Base L2, Berachain, Gnosis Chain, and Binance Smart Chain for their execution clients . Supports JSON-RPC with `eth` and `trace` APIs. Apache 2.0 licensed.



- **[Forest (Filecoin)](https://github.com/ChainSafe/forest)**  

  Rust implementation of the Filecoin protocol providing a lightweight, high-performance alternative to Lotus. Only implementation with fast snapshot generation (10x faster, ~88% less RAM, ~56% less disk). Provides exclusive RPC methods (`debug_traceTransaction`, `trace_call`) and is the sole source of client diversity for Filecoin (Lotus and Venus are both Go) . Powers 2 of 4 bootstrap nodes on mainnet and calibnet.



- **[proxyd](https://github.com/ethereum-optimism/infra)**  

  Fault-tolerant RPC proxy and load balancer for Ethereum and EVM-compatible chains, maintained by Optimism. Features backend health probing inspired by Kubernetes liveness/readiness probes, configurable success/failure thresholds, and passive transaction UX monitoring . Supports translation to Alchemy, Parity, and standard Ethereum receipt methods.



- **[nodecore](https://github.com/drpcorg/nodecore)**  

  Fault-tolerant, API-agnostic RPC load balancer for blockchain APIs. Supports JSON-RPC, WebSocket, REST, and gRPC interfaces across EVM, Solana, Algorand, Aztec, Aptos, Bitcoin, NEAR, Starknet, TON, Cosmos SDK, Polkadot/Substrate, Stellar, Sui, Celestia, and Beacon Chain . Features intelligent routing based on real-time performance metrics, caching, request hedging, quorum verification, and flexible authentication.



- **[rpcgate](https://github.com/BinaryArchaism/rpcgate)**  

  Self-hosted open-source proxy and load balancer for EVM RPC providers. Increases reliability and provides unified access across chains with metrics for observability . Features multi-chain configuration, multi-provider balancing (p2cewma adaptive, round-robin, least-connection), client tracking via Basic Auth or query parameters, and an official Grafana dashboard.



- **[Rindexer](https://github.com/joshstevens19/rindexer)**  

  High-performance EVM indexer written in Rust with 474+ events/s throughput. Ranked #3 in open indexer benchmarks behind Envio (HyperSync) and Squid SDK (SQD Network) . Uses RPC for data ingestion with Postgres storage.



- **[Ponder](https://github.com/ponder-sh/ponder)**  

  Open-source TypeScript-based EVM indexer. Benchmarked at 65 events/s (state aggregation) and 230 events/s (decoded event stream) — slower than Rust alternatives but developer-friendly . Uses RPC for data ingestion.



- **[SubQuery](https://github.com/subquery/subql)**  

  Open-source blockchain indexer with support for multiple chains. Benchmarked at 31 events/s (state aggregation) and 36 events/s (decoded event stream) .



- **[evm-indexer (eabz)](https://github.com/eabz/evm-indexer)**  

  Scalable SQL indexer for EVM-compatible blockchains with 86+ stars. Alternative to Ponder and SubQuery for teams preferring SQL-first indexing approaches .



- **[tzkt](https://github.com/baking-bad/tzkt)**  

  Awesome Tezos blockchain indexer and API with 184+ stars. C# based, providing comprehensive indexing for the Tezos ecosystem .



- **[barreleye](https://github.com/barreleye/barreleye)**  

  Open-source blockchain indexer and explorer written in Rust. Lightweight alternative for teams building custom indexing solutions .



- **[chaindexing-ts](https://github.com/chaindexing/chaindexing-ts)**  

  Index any EVM chain and query in SQL. TypeScript-based indexer for teams wanting SQL query capabilities .



### Additional Strong Open-Source Options



- **Squid SDK** — Open-source indexing framework with SQD Network support, benchmarked at 705 events/s (state aggregation) .

- **Subgraph** — The Graph's indexing protocol, benchmarked at 40 events/s (state aggregation) and 158 events/s (decoded event stream) .

- **Chia Blockchain** — Full blockchain node, farmer, harvester, timelord, and wallet in Python with GUI and CLI interfaces .

- **Blockroma** — Open-source blockchain explorer built with TypeScript for Ethereum web3 compatible blockchains .



**Frameworks for building custom blockchain infrastructure**: Combine **Reth** for high-performance Ethereum execution, **proxyd** or **nodecore** for RPC load balancing and failover, and **Rindexer** or **Ponder** for indexing. For enterprise deployments, **Tatum** provides MPC wallets, data APIs, and notifications with SOC 2 and ISO 27001 compliance . For AI-powered agents, **Moralis Onchain Skills** enables direct blockchain queries from Claude Code, Cursor, and other AI tools .



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- Blockchain infrastructure requires significant operational expertise including networking, storage management, and security hardening.

- Self-hosted open-source solutions require proper infrastructure, monitoring, and ongoing maintenance. Running a node is not "set and forget" — clients require regular updates for security patches and network upgrades.

- SaaS providers offer convenience and managed uptime, but introduce provider dependency and potential single points of failure. Consider multi-provider architectures for mission-critical applications.



---



**Made for Web3 developers, node operators, infrastructure engineers, and blockchain architects.**  

Let's make blockchain infrastructure more open, transparent, and resilient.
