# zed-pkg/zed-mcp-server.rs#2 — docs: add AGENTS.md and fleet sops env layout

head: chore/agents-md-and-sops-env  base: main  author: ORESoftware  updated: 2026-08-27T02:58:01Z
dir: /Users/maca5/codes/.claude-fleet/scratch/merge/zed-pkg_zed-mcp-server.rs__2

## conflicted files
- justfile

## base (main) last 8 commits
95ea25f DEN-965: harden zed-pkg MCP client and provider parity
7f5e8fd Merge pull request #3 from zed-pkg/agent/ores-sops-ensure-dec-20260828
b83e7e4 Cover remaining env/dec creation paths with ores-sops ensure-dec.
0c581dc Refuse unguarded env/dec mkdir before ores-sops.
9e672ea feat: add hardened read-only zed-pkg MCP server

## head (chore/agents-md-and-sops-env) last 8 commits
e6f3eb5 docs: point AGENTS.md at the parent my-ai contract and codes symlink
8e9f03f docs: add functional programming coding patterns to AGENTS.md
b7421da docs: add AGENTS.md and fleet sops env layout
9e672ea feat: add hardened read-only zed-pkg MCP server

## merge-base: 9e672ea21dfab2482898041ddc8818d400018444

## PR diff stat (merge-base..head)
 .envrc                              |   7 +
 .github/workflows/secrets-audit.yml |  32 +++
 .gitignore                          |  17 ++
 .just/dotenv.py                     |  87 +++++++
 .just/env.just                      | 461 ++++++++++++++++++++++++++++++++++++
 .sops.yaml                          |  27 ++-
 AGENTS.md                           | 105 ++++++++
 env/README.md                       |  28 +++
 env/enc/prod.env.enc                |  10 +
 flake.nix                           |  13 +-
 justfile                            |  76 +++---
 11 files changed, 827 insertions(+), 36 deletions(-)

## base diff stat (merge-base..base)
 .github/workflows/ci.yml |   13 +-
 Cargo.lock               | 1581 +++++++++++++++++++++++++++++++++++++++++++---
 Cargo.toml               |   11 +-
 README.md                |   74 ++-
 justfile                 |    4 +-
 mcp-fleet-profile.json   |  214 +++++++
 src/http.rs              |   10 +
 src/main.rs              |   21 +-
 src/spec.rs              |   61 ++
 tests/stdio_parity.rs    |  255 ++++++++
 10 files changed, 2135 insertions(+), 109 deletions(-)

## merge output
Auto-merging justfile
CONFLICT (content): Merge conflict in justfile
Automatic merge failed; fix conflicts and then commit the result.
