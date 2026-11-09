# Repolex Knowledge Graph of optonaut/ActiveLabel.swift

RDF knowledge graph data for [optonaut/ActiveLabel.swift](https://github.com/optonaut/ActiveLabel.swift), parsed by [repolex](https://repolex.ai).

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
rlex download optonaut/ActiveLabel.swift
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── 36949c1a69ef8b40574da20c9e24b115f387b1cf
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── 36949c1a69ef8b40574da20c9e24b115f387b1cf
│           └── chunk-001.nq.gz
├── blob
│   ├── 073d4532931c2f125d72672ab80c9e9d8adf5f99.nq.gz
│   ├── 18d981003d68d0546c4804ac2ff47dd97c6e7921.nq.gz
│   ├── 1c547367212d3b3f39fa4e1152a8e4af34b7f933.nq.gz
│   ├── 2a9926bf37838f66182a7e6d34783821b0e06b54.nq.gz
│   ├── 2e721e1833f03bb0e1b962a84491d7e43e3fef9c.nq.gz
│   ├── 311e4a1c00a8c00537824809f1d525e0daa818d4.nq.gz
│   ├── 3d9795f39ce8c40325720708def51693d04cfca2.nq.gz
│   ├── 3dccd3ab3701b1b5d0969e70640f10c4bd5e27c7.nq.gz
│   ├── 40c6215d906736d7b2a439c17cf9ee0776580474.nq.gz
│   ├── 4a109c87e7eec8b8b55bde2bbb2e32f55664dc13.nq.gz
│   ├── 55ee66fc24771fe6d53ba63be62e8b5ac030ee21.nq.gz
│   ├── 55f1da8b64c424eed45ddcc0f348215ef519a0f5.nq.gz
│   ├── 56b7226a65838c9c995d3ac105dd2b9e1721a317.nq.gz
│   ├── 5a813f1b3a71b55d2ed827e9000229549ceea80c.nq.gz
│   ├── 6fa9267c6de6ed0b53799f25485f817b26d4faed.nq.gz
│   ├── 7ec151cad37e959b4df8b780a63a9bb76891e78c.nq.gz
│   ├── 819e07a22435f1e8efcbdd1d1c062deef0e501b1.nq.gz
│   ├── 84fde9d5100b37585c7ad76b2dc7754241467608.nq.gz
│   ├── 8897133ed5a594376266c5512c78f4835cac14eb.nq.gz
│   ├── 9da442e945d2221afc7129b00ff17ecb7ed588a9.nq.gz
│   ├── b2b5261cc4fa027661756e80c4b2725b2f278c05.nq.gz
│   ├── ba72822e8728ef2951005e49b6c27a2f1da6572d.nq.gz
│   ├── ca23c84f4c4e0c3bd1dc74cd562b3bf0aba22335.nq.gz
│   ├── d6246ddfe0524cd4faaf1844a89be7a188ce112b.nq.gz
│   ├── ed4916d6d76ec059d77cc58dcd96d0315eea722c.nq.gz
│   ├── fe9bd7ab459a599b309c30ca8db2d1159f50f210.nq.gz
│   └── ff4722132eb83c733c1fabb69c7c0351985658f2.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── 36949c1a69ef8b40574da20c9e24b115f387b1cf.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

13 directories, 35 files
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

[optonaut/ActiveLabel.swift](https://github.com/optonaut/ActiveLabel.swift)

---
*Parsed on 2026-11-09 by [repolex](https://repolex.ai)*
