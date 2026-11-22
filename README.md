# Repolex Knowledge Graph of explosion/preshed

RDF knowledge graph data for [explosion/preshed](https://github.com/explosion/preshed), parsed by [repolex](https://repolex.ai).

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
rlex download explosion/preshed
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   ├── 18eb82ba07dde69ab12f2271ee3da4cd5e94039a
│   │   │   └── chunk-001.nq.gz
│   │   └── 1d274ae9601396830ae340f501ee0a63a2c63239
│   │       └── chunk-001.nq.gz
│   ├── lsp
│   │   └── 1d274ae9601396830ae340f501ee0a63a2c63239.nq.gz
│   └── repolex
│       ├── 18eb82ba07dde69ab12f2271ee3da4cd5e94039a
│       │   └── chunk-001.nq.gz
│       └── 1d274ae9601396830ae340f501ee0a63a2c63239
│           └── chunk-001.nq.gz
├── blob
│   ├── 01763013fd4a763fe93c7887ecd9ae93ac45db35.nq.gz
│   ├── 0b1d6d0253ca541544c0cd9281472d102c352e90.nq.gz
│   ├── 0d42cd6a5aa2c4b807097680d5f4613987d9af12.nq.gz
│   ├── 128fa0701f53a150d271d30695bd874cad17dd39.nq.gz
│   ├── 176756ef133c020623369feab3332a2f08eee8e6.nq.gz
│   ├── 1d27cb45321a24589c99d85346bb5a08bfecfbbe.nq.gz
│   ├── 2d65053a8ecb1d7b26ffc038d21159ce8bfcfb70.nq.gz
│   ├── 2f8e68147c3924e450f4fb3519bda9f7a75c3b66.nq.gz
│   ├── 3392cefc9e3ddb6b3d91435861a28c00f37f9a30.nq.gz
│   ├── 33bc131f4561a57bfbe695c780ddb6d46f5aafe0.nq.gz
│   ├── 3ef060b107ef4085d8b26f24353cff981843d5e0.nq.gz
│   ├── 47732a9531cbbddc8035ec21a7816aa46833f23d.nq.gz
│   ├── 4fe0ef9a9b21859dea9fd834ce3d2fcf23bad2e0.nq.gz
│   ├── 5921f177ba61b41ad1ae6025455b198cb632b973.nq.gz
│   ├── 5d1c4e4d0f9977f5a0f39a56ab0dac7159fbf902.nq.gz
│   ├── 5d93f416bd96cac18de8e700fd227b7e015f7a3c.nq.gz
│   ├── 6513e67375cdff0cc6d6aeca394ebeeb7649e598.nq.gz
│   ├── 6925af16d70a80b3acbfe1236290c8d03670fc3f.nq.gz
│   ├── 6c8acd6a26393da32bb30badb2243f08c1a72222.nq.gz
│   ├── 7d6b183e03afd9f60e28146623f6e02248050b30.nq.gz
│   ├── 9543aeedcf8e6830c5e1160983abb4d226e7c987.nq.gz
│   ├── 95dc1bd269703235fbf33a230c375ef38ad3fc6b.nq.gz
│   ├── 9be27831cfd3cbae5b3ad2e3d7a1996dee3b3518.nq.gz
│   ├── a55014485a1e94a14df8dfaf1bce1c2921d047c3.nq.gz
│   ├── a72d54c866db7cb2be01c832f24876bce7005512.nq.gz
│   ├── a8efff9475abdaec16bd3c2cfc69ebef2caa40db.nq.gz
│   ├── b101d371ba6168f14c2ef7e5e0801572481c84a3.nq.gz
│   ├── b1091eaa320cefa3705f13d7b15c9921e461c8a4.nq.gz
│   ├── b1e363211114f2476f916f7387e72a57185e0592.nq.gz
│   ├── b5f25f7f1ffa2e3bc4543faf97693db71e54a0d5.nq.gz
│   ├── bade909b81bd6fd763a58bbd81c1f69b3b582985.nq.gz
│   ├── c114bf7750af1c7387b3373f82e0c8f953964716.nq.gz
│   ├── cf30f72c5352457167c577bcd5104648f998c339.nq.gz
│   ├── d29375bf3ed1576f96165c1b50fb7a2e2625c15b.nq.gz
│   ├── d615e3931cf86f8e47db2a70511186c9243abce8.nq.gz
│   ├── e69de29bb2d1d6434b8b29ae775ad8c2e48c5391.nq.gz
│   ├── eea3db5b44654ad97422dc41ba5b06200641b4d3.nq.gz
│   ├── fb75265ddc1253f751a5574df01c0f97aa142411.nq.gz
│   └── fbe31c49c6a4de5395a4c4b4a4d89b1d4855b697.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── dep
│   └── 1d274ae9601396830ae340f501ee0a63a2c63239.nq.gz
├── filetree
│   ├── 18eb82ba07dde69ab12f2271ee3da4cd5e94039a.nq.gz
│   └── 1d274ae9601396830ae340f501ee0a63a2c63239.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

17 directories, 52 files
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

[explosion/preshed](https://github.com/explosion/preshed)

---
*Parsed on 2026-11-22 by [repolex](https://repolex.ai)*
