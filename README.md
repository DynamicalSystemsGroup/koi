# Welcome to the KOI project!

KOI (Knowledge Organization Infrastructure) is a collective research effort across Dynamical Systems Group, Metagov, and RMIT. This repo is intended to be a jumping off point to find resources and information related to the project.

The repositories below are roughly divided into KOI versions 1 - 3, indicating which iteration the core infrastructure is on.


## KOI v3 - "KOI-net"
Version 3 is the current research effort being led by Dynamical Systems Group and RMIT (through the Telescope project). RIDs have been codified into v3 (`rid-lib`, `rid-registry`), and a KOI-net protocol has been established for network based communication (`koi-net`).

## KOI v2 - "KOI Pond"
Version 2 is Metagov's KOI Pond project, which was the next iteration of the KOI technology. This is based upon the monolithic API (`koi-api`) and RID v2, with primitive knowledge sensors for a few platforms (`kms-tools`). 

## KOI v1 - "KMS"
Version 1 is Dynamical Systems Group's KMS (Knowledge Management System), which started the KOI research initiative. This version predates RIDs and powers a KMS-GPT Slack bot (`kms-slack`) as well as a web interface (`kms-api`, `kms-web`) using a cloud based knowledge processing pipeline (not all repos are publicly available). 


## Code Repository Inventory

- KOI-net (KOI v3)
  - Core Infrastructure
    - [`koi-net`](https://github.com/DynamicalSystemsGroup/koi-net) - Implementation of KOI-net protocol, currently in beta release. Includes boilerplate for node setup, network communication, RID caching, and knowledge processing.
    - [`koi-net-node-template`](https://github.com/DynamicalSystemsGroup/koi-net-node-template) - Template repo for creating new KOI-net nodes
    - [`rid-lib`](https://github.com/DynamicalSystemsGroup/rid-lib/) - Implementation of RID v3 specification, and extended features (RID manifests, caching).
    - [`rid-registry`](https://github.com/DynamicalSystemsGroup/rid-registry) - Registry of supported RID types to be implemented by rid-lib.
  - Node Implementations
    - [`koi-net-coordinator-node`](https://github.com/DynamicalSystemsGroup/koi-net-coordinator-node)
    - [`koi-net-slack-sensor-node`](https://github.com/DynamicalSystemsGroup/koi-net-slack-sensor-node)
    - [`koi-net-hackmd-sensor-node`](https://github.com/DynamicalSystemsGroup/koi-net-hackmd-sensor-node)
    - [`koi-net-github-sensor-node`](https://github.com/DynamicalSystemsGroup/koi-net-github-sensor-node)
    - [`koi-net-gdrive-sensor-node`](https://github.com/DynamicalSystemsGroup/koi-net-gdrive-sensor-node)
    - [`koi-net-debug-node`](github.com/DynamicalSystemsGroup/koi-net-debug-node)
    - [`koi-net-hackmd-processor-node`](https://github.com/DynamicalSystemsGroup/koi-net-hackmd-processor-node)
    - [`koi-net-github-processor-node`](https://github.com/DynamicalSystemsGroup/koi-net-github-processor-node)
  - Demos
    - [`koi-net-demo-v1`](https://github.com/DynamicalSystemsGroup/koi-net-demo-v1)
  - Related Projects
      - [`slack-telescope`](https://github.com/metagov/slack-telescope) - RMIT tool to manage consent based ethnographic research collecting Slack messages. "KOI-lite" stand alone implementation with a built in cache and limited graph capabilities. Using latest version of rid-lib.
      - [`koi-obsidian-plugin`](https://github.com/metagov/koi-obsidian-plugin) - KOI-net compatible partial node used by RMIT researchers to sync research data between KOI and Obsidian.
- KOI Pond (KOI v2)
  - [`koi-api`](https://github.com/DynamicalSystemsGroup/koi-api) - Metagov KOI instance with RID v2 support including graph, cache, and vectorstore subsystems. All integrated in a single monolithic API.
  - [`kms-tools`](https://github.com/metagov/kms-tools) - Sensors and interfaces for Metagov KOI, including KOI-GPT, Slack listener and backfill, and websites.
- KMS (KOI v1)
  - [`kms-slack`](https://github.com/DynamicalSystemsGroup/kms-slack) - KMS-GPT Slack bot chat interface implementing its own vectorstore.
  - [`kms-web`](https://github.com/DynamicalSystemsGroup/kms-web) - Upgraded KMS website with KMS-GPT chat interface and text search.
  - [`kms-api`](https://github.com/DynamicalSystemsGroup/kms-api) - Backend for upgraded KMS website.
  - Prototypes
    - [`kms-identity`](https://github.com/DynamicalSystemsGroup/kms-identity) (pre-KOI v2) - Prototype implementing RID v1 with graph primitives.
 
## Other Resources
- Documentation
  - [RID v3 Protocol Documentation](https://github.com/DynamicalSystemsGroup/rid-lib/blob/main/README.md) 
- Publications
  - [Metagov KOI Pond project homepage](https://metagov.org/projects/koi-pond)
  - ["KOI-Pond: The creation of a synthetic deme" - Ellie Rennie (RMIT)](https://ellierennie.medium.com/koi-pond-the-creation-of-a-synthetic-deme-999a6f1f3426)
  - [Metagov Project Spotlight: KOI Pond](https://metagov.substack.com/p/metagov-project-spotlight-koi-pond)
  - "A Language for Knowledge Networks" - Michael Zargham & Ilan Ben-Meir (Dynamical Systems Group)
  - "Objects as Reference" - Orion Reed (Dynamical Systems Group)objects-as-reference-toward-robust-first-principles-of-digital-organization/)
  - Digital Infrastructure Research & Development: KOI Network Protocol x Project Interlay
