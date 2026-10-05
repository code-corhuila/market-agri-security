# market-agri-security

> Transversal security microservice: RS256 signing, JWKS and service tokens (Annex J)

Part of the **Marketplace Agricultural Huila** distributed system — team `marketplace-agricultural-huila`, Grupo 1.
Governance and documentation live in [`market-agri-docs`](https://github.com/code-corhuila/market-agri-docs).

## Branching

Three permanent branches. **None of them accepts a direct commit** — you enter through a child
branch and leave through a Pull Request.

```
develop  <--PR--  feat/... fix/... chore/...
qa       <--PR--  qa/...
main     <--PR--  release/...  hotfix/...
```

Promotion happens **by re-application** (`git cherry-pick -x`), never by merging one permanent
branch into another: `merge develop -> qa` and `merge qa -> main` do not exist in this model.

`main` requires **1 approval from `ariel5253`**. On `develop` and `qa` the team sets its own review
rule.

Full policy: `00-governance/branching-policy.md` in `market-agri-docs`.
