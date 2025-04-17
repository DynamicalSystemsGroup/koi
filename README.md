# Welcome to the KOI project!

KOI (Knowledge Organization Infrastructure) is a collective research effort across BlockScience, Metagov, and RMIT. This repo is intended to be a jumping off point to find resources and information related to the project.

The repositories below are roughly divided into KOI versions 1 - 3, indicating which iteration the core infrastructure is on (not necessarily how recent or in use it is). Version 1 is BlockScience's KMS (Knowledge Management System), which started the KOI research initiative. This version predates RIDs and powers a KMS-GPT Slack bot (kms-slack) as well as a web interface (kms-api, kms-web) using a cloud based knowledge processing pipeline (not all repos are publicly available). Version 2 is Metagov's KOI Pond project, which was the next iteration of the KOI technology. This is based upon the monolithic API (koi-api) and RID v2, with primitive knowledge sensors for a few platforms (kms-tools). Version 3 is the current research effort being led by BlockScience and RMIT (through the Telescope project). RIDs have been codified into v3 (rid-lib, rid-registry), and a prototype of a decentralized node based network architecture is being developed (koi-sensors, etc.). 

Repositories are (again roughly) sorted into four tracks: the core infrastructure, and the involved orgs: BlockScience, Metagov, and RMIT. This generally indicates under which org the work for that repository was done. Past work on KOI v1/2 could also be considered core infrastructure, but I've only put the KOI v3 repos which are intended for broader usage there. As development of v3 continues under BlockScience and RMIT continues, more resources will be spun out into the core infrastructure track. The goal is for each org's individual KOI implementation to be built on top of the core infrastructure, and to jointly contribute to its research and development.

## Code Repository Inventory
- Core Infrastructure
  - [rid-lib](https://github.com/BlockScience/rid-lib/) (KOI v3) - Implementation of RID v3 specification, and extended features (RID manifests, caching).
  - [rid-registry](https://github.com/BlockScience/rid-registry) (KOI v3) - Registry of supported RID types to be implemented by rid-lib.
  - [koi-net](https://github.com/BlockScience/koi-net) (KOI v3) - Implementation of KOI-net protocol, currently in beta release.
- BlockScience
  - [koi-net-coordinator-node](https://github.com/BlockScience/koi-net-coordinator-node) (KOI v3) - KOI-net coordinator node implementation.
  - [koi-net-slack-sensor-node](https://github.com/BlockScience/koi-net-slack-sensor-node) (KOI v3) - KOI-net Slack sensor node implementation.
  - [koi-net-hackmd-sensor-node](https://github.com/BlockScience/koi-net-hackmd-sensor-node) (KOI v3) - KOI-net HackMD sensor node implementation.
  - [koi-coordinator](https://github.com/BlockScience/koi-coordinator) (KOI v3 prototype) - Previous development of coordinator node prototypes. Integrates with sensors below.
  - [koi-sensors](https://github.com/blockScience/koi-sensors) (KOI v3 prototype) - Previous development of sensor node prototypes exploring new KOI network architecture. Using latest version of rid-lib.
  - [kms-slack](https://github.com/BlockScience/kms-slack) (KOI v1) - KMS-GPT Slack bot chat interface implementing its own vectorstore.
  - [kms-web](https://github.com/BlockScience/kms-web) (KOI v1) - Upgraded KMS website with KMS-GPT chat interface and text search.
  - [kms-api](https://github.com/BlockScience/kms-api) (KOI v1) - Backend for upgraded KMS website.
  - [kms-identity](https://github.com/BlockScience/kms-identity) (pre-KOI v2) - Prototype implementing RID v1 with graph primitives.
- Metagov
  - [koi-api](https://github.com/BlockScience/koi-api) (KOI v2) - Metagov KOI instance with RID v2 support including graph, cache, and vectorstore subsystems. All integrated in a single monolithic API that isn't very composable.
  - [kms-tools](https://github.com/metagov/kms-tools) (KOI v2) - Sensors and interfaces for Metagov KOI, including KOI-GPT, Slack listener and backfill, and websites.
- RMIT
  - [slack-telescope](https://github.com/metagov/slack-telescope) (KOI v3) - RMIT tool to manage consent based ethnographic research collecting Slack messages. "KOI-lite" stand alone implementation with a built in cache and limited graph capabilities. Using latest version of rid-lib.
  - [koi-obsidian-plugin](https://github.com/metagov/koi-obsidian-plugin) (KOI v3) - Obsidian plugin for syncing knowledge objects from KOI-net nodes into Markdown documents.
 
## Other Resources
- Documentation
  - [RID v3 Protocol Documentation](https://github.com/BlockScience/rid-lib/blob/main/README.md) 
- Publications
  - [Metagov KOI Pond project homepage](https://metagov.org/projects/koi-pond)
  - ["KOI-Pond: The creation of a synthetic deme" - Ellie Rennie (RMIT)](https://ellierennie.medium.com/koi-pond-the-creation-of-a-synthetic-deme-999a6f1f3426)
  - [Metagov Project Spotlight: KOI Pond](https://metagov.substack.com/p/metagov-project-spotlight-koi-pond)
  - ["A Language for Knowledge Networks" - Michael Zargham & Ilan Ben-Meir (BlockScience)](https://blog.block.science/a-language-for-knowledge-networks/)
  - ["Objects as Reference" - Orion Reed (BlockScience)](https://blog.block.science/objects-as-reference-toward-robust-first-principles-of-digital-organization/)
