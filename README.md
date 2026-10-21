# Repolex Knowledge Graph of scverse/spatialdata-integration-testing

RDF knowledge graph data for [scverse/spatialdata-integration-testing](https://github.com/scverse/spatialdata-integration-testing), parsed by [repolex](https://repolex.ai).

> **Note**: This data is experimental and subject to change without notice.

## How to use this data

The easiest way to get started is to install the [rlex](https://github.com/repolex-ai/rlex) query tool:

```bash
cargo install --git https://github.com/repolex-ai/rlex
```

Verify the install:

```bash
rlex --help
```

**rlex is designed to be used primarily by LLMs in a terminal.** Start up your favorite AI assistant and ask it to use rlex. It handles the SPARQL — you just ask questions in plain English.

To load this repo's data:

```bash
rlex download scverse/spatialdata-integration-testing
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── 4982079e516f58c51b19c93bb60aac178a2c4512
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── 4982079e516f58c51b19c93bb60aac178a2c4512
│           └── chunk-001.nq.gz
├── blob
│   ├── 01e1a5754acf73a71b2f9c1d99579f60d223267b.nq.gz
│   ├── 020ef1c4ddb6b1056992808c0e66a410812ac6d1.nq.gz
│   ├── 02cd55a257d8c51e426c5d07101162483164b8d0.nq.gz
│   ├── 095dafda64a0f319f8ac27db4ab2cf834be8ac6f.nq.gz
│   ├── 0e5726b76aafa1b78d0b090c104f0fddad2efd21.nq.gz
│   ├── 1b9aef7befd68dce4e52fc493d68703c36e1c075.nq.gz
│   ├── 21a88d21bea5db4f7f1097b4ec4ea60ea58e87d6.nq.gz
│   ├── 22e5d134a7f4eb9a38708cd5347803631b3a56e5.nq.gz
│   ├── 40c289345cc3abe4b8018f46cbbd21560219a3e2.nq.gz
│   ├── 42cc01eda94822a3925c614781652098505b8540.nq.gz
│   ├── 5008ddfcf53c02e82d7eee2e57c38e5672ef89f6.nq.gz
│   ├── 519040ae90d6745b587fe8da6bd520f2d0cdde01.nq.gz
│   ├── 58aef2117380b3e1d2fcdd45e546f676fcaa9288.nq.gz
│   ├── 718a7582bf9d34aa23d461aeb010c6fcf80eda4e.nq.gz
│   ├── 71b21233a7d33a1b33d06a447a171a8f4eefa2e5.nq.gz
│   ├── 7409abb6b69e2ab64d06e68754bb656a2c6c0d56.nq.gz
│   ├── 7d1034c78e3c8b80ba81aebb59f783db9b2485ef.nq.gz
│   ├── 7f0033265565f9896dababb3aef7a0f2304f3e28.nq.gz
│   ├── 82544d16f8ad44854c51dd7dc586ce95610e663f.nq.gz
│   ├── 84ca9dfa4c6039140ed93517ab17c2f34e699297.nq.gz
│   ├── 8fff463644885ace84a588b422cfaceb5cec11d1.nq.gz
│   ├── a2700544c26c043c572345ff95f93b7347367cf2.nq.gz
│   ├── a8b3f98ec2f33aa4db4f2e7bf2750c099ce34871.nq.gz
│   ├── ac8b11083cffa79acc33d4f0d4ce1d80fb89ad6b.nq.gz
│   ├── b7a2897067339cbe10fb263b6056c11c16ef0e70.nq.gz
│   ├── b95f8570556fa38a5eddfcc728360e4e8283fda7.nq.gz
│   ├── bc18b9cb52df6f3c38fa2fbbe24a984af0c0792e.nq.gz
│   ├── bf3ed503eab75285fc343dfede5d880c8143ca1b.nq.gz
│   ├── c067584508ea8f88bd5451432e65e158abc9b9e4.nq.gz
│   ├── c489013a55f624867729a25b8fa355be98135191.nq.gz
│   ├── d0a7e3f7edbacdfae56dd27b722ed939d9e9805e.nq.gz
│   ├── d6aa8ac3d75709d7bf22ae0b91ad98c2dcd4f173.nq.gz
│   ├── d712df841ba00d0a54ab201d33c163eb9b807d47.nq.gz
│   ├── dd8c9869cb9e9381b86015a8581213bde3507f0f.nq.gz
│   ├── e5b4ee794a306ff4af1c108c5e06105949d841b2.nq.gz
│   ├── e69de29bb2d1d6434b8b29ae775ad8c2e48c5391.nq.gz
│   ├── e8a4cdd45d65abe5caf95830a33b155bb9f54c63.nq.gz
│   ├── ebd2786794ac0d3ac0fe6a3fafd5a0019f31f0dd.nq.gz
│   ├── f0cb8ce341a9c6a802b92e2ff3fbde97ff2d64b8.nq.gz
│   ├── f0f8f8c40831fc7c86a48001a079e8f18038f0a3.nq.gz
│   └── fcb55c3511a39037f91e8a1ec8dc31d71284dcb3.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── 4982079e516f58c51b19c93bb60aac178a2c4512.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

12 directories, 48 files
```

| Directory | What it contains |
|-----------|-----------------|
| `blob/` | Per-file AST graphs, content-addressed by git blob SHA. Each file in the source repo gets its own graph. |
| `aggregate/ast/` | Combined AST graph per parsed commit. Merges all blob graphs for a snapshot of the entire codebase at that point. |
| `aggregate/lsp/` | Language Server Protocol enrichment: resolved symbols, definitions, references, and type information. |
| `aggregate/dataflow/` | Interprocedural data flow edges between functions and modules. |
| `aggregate/repolex/` | Combined graph (AST + LSP + dataflow) per commit. |
| `commit/` | Git commit metadata (author, date, message, parent links). |
| `branch/` | Branch metadata. |
| `tag/` | Tag metadata. |
| `filetree/` | File tree snapshots per commit (which files existed and their blob SHAs). |
| `audit/` | Code architecture and graph audit reports per commit. |

## Source repository

[scverse/spatialdata-integration-testing](https://github.com/scverse/spatialdata-integration-testing)

---
*Parsed on 2026-10-21 by [repolex](https://repolex.ai)*
