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



- **[Alchemy](https://www.alchemy.com/)**  

  Web3 development platform providing RPC access plus enhanced APIs, Notify, and a large suite of tooling for Ethereum and multi-chain development. Free tier includes 100,000 requests/day and 10 GB storage .



- **[Infura](https://www.infura.io/)**  

  One of the oldest and most trusted Ethereum RPC providers, owned by Consensys and serving as MetaMask's default backend. Supports 20+ chains including Ethereum, Polygon, Optimism, Arbitrum, and Base. Free tier: 100,000 requests/day and 5 GB storage .



- **[QuickNode](https://www.quicknode.com/)**  

  Blockchain infrastructure platform supporting 80+ chains with high-performance RPC endpoints. Known for good scalability and reliability .



- **[Ankr](https://www.ankr.com/)**  

  Blockchain infrastructure provider built around a decentralized physical infrastructure network (DePIN) with a globally distributed node fleet. Offers free tier access .



- **[Chainstack](https://chainstack.com/)**  

  Multi-chain infrastructure platform supporting 70+ protocols with enterprise-grade deployment control. Features Hybrid Cloud for running dedicated nodes in your own cloud environment .



- **[Tatum](https://tatum.io/)**  

  Enterprise blockchain infrastructure platform combining RPC access with advanced developer tools including Wallet SDK, Blockchain Data API, and smart wallet solutions. SOC 2 compliant and ISO/IEC 27001:2022 certified . Platform consists of Blockchain Infrastructure, Tatum Platform (Cloud), and Developer Libraries .



- **[Moralis](https://moralis.io/)**  

  Web3 data platform providing structured, real-time blockchain data APIs across 40+ EVM chains and Solana. SOC 2 Type 2 certified with enterprise-grade security . Offers Onchain Skills for AI agents with 136+ endpoints for blockchain data queries .



- **[GetBlock](https://getblock.io/)**  

  Web3 infrastructure provider offering RPC access to blockchain networks via JSON-RPC and WebSocket endpoints without running your own nodes .



- **[Blockdaemon](https://www.blockdaemon.com/)**  

  Enterprise-grade blockchain infrastructure with node management, staking, and institutional-grade security.



- **[NOWNodes](https://nownodes.io/)**  

  Blockchain node provider offering shared and dedicated nodes with a focus on cost-effective RPC access.



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
