# MAJOR//MINOR repository conventions

[Public project map](profile/README.md) · [Research and publications](https://majorminor.xyz)

## Taxonomy

| Prefix | Scope |
|---|---|
| `research-*` | Independently published research, benchmarks, and substantial studies. |
| `tools-*` | Reusable software and products with their own maintenance or release lifecycle. |
| `recipes-*` | Reproducible model, hardware, and configuration recipes with pinned inputs. |
| `lab-*` | Active experimental work that has not been promoted to a public research artifact. |
| `internal-*` | Private infrastructure, websites, and editorial systems when a rename has no deployment cost. |

Existing deployment-connected websites and client projects keep their current names until a migration is justified. The special `.github` and account-profile repositories are presentation infrastructure.

## Repository boundaries

Create a standalone repository for an independent product, reusable tool, citable research artifact, or distinct release lifecycle. Keep smaller studies, E0xx iterations, runs, failed experiments, and supporting work inside their owning research or lab repository. An experiment identifier belongs in its ledger and manifest; it need not become the repository name.

Keep raw evidence, failures, frozen manifests, tags, and release provenance. Consolidation requires preserving useful history and clearly documenting ownership. Archive obsolete repositories before considering removal. Do not delete or force-push to make the repository list cleaner.

## Metadata

Use concise descriptions that state the project's actual purpose and scope. Apply only relevant topics: `major-minor`, `research`, `benchmark`, `agents`, `model-compression`, `local-llm`, `recipe`, and `tool`, with project-specific topics where helpful. Public profile links should lead to meaningful public projects; private infrastructure is not advertised as public research.

## Local clone integrity

After a repository rename, update every clone/worktree's origin to the canonical GitHub URL and verify fetch, push URL, local branch/tracking state, and preservation of uncommitted work. Shared worktrees use their common Git configuration. Update live links and integration references; retain historical/raw evidence references when rewriting would compromise provenance.

## Recommended pins

1. `research-devin-agent-benchmark`
2. `research-4b-agent-models`
3. `research-7b-8b-agent-scaling`
4. `research-luna-5.6-vs-6`
5. `tools-talaria`
6. `tools-experiment-plates`

The current namespace is a GitHub user account. `.github/profile/README.md` is ready for an organization profile if the account structure changes; the `majorminorlabs/majorminorlabs` README supplies the visible user profile now.
