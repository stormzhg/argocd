# CMC Management Service on Argo CD (GitOps template)

Template repo for moving a `mstrcli`-installed CMC Management Service to Argo CD,
without reinstalling. **Follow RUNBOOK.md (shipped with this template) step by step.**

| Path | What it is | You |
| --- | --- | --- |
| `apps/` | Argo CD Applications: add-ons (wave 0), Redis + Elasticsearch (wave 1), operator (wave 2); environments (wave 3) are generated | Replace `<REPO_URL>` and `<BRANCH>` (§4d). Delete the files of services you don't have. |
| `charts/` | Product charts | Unpack from the StrategyOne package (§4a). Never edit. |
| `services.json` | Image list | Copy from the package (§4a). Never edit. |
| `values/*.yaml` | Helm values (**samples**) | Overwrite with the values exported from your cluster (§4b). |
| `envs/<env>/environment.yaml` | Environments | Generated from your cluster (§4c). |
| `examples/` | What generated files look like | Reference only; never applied. |

Never commit secrets: no customer profile, no TLS keys, no registry or Redis passwords.
