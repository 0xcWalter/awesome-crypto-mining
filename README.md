<div align="center">

# Awesome Crypto Mining [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of Proof of Work (PoW) mining resources — hardware, firmware, miners, pools, stratum software, network data and per-coin toolchains — for people who actually run machines and for investors who model the economics behind them.

[Contributing](CONTRIBUTING.md) • [License](#license)

</div>

---

Every entry below points at a canonical project site or its official repository. No referral links, no affiliate tags, no cloud-mining contracts. Anything that goes dark or gets abandoned is removed — see [CONTRIBUTING.md](CONTRIBUTING.md) for the inclusion rules.

## Contents

- [Start Here](#start-here)
- [Network Data, Calculators & Mining Economics](#network-data-calculators--mining-economics)
- [Mining Hardware](#mining-hardware)
  - [Open Source & Home Micro-Miners](#open-source--home-micro-miners)
  - [Industrial ASIC Manufacturers](#industrial-asic-manufacturers)
  - [Hardware Databases & Benchmarks](#hardware-databases--benchmarks)
  - [GPU Mining](#gpu-mining)
  - [CPU Mining](#cpu-mining)
- [Mining Software](#mining-software)
  - [CPU Miners](#cpu-miners)
  - [GPU Miners](#gpu-miners)
  - [Miner Managers & Profit Switchers](#miner-managers--profit-switchers)
- [Operating Systems & Custom Firmware](#operating-systems--custom-firmware)
- [Pool & Stratum Software](#pool--stratum-software)
- [Mining Pools](#mining-pools)
  - [Solo Mining Pools](#solo-mining-pools)
  - [PPLNS, PPS & Multi-Coin Pools](#pplns-pps--multi-coin-pools)
- [PoW Coins: Tools by Algorithm Family](#pow-coins-tools-by-algorithm-family)
  - [SHA-256](#sha-256)
  - [Scrypt](#scrypt)
  - [RandomX & CPU-First Chains](#randomx--cpu-first-chains)
  - [kHeavyHash & BlockDAG](#kheavyhash--blockdag)
  - [KawPow Family](#kawpow-family)
  - [Autolykos, FishHash & Modern GPU Algorithms](#autolykos-fishhash--modern-gpu-algorithms)
  - [Ethash & Successors](#ethash--successors)
  - [Equihash & zk-Focused Chains](#equihash--zk-focused-chains)
  - [Independent & Unique Algorithms](#independent--unique-algorithms)
- [Research, News & Community](#research-news--community)
- [Contributing](#contributing)
- [License](#license)

---

## Start Here

New to mining, or evaluating whether a machine pays for itself before you buy it? These four answer most first questions.

- **[Open Source Miners United Wiki](https://osmu.wiki/)** — Community-maintained wiki covering miner configuration, algorithm support matrices, overclocking and troubleshooting across dozens of coins.
- **[MiningPoolStats](https://miningpoolstats.stream/)** — Live network hashrate, difficulty and the full pool list for essentially every PoW coin in circulation. The fastest way to see whether a chain has real infrastructure behind it.
- **[BackPoW](https://backpow.com)** — Proof of Work oracle: electrical Cost of Production per coin, breakeven electricity rate, and Poisson-modelled solo block discovery odds for 120+ chains against 650+ ASICs, GPUs and CPUs. Public REST API, no account required.
- **[WhatToMine](https://whattomine.com/)** — The long-standing switching calculator for [GPU rigs](https://whattomine.com/coins) and [ASICs](https://whattomine.com/asic), useful for a first pass on what an existing machine should be pointed at.

---

## Network Data, Calculators & Mining Economics

- **[2CryptoCalc](https://2cryptocalc.com/)** — Historical mining profitability charts and per-pool reward comparisons over time rather than a single spot snapshot.
- **[ASIC Miner Value](https://www.asicminervalue.com/)** — Catalogue of ASIC models with hashrate, power draw, efficiency in J/TH and current profitability ranking.
- **[BackPoW](https://backpow.com)** — Cost of Production and solo block odds oracle, with per-coin pages, hardware-vs-coin combinations and an unauthenticated JSON API for scripted analysis.
- **[BitInfoCharts](https://bitinfocharts.com/)** — Long-range difficulty, hashrate, fee and address-distribution charts for major PoW chains.
- **[CoinWarz](https://www.coinwarz.com/calculators)** — Classic difficulty and profitability calculators with historical difficulty series per coin.
- **[Diff.cat](https://diff.cat/)** — Minimal Bitcoin difficulty adjustment tracker with projected change and time to retarget.
- **[Hashrate.no](https://hashrate.no/)** — GPU and CPU benchmark database with tuned overclock profiles, power draw and per-coin revenue per card.
- **[Hashrate Index](https://hashrateindex.com/)** — Luxor's hashprice index, rig price index and mining market research for industrial-scale operators.
- **[Mempool.space](https://mempool.space/)** — Bitcoin mempool, fee market and block visualiser, including a mining dashboard with pool share and reward breakdowns.
- **[minerstat](https://minerstat.com/coins)** — Coin, algorithm and [hardware](https://minerstat.com/hardware) reference database alongside profitability calculators.
- **[MiningPoolStats](https://miningpoolstats.stream/)** — Real-time network hashrate distribution, pool listings and block explorer directory for all PoW coins.
- **[NiceHash Profitability Calculator](https://www.nicehash.com/profitability-calculator)** — Hashrate marketplace pricing per algorithm, a useful proxy for the rental cost of attacking or renting into a small chain.
- **[SoloChance](https://solochance.com/)** — Simple solo lottery odds calculator for small SHA-256 machines.
- **[Timechain Calendar](https://timechaincalendar.com/)** — Bitcoin block height, halving countdown and epoch data presented as a calendar.
- **[WhatToMine](https://whattomine.com/)** — Multi-GPU and multi-ASIC profitability and algorithm switching calculator.

---

## Mining Hardware

### Open Source & Home Micro-Miners

- **[Bitaxe](https://github.com/skot/bitaxe)** — Open-source hardware Bitcoin ASIC miner built around single BM1366/BM1368/BM1370 chips (Ultra, Supra, Gamma). Fully documented schematics, 15–30 W, near-silent.
- **[Bitaxe.org](https://www.bitaxe.org/)** — Project hub for the Bitaxe family: variants, build guides and firmware links.
- **[GekkoScience](https://www.gekkoscience.com/)** — USB stick and pod miners (NewPac, Compac F, Terminus R909) for tinkering and low-power solo mining.
- **[NerdMiner v2](https://github.com/BitMaker-hub/NerdMiner_v2)** — Open-source ESP32 lottery miner (~78 KH/s) designed as a teaching and hobby device rather than a revenue machine.

### Industrial ASIC Manufacturers

- **[Bitmain](https://www.bitmain.com/)** — Antminer line for SHA-256 (S21 series), Scrypt (L7/L9), Equihash (Z15 Pro) and kHeavyHash (KS5 Pro).
- **[Canaan](https://www.canaan.io/)** — Avalon series Bitcoin miners and home-format units.
- **[Goldshell](https://www.goldshell.com/)** — Quiet BOX-series units for altcoin algorithms plus rackmount models.
- **[IceRiver](https://www.iceriver.io/)** — kHeavyHash and Blake3 ASICs (KS series for Kaspa, AL series for Alephium).
- **[MicroBT](https://www.whatsminer.com/)** — Whatsminer M-series SHA-256 machines, including hydro and immersion variants.

### Hardware Databases & Benchmarks

- **[ASIC Miner Value](https://www.asicminervalue.com/)** — Specifications, efficiency and resale-market pricing for retired and current ASIC models.
- **[Hashrate.no](https://hashrate.no/)** — Measured GPU/CPU hashrate and power figures per algorithm, with community-submitted tuning profiles.
- **[minerstat Hardware](https://minerstat.com/hardware)** — Cross-referenced ASIC, GPU and CPU database linked to supported algorithms.

### GPU Mining

- **NVIDIA GeForce RTX Series** — RTX 5090/4090/4080/3080-class cards for memory-hard and compute-heavy algorithms (KawPow, Autolykos2, FishHash, Blake3, XelisHash).
- **AMD Radeon RX Series** — RX 7900 XTX, 7800 XT, 6800 XT and 6700 XT, historically strongest on compute-per-watt for Ethash variants, ProgPoW and KawPow.

### CPU Mining

- **AMD Ryzen & Threadripper** — Large L3 cache parts (7950X, 9950X, Threadripper PRO) are the reference platform for RandomX and VerusHash.
- **AMD EPYC** — Multi-socket server CPUs with high memory bandwidth and L3 per core, used for dense RandomX deployments.
- **Intel Xeon & Core Ultra** — Competitive on AVX-512-friendly workloads and widely available second-hand for low-cost CPU mining.

---

## Mining Software

### CPU Miners

- **[cpuminer-multi / pooler's cpuminer](https://github.com/pooler/cpuminer)** — Minimal, auditable Scrypt and SHA-256 CPU reference miner.
- **[cpuminer-opt](https://github.com/JayDDee/cpuminer-opt)** — Optimised multi-algorithm CPU miner with hand-tuned SIMD paths for dozens of hash functions.
- **[SRBMiner-Multi](https://github.com/doktor83/SRBMiner-Multi)** — CPU and AMD/NVIDIA/Intel GPU miner covering one of the widest algorithm ranges available ([releases](https://github.com/doktor83/SRBMiner-Multi/releases)).
- **[XMRig](https://github.com/xmrig/xmrig)** — The reference RandomX miner, with MSR mods, huge pages automation and [documentation](https://xmrig.com/docs/miner) that doubles as a tuning guide.
- **[XMRig MoneroOcean fork](https://github.com/MoneroOcean/xmrig)** — XMRig build with automatic algorithm switching for multi-algo CPU pools.

### GPU Miners

- **[BzMiner](https://github.com/bzminer/bzminer)** — Multi-platform GPU miner with dual mining and a built-in HTTP monitoring endpoint.
- **[ccminer](https://github.com/tpruvot/ccminer)** — Open-source CUDA miner, still the base for many niche algorithm forks.
- **[GMiner](https://github.com/develsoftware/GMinerRelease)** — Long-maintained NVIDIA/AMD miner with broad Equihash, Autolykos and Ethash coverage.
- **[kawpowminer](https://github.com/RavenCommunity/kawpowminer)** — Open-source reference KawPow miner maintained by the Ravencoin community.
- **[lolMiner](https://github.com/Lolliedieb/lolMiner-releases)** — Autolykos2, Equihash, Blake3, FishHash and dual-mining workhorse ([releases](https://github.com/Lolliedieb/lolMiner-releases/releases)).
- **[nanominer](https://github.com/nanopool/nanominer)** — Multi-algorithm miner with a straightforward configuration format and watchdog.
- **[OneZeroMiner](https://github.com/OneZeroMiner/onezerominer)** — Specialised client for Dynex, Salvium and newer compute-oriented algorithms.
- **[Rigel](https://github.com/rigelminer/rigel)** — Fast NVIDIA miner focused on dual/triple mining across Nexa, Alephium, Iron Fish, KawPow and Karlsen ([releases](https://github.com/rigelminer/rigel/releases)).
- **[T-Rex](https://github.com/trexminer/T-Rex)** — NVIDIA miner with a strong KawPow/Octopus track record and an active release feed.
- **[TeamRedMiner](https://github.com/todxx/teamredminer)** — AMD-only miner with hand-optimised kernels for KawPow, Autolykos2 and FiroPow.
- **[WildRig Multi](https://github.com/andru-kun/wildrig-multi)** — Broad coverage of legacy and exotic GPU algorithms that other miners have dropped.

### Miner Managers & Profit Switchers

- **[Awesome Miner](https://awesomeminer.com/)** — Windows-based management for large mixed fleets of GPU rigs and ASICs, with rules-based profit switching.
- **[NiceHash Miner](https://github.com/nicehash/NiceHashMiner)** — Open-source benchmarking and switching front-end for the NiceHash hashrate marketplace.
- **[Sriracha](https://github.com/ccuetoh/sriracha)** — Lightweight open-source tooling for scripted miner orchestration.
- **[UG-Miner](https://github.com/UselessGuru/UG-Miner)** — Open-source PowerShell profit switcher supporting many miners, pools and algorithms.

---

## Operating Systems & Custom Firmware

- **[AxeOS / ESP-Miner](https://github.com/bitaxeorg/ESP-Miner)** — Open-source firmware for ESP32-based ASIC miners (Bitaxe family) with a responsive web UI, frequency/voltage tuning and stratum failover.
- **[Braiins OS](https://braiins.com/os)** — Open-source-derived autotuning firmware for Antminer hardware with per-chip frequency and voltage scaling, and native Stratum V2 support.
- **[HiveOS](https://hiveon.com/os/)** — Linux mining OS with a hosted dashboard, overclock profiles and fleet telemetry.
- **[LuxOS](https://luxor.tech/mining/firmware)** — Commercial firmware for Antminer fleets focused on efficiency curves and reliability at scale.
- **[minerstat msOS](https://minerstat.com/software/mining-os)** — Linux distribution for farm management with remote diagnostics and profit switching.
- **[RaveOS](https://raveos.com/)** — Lightweight headless OS supporting mixed AMD/NVIDIA rigs and ASIC management.
- **[VNish](https://vnish.net/)** — Third-party firmware for Antminer and Whatsminer units with autotuning and efficiency presets.

---

## Pool & Stratum Software

Run your own infrastructure instead of trusting someone else's.

- **[ckpool](https://github.com/ckolivas/ckpool)** — Con Kolivas's minimal C pool server, the codebase behind solo.ckpool.org.
- **[DATUM Gateway](https://github.com/OCEAN-xyz/datum_gateway)** — Lets a miner build and choose its own block templates while pooling variance through OCEAN.
- **[Miningcore](https://github.com/oliverw/miningcore)** — Multi-coin pool engine in .NET supporting most major PoW families.
- **[P2Pool](https://github.com/SChernykh/p2pool)** — Decentralised, chain-based Monero pool: 0% fee, no operator, payouts direct in the coinbase.
- **[public-pool](https://github.com/benjamin-wilson/public-pool)** — Open-source solo Bitcoin stratum server popular with Bitaxe and home-miner setups.
- **[Stratum V2 Reference Implementation](https://github.com/stratum-mining/stratum)** — Rust implementation of the encrypted, template-negotiating successor to Stratum V1 ([specification](https://github.com/stratum-mining/sv2-spec), [protocol site](https://stratumprotocol.org/)).

---

## Mining Pools

### Solo Mining Pools

- **[2Miners Solo](https://2miners.com/)** — Isolated solo tiers alongside its PPLNS pools, including [Ravencoin](https://2miners.com/solo-rvn-mining-pool), [Ergo](https://2miners.com/solo-erg-mining-pool), [Kaspa](https://2miners.com/solo-kas-mining-pool) and [Ethereum Classic](https://2miners.com/solo-etc-mining-pool).
- **[BTC PoW Lab](https://btcpowlab-pool.com/)** — Bitcoin Hybrid Solo pool with public Stratum V1, address based access, public status and proof pages, and a transparent 85% finder, 10% eligible community and 5% operator reward split.
- **[CKPool Solo](https://solo.ckpool.org/)** — The original zero-dependency Bitcoin solo pool; 2% fee, paid only on a found block.
- **[OCEAN](https://ocean.xyz/)** — Non-custodial Bitcoin pool paying directly from the coinbase, with [DATUM](https://www.ocean.xyz/docs/datum) for miner-side template construction.
- **[SoloPool.org](https://solopool.org/)** — Solo stratum endpoints for 40+ altcoins with global low-latency nodes.

### PPLNS, PPS & Multi-Coin Pools

- **[AntPool](https://www.antpool.com/)** — Large multi-coin pool with global stratum nodes and merged mining support.
- **[Braiins Pool](https://braiins.com/pool)** — Long-running Bitcoin pool (formerly Slush Pool) and an early Stratum V2 deployment.
- **[F2Pool](https://www.f2pool.com/)** — One of the oldest pools, covering BTC, LTC, DOGE, ZEC, HNS, KAS and dozens more.
- **[FlockPool](https://flockpool.com/)** — Focused pool for Evrmore, Clore and other KawPow-family chains.
- **[HeroMiners](https://herominers.com/)** — Multi-coin operator with per-coin subdomains offering both PPLNS and solo endpoints for most newer algorithms.
- **[K1Pool](https://k1pool.com/)** — Multi-coin pool covering CKB, Nexa, Alephium and others, with merged-mining options.
- **[Kryptex Pool](https://pool.kryptex.com/)** — Beginner-oriented pool with clear per-coin setup docs for KawPow, kHeavyHash and Blake3 chains.
- **[Luxor](https://luxor.tech/mining/mining-pool)** — Institutional-grade pool and hashrate marketplace with detailed payout reporting.
- **[Mining Dutch](https://www.mining-dutch.nl/)** — Long-running European multi-algorithm pool.
- **[Nanopool](https://nanopool.org/)** — Established multi-coin pool with a public API for worker monitoring.
- **[Prohashing](https://prohashing.com/)** — Multi-algorithm pool with payouts in a chosen coin and transparent accounting.
- **[ViaBTC](https://www.viabtc.com/)** — PPS+, PPLNS and merged mining across major SHA-256 and Scrypt chains.
- **[WoolyPooly](https://woolypooly.com/)** — Mid-size pool with strong coverage of newer GPU coins and a clean stats interface.

---

## PoW Coins: Tools by Algorithm Family

Chains are grouped by the algorithm they actually use, because that is what determines which hardware and which miner binary you need. For each coin: node software, explorer, wallet, miner support, pools, and the data sources used to model returns before committing hardware.

### SHA-256

#### Bitcoin (BTC)

- **[Bitcoin Core](https://bitcoincore.org/)** — Reference full node and wallet; running one is the prerequisite for template-level control over what you mine.
- **[Mempool.space](https://mempool.space/)** — Block explorer, fee market and mining dashboard with pool share, reward and difficulty adjustment data.
- **[Bitnodes](https://bitnodes.io/)** — Reachable node census and network topology snapshot.
- **[Fork Monitor](https://forkmonitor.info/)** — Watches for stale blocks, chain splits and inflation-invariant violations across node implementations.
- **[CKPool Solo](https://solo.ckpool.org/)** — Solo stratum for small machines; the canonical home of the lottery-block story.
- **[OCEAN](https://ocean.xyz/)** — Non-custodial pool with miner-built templates via DATUM.
- **[Braiins Pool](https://braiins.com/pool)** — Established pool with Stratum V2 support.
- **[BackPoW Bitcoin](https://backpow.com/Bitcoin)** — Cost of Production per machine, breakeven electricity rate, and Poisson solo odds for any hashrate you point at the network.
- **[Timechain Calendar](https://timechaincalendar.com/)** — Halving countdown, epoch progress and block height reference.
- **[MiningPoolStats BTC](https://miningpoolstats.stream/bitcoin)** — Pool hashrate distribution and difficulty history.

#### Bitcoin Cash (BCH)

- **[Bitcoin Cash Node](https://bitcoincashnode.org/)** — Reference full node implementation.
- **[Blockchair BCH](https://blockchair.com/bitcoin-cash)** — Explorer with full-text search and downloadable datasets.
- **[F2Pool BCH](https://www.f2pool.com/coin/bitcoin-cash)** — Major SHA-256 pool with a dedicated BCH endpoint and payout stats.
- **[MiningPoolStats BCH](https://miningpoolstats.stream/bitcoincash)** — Pool distribution and network hashrate.
- **[BackPoW Bitcoin Cash](https://backpow.com/BitcoinCash)** — SHA-256 profitability and CoP against the same hardware set used for BTC, which is what makes the two chains directly comparable.
- **[Hashrate.no BCH](https://www.hashrate.no/coins/BCH)** — Revenue per machine at current difficulty.

### Scrypt

#### Litecoin (LTC)

- **[Litecoin Core](https://github.com/litecoin-project/litecoin)** — Official node and wallet ([project site](https://litecoin.org/)).
- **[litecoinspace.org](https://litecoinspace.org/)** — Mempool-style explorer with fee estimation and mining stats.
- **[Blockchair Litecoin](https://blockchair.com/litecoin)** — Universal explorer with API access.
- **[F2Pool LTC](https://www.f2pool.com/coin/litecoin)** — Scrypt pool with LTC/DOGE merged mining enabled by default.
- **[Hashrate.no LTC](https://www.hashrate.no/coins/LTC)** — Hardware revenue per model for Scrypt ASICs.
- **[BackPoW Litecoin](https://backpow.com/Litecoin)** — Scrypt CoP, breakeven power price and the merged-mining context that decides whether an L7/L9 is viable.
- **[MiningPoolStats LTC](https://miningpoolstats.stream/litecoin)** — Pool and difficulty tracking.

#### Dogecoin (DOGE)

- **[Dogecoin Core](https://github.com/dogecoin/dogecoin)** — Reference node and wallet.
- **[Blockchair Dogecoin](https://blockchair.com/dogecoin)** — Explorer and dataset access.
- **[F2Pool DOGE](https://www.f2pool.com/coin/dogecoin)** — Merged LTC/DOGE mining, which is where almost all DOGE hashrate actually comes from.
- **[MiningPoolStats DOGE](https://miningpoolstats.stream/dogecoin)** — Pool share and network difficulty.
- **[BackPoW Dogecoin](https://backpow.com/Dogecoin)** — Auxiliary-PoW aware revenue model, including the merged-mining reward stacked on Litecoin hashrate.

#### Pepecoin (PEPE)

- **[Pepecoin Core](https://github.com/pepecoinppc/pepecoin)** — Dogecoin-derived node and wallet ([project site](https://pepecoin.org/)).
- **[MiningPoolStats PEPE](https://miningpoolstats.stream/pepecoin)** — Active pools and network hashrate.
- **[BackPoW Pepecoin](https://backpow.com/Pepecoin)** — Scrypt solo odds and CoP for the small-cap end of the Scrypt market.
- **[SRBMiner-Multi](https://github.com/doktor83/SRBMiner-Multi)** — Scrypt support for GPU and CPU miners.

### RandomX & CPU-First Chains

#### Monero (XMR)

- **[Monero](https://github.com/monero-project/monero)** — Reference daemon, CLI and GUI wallet ([project site](https://www.getmonero.org/)).
- **[XMRig](https://github.com/xmrig/xmrig)** — The RandomX miner, plus [tuning docs](https://xmrig.com/docs/miner) covering MSR mods and huge pages.
- **[P2Pool](https://github.com/SChernykh/p2pool)** — Decentralised pool with no operator and coinbase payouts.
- **[P2Pool Observer](https://p2pool.observer/)** — Explorer and payout statistics for the P2Pool sidechain.
- **[Gupax](https://gupax.io/)** — Cross-platform GUI bundling XMRig and P2Pool for one-click decentralised mining.
- **[xmrchain.net](https://xmrchain.net/)** — Open-source Monero block explorer.
- **[Monero HeroMiners](https://monero.herominers.com/)**, **[SupportXMR](https://www.supportxmr.com/)**, **[HashVault](https://hashvault.pro/)** — Established centralised alternatives when P2Pool's minimum payout is impractical.
- **[BackPoW Monero](https://backpow.com/Monero)** — RandomX CoP per CPU model and breakeven electricity price, the number that decides whether home CPU mining clears its own power bill.
- **[MiningPoolStats XMR](https://miningpoolstats.stream/monero)** — Pool distribution and difficulty.

#### Zephyr Protocol (ZEPH)

- **[Zephyr Node](https://github.com/ZephyrProtocol/zephyr)** — Core daemon and GUI wallet ([project site](https://zephyrprotocol.com/)).
- **[Zephyr Explorer](https://explorer.zephyrprotocol.com/)** — Blockchain explorer with reserve-asset monitoring.
- **[XMRig](https://github.com/xmrig/xmrig)** — RandomX miner used for ZEPH.
- **[Zephyr HeroMiners](https://zephyr.herominers.com/)** and **[2Miners ZEPH](https://2miners.com/zeph-mining-pool)** — Main public pools.
- **[BackPoW Zephyr](https://backpow.com/Zephyr)** — RandomX CPU revenue and CoP, useful because ZEPH's emission interacts with its reserve system.
- **[Hashrate.no ZEPH](https://www.hashrate.no/coins/ZEPH)** — Per-CPU and per-GPU measured performance.

#### Salvium (SAL)

- **[Salvium](https://github.com/salvium/salvium)** — Core daemon and wallet ([project site](https://salvium.io/)).
- **[Salvium Explorer](https://explorer.salvium.io/)** — Official block explorer.
- **[Salvium HeroMiners](https://salvium.herominers.com/)** — Public pool with solo and PPLNS ports.
- **[MiningPoolStats SAL](https://miningpoolstats.stream/salvium)** — Pool and hashrate overview.
- **[BackPoW Salvium](https://backpow.com/Salvium)** — CPU mining economics for a young RandomX-family chain.

#### Verus (VRSC)

- **[VerusCoin](https://github.com/VerusCoin/VerusCoin)** — Node, wallet and VerusHash implementation ([project site](https://verus.io/)).
- **[Verus Explorer](https://explorer.verus.io/)** — Official explorer.
- **[LuckPool](https://luckpool.net/)** — The dominant VerusHash pool, with per-region stratum endpoints.
- **[BackPoW Verus](https://backpow.com/Verus)** — VerusHash CPU profitability and breakeven power rate.
- **[Hashrate.no VRSC](https://www.hashrate.no/coins/VRSC)** — CPU benchmark reference for VerusHash tuning.

### kHeavyHash & BlockDAG

#### Kaspa (KAS)

- **[Rusty-Kaspa](https://github.com/kaspanet/rusty-kaspa)** — Official high-performance Rust node ([project site](https://kaspa.org/)).
- **[Kaspa Explorer](https://explorer.kaspa.org/)** — Official BlockDAG explorer.
- **[kas.fyi](https://kas.fyi/)** — Alternative explorer with richer address, token and network analytics.
- **[Kaspium](https://kaspium.io/)** — Non-custodial mobile and desktop wallet.
- **[Rigel](https://github.com/rigelminer/rigel)** and **[lolMiner](https://github.com/Lolliedieb/lolMiner-releases)** — GPU miners for kHeavyHash, still relevant for testing even though ASICs dominate.
- **[Kaspa HeroMiners](https://kaspa.herominers.com/)**, **[2Miners KAS](https://2miners.com/kas-mining-pool)** (with a [solo tier](https://2miners.com/solo-kas-mining-pool)), **[Kaspa-Pool](https://kaspa-pool.org/)**, **[ACC-Pool](https://acc-pool.pw/)**, **[Katpool](https://katpool.com/)** — Active pool options across fee models.
- **[BackPoW Kaspa](https://backpow.com/Kaspa)** — kHeavyHash CoP per ASIC model and solo block odds, which on a one-second block time is one of the few places solo mining is statistically meaningful for small machines.
- **[MiningPoolStats KAS](https://miningpoolstats.stream/kaspa)** — Pool distribution and difficulty.

#### Karlsen (KLS)

- **[karlsend](https://github.com/karlsen-network/karlsend)** — Go node implementation for the KarlsenHashV2 (FishHash + Blake3) BlockDAG ([project site](https://karlsencoin.org/)).
- **[Karlsen Explorer](https://explorer.karlsencoin.org/)** — Official explorer.
- **[Rigel](https://github.com/rigelminer/rigel)** — Primary GPU miner for KarlsenHashV2.
- **[WoolyPooly KLS](https://woolypooly.com/en/coin/kls)** — Main public pool.
- **[Hashrate.no KLS](https://www.hashrate.no/coins/KLS)** — Per-GPU measured hashrate, important because the 4 GB DAG excludes older cards.
- **[BackPoW Karlsen](https://backpow.com/Karlsen)** — GPU profitability and CoP for an explicitly ASIC-resistant DAG chain.
- **[MiningPoolStats KLS](https://miningpoolstats.stream/karlsen)** — Pool listing and difficulty.

#### Hoosat (HTN)

- **[HTND](https://github.com/HoosatNetwork/HTND)** — Official Go node ([project site](https://hoosat.fi/)).
- **[Hoosat Explorer](https://explorer.hoosat.fi/)** — Official block explorer.
- **[SRBMiner-Multi](https://github.com/doktor83/SRBMiner-Multi)** — Hoohash support for AMD and NVIDIA.
- **[MiningPoolStats HTN](https://miningpoolstats.stream/hoosat)** — Active pools and network hashrate.
- **[BackPoW Hoosat](https://backpow.com/Hoosat)** — Hoohash GPU economics and difficulty tracking.

#### Nexa (NEXA)

- **[Nexa](https://gitlab.com/nexa/nexa)** — Official node and wallet source ([project site](https://nexa.org/)).
- **[Nexa Explorer](https://explorer.nexa.org/)** — Official explorer.
- **[Rigel](https://github.com/rigelminer/rigel)** — NexaPow GPU miner, commonly run in dual-mining configurations.
- **[2Miners NEXA](https://2miners.com/nexa-mining-pool)** and **[Kryptex Pool NEXA](https://pool.kryptex.com/nexa)** — Public pools.
- **[BackPoW Nexa](https://backpow.com/Nexa)** — Per-GPU revenue and CoP for a high-emission chain where power price dominates the outcome.
- **[MiningPoolStats NEXA](https://miningpoolstats.stream/nexa)** — Pool and hashrate data.

### KawPow Family

#### Ravencoin (RVN)

- **[Ravencoin Core](https://github.com/RavenProject/Ravencoin)** — Official node, wallet and asset layer ([project site](https://ravencoin.org/)).
- **[CryptoScope RVN](https://cryptoscope.io/rvn/)** — Block, asset and rich-list explorer.
- **[kawpowminer](https://github.com/RavenCommunity/kawpowminer)** — Community-maintained open-source reference miner.
- **[TeamRedMiner](https://github.com/todxx/teamredminer)** (AMD) and **[T-Rex](https://github.com/trexminer/T-Rex)** (NVIDIA) — The two performance miners most RVN hashrate runs on.
- **[2Miners RVN](https://2miners.com/rvn-mining-pool)** with a [solo tier](https://2miners.com/solo-rvn-mining-pool), **[WoolyPooly RVN](https://woolypooly.com/en/coin/rvn)** and **[Kryptex Pool RVN](https://pool.kryptex.com/rvn)** — Pool options.
- **[Hashrate.no RVN](https://www.hashrate.no/coins/RVN)** — Per-card hashrate and tuned power draw.
- **[BackPoW Ravencoin](https://backpow.com/Ravencoin)** — KawPow CoP, breakeven electricity rate and solo odds per rig size.
- **[MiningPoolStats RVN](https://miningpoolstats.stream/ravencoin)** — Pool distribution.

#### Evrmore (EVR)

- **[Evrmore](https://github.com/EvrmoreOrg/Evrmore)** — Ravencoin-derived node with the EvrProgPow algorithm ([project site](https://evrmorecoin.org/)).
- **[CryptoScope EVR](https://cryptoscope.io/evrmore/)** — Block and asset explorer.
- **[FlockPool EVR](https://flockpool.com/coins/evr)** — Primary public pool.
- **[BackPoW Evrmore](https://backpow.com/Evrmore)** — GPU profitability and CoP.
- **[MiningPoolStats EVR](https://miningpoolstats.stream/evrmorecoin)** — Pool and difficulty overview.

#### Neoxa (NEOX)

- **[Neoxa Core](https://github.com/NeoxaChain/Neoxa)** — Official node and wallet ([project site](https://neoxa.net/)).
- **[Neoxa Explorer](https://explorer.neoxa.net/)** — Transaction and asset explorer.
- **[Hashrate.no NEOX](https://www.hashrate.no/coins/NEOX)** — Measured per-GPU performance.
- **[BackPoW Neoxa](https://backpow.com/Neoxa)** — KawPow economics including the gaming-reward emission split.
- **[MiningPoolStats NEOX](https://miningpoolstats.stream/neoxa)** — Active pools.

#### Clore.ai (CLORE)

- **[Clore.ai](https://clore.ai/)** — GPU rental marketplace whose native chain is mined with KawPow; rental income is the reason the coin's mining economics differ from its peers.
- **[FlockPool CLORE](https://flockpool.com/coins/clore)** and **[Kryptex Pool](https://pool.kryptex.com/clore)** — Public pools.
- **[Hashrate.no CLORE](https://www.hashrate.no/coins/CLORE)** — Per-GPU revenue figures.
- **[MiningPoolStats CLORE](https://miningpoolstats.stream/clore)** — Pool distribution and hashrate.

#### Neurai (XNA)

- **[Neurai](https://neurai.org/)** — Project site with node and wallet downloads.
- **[Neurai Explorer](https://explorer.neurai.org/)** — Official explorer.
- **[MiningPoolStats XNA](https://miningpoolstats.stream/neurai)** — Pools and difficulty.
- **[BackPoW Neurai](https://backpow.com/Neurai)** — KawPow CoP for a low-difficulty chain where solo mining is still plausible.
- **[Hashrate.no XNA](https://www.hashrate.no/coins/XNA)** — Per-card benchmarks.

#### Telestai (TLS)

- **[Telestai](https://github.com/Telestai-Project/telestai)** — Node and wallet source ([project site](https://www.telestai.io/)).
- **[Telestai Explorer](https://explorer.telestai.io/)** — Official explorer.
- **[MiningPoolStats TLS](https://miningpoolstats.stream/telestai)** — Pool listing.
- **[BackPoW Telestai](https://backpow.com/Telestai)** — Mining calculator and network metrics.

### Autolykos, FishHash & Modern GPU Algorithms

#### Ergo (ERG)

- **[Ergo Node](https://github.com/ergoplatform/ergo)** — Official Scala reference node ([project site](https://ergoplatform.org/en/)).
- **[Ergo Explorer](https://explorer.ergoplatform.com/)** — On-chain explorer with box search and token metrics.
- **[ErgExplorer](https://ergexplorer.com/)** — Alternative explorer with a different UI and API.
- **[ergo.watch](https://ergo.watch/)** — On-chain metrics dashboard tracking addresses, supply distribution and mining flows.
- **[Nautilus Wallet](https://github.com/nautls/nautilus-wallet)** — Non-custodial browser wallet.
- **[lolMiner](https://github.com/Lolliedieb/lolMiner-releases)** and **[TeamRedMiner](https://github.com/todxx/teamredminer)** — Autolykos2 miners for NVIDIA and AMD respectively.
- **[Ergo HeroMiners](https://ergo.herominers.com/)**, **[2Miners ERG](https://2miners.com/erg-mining-pool)** plus a [solo tier](https://2miners.com/solo-erg-mining-pool) — Pool options.
- **[BackPoW Ergo](https://backpow.com/Ergo)** — Autolykos2 CoP per GPU and solo block odds, with the storage-rent and emission context that affects long-run returns.
- **[MiningPoolStats ERG](https://miningpoolstats.stream/ergo)** — Pool distribution.

#### Firo (FIRO)

- **[Firo](https://github.com/firoorg/firo)** — Official node implementing FiroPoW and Lelantus Spark ([downloads](https://firo.org/get-firo/download/)).
- **[Firo Explorer](https://explorer.firo.org/)** — Official blockchain and masternode explorer.
- **[TeamRedMiner](https://github.com/todxx/teamredminer)** and **[T-Rex](https://github.com/trexminer/T-Rex)** — FiroPoW miners.
- **[WoolyPooly FIRO](https://woolypooly.com/en/coin/firo)** — Public pool.
- **[MiningPoolStats FIRO](https://miningpoolstats.stream/firo)** — Pool and hashrate data.
- **[BackPoW Firo](https://backpow.com/Firo)** — FiroPoW GPU profitability, with the 50/50 masternode split reflected in the miner's share of emission.

#### Alephium (ALPH)

- **[Alephium Core](https://github.com/alephium/alephium)** — Official Scala full node for the sharded Blockflow chain ([project site](https://alephium.org/)).
- **[Alephium Explorer](https://explorer.alephium.org/)** — Sharded explorer with hashrate distribution per chain.
- **[Alephium GPU Miner](https://github.com/alephium/gpu-miner)** — Official Blake3 GPU miner.
- **[Alephium HeroMiners](https://alephium.herominers.com/)** and **[K1Pool ALPH](https://k1pool.com/pool/alph)** — Public pools.
- **[BackPoW Alephium](https://backpow.com/Alephium)** — Blake3 economics including the Proof-of-Less-Work adjustment that burns part of the reward as hashrate rises.
- **[MiningPoolStats ALPH](https://miningpoolstats.stream/alephium)** — Pools and difficulty.

#### Xelis (XEL)

- **[Xelis Blockchain](https://github.com/xelis-project/xelis-blockchain)** — Official Rust node, wallet and miner ([releases](https://github.com/xelis-project/xelis-blockchain/releases), [project site](https://xelis.io/)).
- **[Xelis Explorer](https://explorer.xelis.io/)** — BlockDAG explorer and emission tracker.
- **[Xelis Stats](https://stats.xelis.io/)** — Network statistics dashboard.
- **[xelis-hash](https://github.com/xelis-project/xelis-hash)** — Reference implementation of XelisHashV2, useful if you are benchmarking or porting.
- **[SRBMiner-Multi](https://github.com/doktor83/SRBMiner-Multi)** — CPU and GPU miner for XelisHashV2.
- **[Xelis HeroMiners](https://xelis.herominers.com/)** — Public pool with solo ports.
- **[BackPoW Xelis](https://backpow.com/Xelis)** — CPU/GPU profitability and CoP for a chain still mineable on commodity hardware.
- **[MiningPoolStats XEL](https://miningpoolstats.stream/xelis)** — Pool distribution.

#### Iron Fish (IRON)

- **[Iron Fish](https://github.com/iron-fish/ironfish)** — Official TypeScript node and CLI ([project site](https://ironfish.network/)).
- **[Iron Fish Explorer](https://explorer.ironfish.network/)** — Privacy-preserving block explorer.
- **[Rigel](https://github.com/rigelminer/rigel)** and **[lolMiner](https://github.com/Lolliedieb/lolMiner-releases)** — FishHash miners.
- **[Iron Fish HeroMiners](https://ironfish.herominers.com/)** — Public pool.
- **[BackPoW Iron Fish](https://backpow.com/IronFish)** — FishHash GPU revenue and breakeven electricity price.
- **[MiningPoolStats IRON](https://miningpoolstats.stream/ironfish)** — Pools and hashrate.

#### Warthog (WART)

- **[Warthog Core](https://github.com/warthog-network/core)** — Node implementing Proof of Balanced Work, which mixes CPU and GPU components ([project site](https://warthog.network/)).
- **[Warthog HeroMiners](https://warthog.herominers.com/)** — Public pool.
- **[MiningPoolStats WART](https://miningpoolstats.stream/warthog)** — Pool listing and difficulty.
- **[BackPoW Warthog](https://backpow.com/Warthog)** — Profitability model for a hybrid CPU/GPU algorithm, where the hardware mix decides the outcome.
- **[Hashrate.no WART](https://www.hashrate.no/coins/WART)** — Measured hardware performance.

#### Dynex (DNX)

- **[Dynex](https://github.com/DynexCoin/Dynex)** — Node software for the neuromorphic-compute PoW chain ([project site](https://dynexcoin.org/)).
- **[OneZeroMiner](https://github.com/OneZeroMiner/onezerominer)** — Primary DynexSolve miner.
- **[MiningPoolStats DNX](https://miningpoolstats.stream/dynexcoin)** — Pools and network hashrate.
- **[BackPoW Dynex](https://backpow.com/Dynexcoin)** — GPU profitability and CoP.
- **[Hashrate.no DNX](https://www.hashrate.no/coins/DNX)** — Per-card measured rates.

### Ethash & Successors

#### Ethereum Classic (ETC)

- **[Core-Geth](https://github.com/etclabscore/core-geth)** — Configurable EVM node supporting ETC ([project site](https://ethereumclassic.org/)).
- **[Blockscout ETC](https://etc.blockscout.com/)** — Open-source explorer with contract verification.
- **[lolMiner](https://github.com/Lolliedieb/lolMiner-releases)** and **[GMiner](https://github.com/develsoftware/GMinerRelease)** — Etchash miners.
- **[2Miners ETC](https://2miners.com/etc-mining-pool)** with a [solo tier](https://2miners.com/solo-etc-mining-pool), and **[F2Pool ETC](https://www.f2pool.com/coin/ethereum-classic)** — Pool options.
- **[BackPoW Ethereum Classic](https://backpow.com/EthereumClassic)** — Etchash CoP across GPUs and ASICs, the direct comparison that matters now that both compete on the same chain.
- **[MiningPoolStats ETC](https://miningpoolstats.stream/ethereumclassic)** — Pool distribution.

#### Conflux (CFX)

- **[conflux-rust](https://github.com/Conflux-Chain/conflux-rust)** — Official Rust node for the Tree-Graph chain ([project site](https://confluxnetwork.org/)).
- **[ConfluxScan](https://www.confluxscan.org/)** — Official explorer for both Core and eSpace.
- **[Conflux HeroMiners](https://conflux.herominers.com/)** — Public pool.
- **[BackPoW Conflux](https://backpow.com/Conflux)** — Octopus GPU profitability and CoP.
- **[MiningPoolStats CFX](https://miningpoolstats.stream/conflux)** — Pools and difficulty.

#### Nervos CKB (CKB)

- **[CKB](https://github.com/nervosnetwork/ckb)** — Official Rust node for the Eaglesong chain ([project site](https://www.nervos.org/)).
- **[CKB Explorer](https://explorer.nervos.org/)** — Official explorer with epoch and mining statistics.
- **[2Miners CKB](https://2miners.com/ckb-mining-pool)** and **[F2Pool CKB](https://www.f2pool.com/coin/nervos)** — Public pools.
- **[BackPoW Nervos](https://backpow.com/Nervos)** — Eaglesong ASIC profitability and CoP.
- **[MiningPoolStats CKB](https://miningpoolstats.stream/nervos)** — Pool distribution.

### Equihash & zk-Focused Chains

#### Zcash (ZEC)

- **[zcashd](https://github.com/zcash/zcash)** — Reference node ([project site](https://z.cash/), [operator documentation](https://zcash.readthedocs.io/en/latest/)).
- **[Zebra](https://github.com/ZcashFoundation/zebra)** — Independent Rust node implementation from the Zcash Foundation.
- **[Zcash Explorer](https://mainnet.zcashexplorer.app/)** — Block explorer with shielded-pool statistics.
- **[F2Pool ZEC](https://www.f2pool.com/coin/zcash)** — Major Equihash pool.
- **[BackPoW Zcash](https://backpow.com/Zcash)** — Equihash ASIC CoP and breakeven power rate.
- **[MiningPoolStats ZEC](https://miningpoolstats.stream/zcash)** — Pool and hashrate data.

#### Beam (BEAM)

- **[Beam](https://beam.mw/)** — Node, wallets and BeamHash documentation.
- **[Beam Explorer](https://explorer.beam.mw/)** — Official explorer.
- **[lolMiner](https://github.com/Lolliedieb/lolMiner-releases)** and **[GMiner](https://github.com/develsoftware/GMinerRelease)** — BeamHash III miners.
- **[Beam HeroMiners](https://beam.herominers.com/)** and **[2Miners BEAM](https://2miners.com/beam-mining-pool)** — Public pools.
- **[BackPoW Beam](https://backpow.com/Beam)** — BeamHash GPU profitability and CoP.
- **[MiningPoolStats BEAM](https://miningpoolstats.stream/beam)** — Pools and difficulty.

#### Grin (GRIN)

- **[Grin](https://github.com/mimblewimble/grin)** — Reference Mimblewimble node ([project site](https://grin.mw/)).
- **[lolMiner](https://github.com/Lolliedieb/lolMiner-releases)** — Cuckatoo32 miner.
- **[MiningPoolStats GRIN](https://miningpoolstats.stream/grin)** — Pool listing and network graph rate.
- **[BackPoW Grin](https://backpow.com/Grin-CT32)** — Cuckatoo32 profitability under Grin's linear, non-halving emission.

### Independent & Unique Algorithms

#### Dash (DASH)

- **[Dash Core](https://github.com/dashpay/dash)** — Official node with InstantSend and masternode support ([downloads](https://www.dash.org/downloads/)).
- **[Dash Insight](https://insight.dash.org/)** — Official network explorer.
- **[BackPoW Dash](https://backpow.com/Dash)** — X11 ASIC CoP, with the masternode and treasury split applied to the miner's actual share.
- **[MiningPoolStats DASH](https://miningpoolstats.stream/dash)** — Pool distribution and difficulty.
- **[Hashrate.no DASH](https://www.hashrate.no/coins/DASH)** — Revenue per X11 machine at current difficulty.

#### Decred (DCR)

- **[dcrd](https://github.com/decred/dcrd)** — Reference Go node for the hybrid PoW/PoS chain ([project site](https://decred.org/)).
- **[Decrediton](https://github.com/decred/decrediton)** — Official GUI wallet with integrated ticket purchasing.
- **[dcrdata](https://dcrdata.decred.org/)** — Official block explorer with ticket pool, staking and governance data.
- **[BackPoW Decred](https://backpow.com/Decred)** — Blake3 ASIC economics with the 10% PoW share of block reward applied, which is the number most generic calculators get wrong.
- **[MiningPoolStats DCR](https://miningpoolstats.stream/decred)** — Pools and hashrate.

#### Vertcoin (VTC)

- **[Vertcoin Core](https://github.com/vertcoin-project/vertcoin-core)** — Official node for the Verthash chain ([project site](https://vertcoin.org/)).
- **[Vertcoin One-Click Miner](https://github.com/vertcoin-project/one-click-miner-vnext)** — Beginner-friendly desktop miner.
- **[Vertcoin Explorer](https://insight.vertcoin.org/)** — Official explorer.
- **[BackPoW Vertcoin](https://backpow.com/Vertcoin)** — Verthash GPU profitability, the practical test of whether ASIC resistance still holds economically.
- **[MiningPoolStats VTC](https://miningpoolstats.stream/vertcoin)** — Pool listing.

#### Radiant (RXD)

- **[radiant-node](https://github.com/RadiantBlockchain/radiant-node)** — Official node for the SHA512/256-based chain ([project site](https://radiantblockchain.org/)).
- **[Radiant Explorer](https://radiantexplorer.com/)** — Block explorer.
- **[Hashrate.no RXD](https://www.hashrate.no/coins/RXD)** — Per-GPU measured performance.
- **[BackPoW Radiant](https://backpow.com/Radiant)** — Mining calculator and CoP.
- **[MiningPoolStats RXD](https://miningpoolstats.stream/radiant)** — Pools and difficulty.

#### Raptoreum (RTM)

- **[Raptoreum](https://github.com/raptor3um/raptoreum)** — Official node for the GhostRider CPU algorithm ([project site](https://raptoreum.com/)).
- **[Raptoreum Explorer](https://explorer.raptoreum.com/)** — Official explorer.
- **[cpuminer-opt](https://github.com/JayDDee/cpuminer-opt)** and **[SRBMiner-Multi](https://github.com/doktor83/SRBMiner-Multi)** — GhostRider miners.
- **[BackPoW Raptoreum](https://backpow.com/Raptoreum)** — CPU profitability with the smartnode reward split accounted for.
- **[MiningPoolStats RTM](https://miningpoolstats.stream/raptoreum)** — Pool distribution.

#### Handshake (HNS)

- **[hsd](https://github.com/handshake-org/hsd)** — Official full node and wallet for the decentralised naming chain ([project site](https://handshake.org/)).
- **[ShakeShift](https://shakeshift.com/)** — Explorer and name-auction browser.
- **[F2Pool HNS](https://www.f2pool.com/coin/handshake)** — Main public pool.
- **[BackPoW Handshake](https://backpow.com/Handshake)** — Blake2b+SHA3 ASIC economics.
- **[MiningPoolStats HNS](https://miningpoolstats.stream/handshake)** — Pools and hashrate.

#### Aeternity (AE)

- **[Aeternity Node](https://github.com/aeternity/aeternity)** — Official Erlang node for the Cuckoo Cycle chain ([project site](https://aeternity.com/)).
- **[AEScan](https://aescan.io/)** — Official explorer.
- **[MiningPoolStats AE](https://miningpoolstats.stream/aeternity)** — Pools and difficulty.
- **[BackPoW Aeternity](https://backpow.com/Aeternity)** — Cuckoo Cycle GPU profitability and CoP.
- **[Hashrate.no AE](https://www.hashrate.no/coins/AE)** — Per-card benchmarks.

#### Siacoin (SC)

- **[Sia](https://sia.tech/)** — Storage network whose blocks are mined with Blake2b; renting and mining economics interact.
- **[Sia Core](https://github.com/SiaFoundation/core)** and **[hostd](https://github.com/SiaFoundation/hostd)** — Consensus library and storage-host daemon.
- **[Siascan](https://siascan.com/)** — Official explorer with host and contract data.
- **[BackPoW Sia](https://backpow.com/Sia)** — Blake2b ASIC profitability and breakeven power price.
- **[MiningPoolStats SC](https://miningpoolstats.stream/siacoin)** — Pool listing.

---

## Research, News & Community

- **[Braiins Academy](https://learn.braiins.com/en)** — Structured explainers on difficulty, pool payout schemes, hashrate derivatives and firmware tuning.
- **[Hashrate Index Research](https://hashrateindex.com/)** — Market reports on hashprice, rig ROI and industrial mining economics.
- **[Open Source Miners United Wiki](https://osmu.wiki/)** — Community knowledge base for miner configuration and troubleshooting.
- **[BitcoinTalk Mining Board](https://bitcointalk.org/index.php?board=14.0)** — The oldest continuously active mining forum, still where hardware faults and firmware issues surface first.
- **[Stratum V2 Protocol](https://stratumprotocol.org/)** — Specification, rationale and implementation status for the modern stratum protocol.

---

## Contributing

Contributions are welcome. Before opening a Pull Request:

1. Read the [contribution guidelines](CONTRIBUTING.md).
2. Confirm the project is alive: a working site or a repository with commits in the last 12 months.
3. Link to the canonical domain or official repository — never a referral, affiliate or tracking URL.
4. Keep descriptions factual and specific about what the tool does.

Broken links, dead projects and rebranded domains are as useful to report as new entries. Open an issue if you find one.

---

## License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, this curation is dedicated to the public domain under **Creative Commons CC0 1.0 Universal**.
