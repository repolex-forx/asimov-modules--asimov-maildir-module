# Repolex Knowledge Graph of asimov-modules/asimov-maildir-module

RDF knowledge graph data for [asimov-modules/asimov-maildir-module](https://github.com/asimov-modules/asimov-maildir-module), parsed by [repolex](https://repolex.ai).

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
rlex download asimov-modules/asimov-maildir-module
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── bc79afd1c1a28d66c325b9d2a8ebabd0486dcab6
│   │       └── chunk-001.nq.gz
│   ├── lsp
│   │   └── bc79afd1c1a28d66c325b9d2a8ebabd0486dcab6.nq.gz
│   └── repolex
│       └── bc79afd1c1a28d66c325b9d2a8ebabd0486dcab6
│           └── chunk-001.nq.gz
├── blob
│   ├── 10b359dd05935c73efb064470f9ecda90f6d28aa.nq.gz
│   ├── 1dfe80692fc1a039e15fcb2a667f86dad7708f91.nq.gz
│   ├── 2ceee01b073a9c93c5761c3149e5f54181b7b930.nq.gz
│   ├── 55f6ee0e088a9f73c7f1d574d412415db4c9f383.nq.gz
│   ├── 66faba7f50ae9bc6d49de8b7c845723f763b4804.nq.gz
│   ├── 6b23d61018f43b840f8d2ff3b45a1c02d76df38d.nq.gz
│   ├── 6e8bf73aa550d4c57f6f35830f1bcdc7a4a62f38.nq.gz
│   ├── 75e3b65f99b29f48ab230e3eab3de8d0b7a9229f.nq.gz
│   ├── 7885eeff583553342b8c228d7cd41580db0f2420.nq.gz
│   ├── 7a5364226712f21bd979339ecd38a4bcca3dfff7.nq.gz
│   ├── 88c55933f1b6e10caabcdcaae8841eac3250f335.nq.gz
│   ├── 8a14e4a507542e44c967752b0f11628e7fa1673d.nq.gz
│   ├── 91b2d175d4fa2be34cfa903eb8eb6b358c437d5e.nq.gz
│   ├── 9fe50de16e59d550235aa6d7d15ee12ddf054414.nq.gz
│   ├── a36fedab8db68b26a76fbbf1de1f549e4a12261b.nq.gz
│   ├── af9908b08f4b33c32a0080af73f53bc0fa0cdce4.nq.gz
│   ├── bb89b6cb77cb0c08b3845ad2b4495de3d52a7cc1.nq.gz
│   ├── c7c328bd9a87e502454085e0c596a1e34d246d8b.nq.gz
│   ├── cf42f6893594e2f8be2b722de51123d65e4d61c4.nq.gz
│   ├── e3e57a8ce4ccbf74759a6df8fa4a3980ff1c9209.nq.gz
│   ├── ee4d9362508d63f9e156fe9ee1b11ebc1a3e86d6.nq.gz
│   ├── efb98088164f5786b17e83ed384971fc3c74f93c.nq.gz
│   └── f86c6cc8efcf7e9c30a72a2acf754c263f71e683.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── dep
│   └── bc79afd1c1a28d66c325b9d2a8ebabd0486dcab6.nq.gz
├── filetree
│   └── bc79afd1c1a28d66c325b9d2a8ebabd0486dcab6.nq.gz
└── tag
    └── tag.nq.gz

13 directories, 31 files
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

[asimov-modules/asimov-maildir-module](https://github.com/asimov-modules/asimov-maildir-module)

---
*Parsed on 2026-09-28 by [repolex](https://repolex.ai)*
