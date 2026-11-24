# This fork: PCBCraft for the Dataverse

This is the Dataverse's fork of [PCBCraft](https://github.com/tangency-labs/pcbcraft) by Tangency Labs
(MIT OR Apache-2.0). The Dataverse runs its command line on the main server, headless, as the `pcbcraft` engine.
Its commands are reached through `pcbcraft-cli mcp` (the MCP tools list_commands, describe_command, execute…).

## Branches

| Branch | What it is |
|---|---|
| `main` | Exactly PCBCraft's `main`. Never commit here; it is only updated from them. |
| `dataverse` | `main` plus our own commits on top. This is what the Dataverse builds. |

Each of our changes is one commit on `dataverse`, so it replays cleanly on every new PCBCraft and can be offered
back as a pull request. PCBCraft's rules for contributors (`AGENTS.md`, `CONTRIBUTING.md`) apply to our commits too.

## Keeping up with PCBCraft

`.github/workflows/dataverse.yml` runs every Monday (and on demand from the Actions tab): it updates `main` from
PCBCraft, replays our commits on `dataverse` (opening an issue when one no longer applies), builds the command line,
runs its tests and attaches the program as `dataverse-pcbcraft-cli` (Linux x86-64).

## Our changes

| Commit | What | Offered upstream? |
|---|---|---|
| (none yet: this branch only adds this file and the workflow) | | |

## Name

Our build is called `dataverse-pcbcraft-cli` and is described as "based on PCBCraft by Tangency Labs".
