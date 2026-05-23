# pleme-io

> The typed substrate that compounds its own ability across the open-source commons.

```
192 typed CI/CD primitives · 30+ categories · 5 reusable workflows
14 substrate composition workflows · 5 institutional skills
ALL auto-published to free public GitHub-hosted compute · $0/month
```

## Pick your entry point

### 👋 I want to use pleme-io actions in MY repo

```yaml
# .github/workflows/auto-release.yml — 6 lines, that's it
on:
  push: { branches: [main] }
jobs:
  release:
    uses: pleme-io/substrate/.github/workflows/auto-release.yml@main
    secrets: inherit
```

This polymorphic dispatcher detects your repo's language (Rust /
npm / Python / Helm / caixa) and routes to the right
bump+commit+tag+publish pipeline. **Free public CI handles the rest.**

→ [Full catalog browser](https://github.com/pleme-io/actions#readme)
→ [Operator CLI](https://github.com/pleme-io/releaser)
→ [How it works](https://github.com/pleme-io/substrate/blob/main/docs/INTERLOCK.md)

### 🛠️ I want to contribute a new action

```bash
cargo install pleme-io-releaser
pleme-release onboard          # scaffold the 3-workflow surface
```

Or by hand:

1. Author `your-action/action.yml` + `your-action/run.tlisp`
   ([5-section canonical shape](https://github.com/pleme-io/blackmatter-pleme/blob/main/skills/pleme-io-pattern-core/SKILL.md))
2. Open a PR — auto-bump publishes it within minutes on merge.
3. Catalog + per-action docs regenerate automatically.

→ [Contribution guide](https://github.com/pleme-io/actions/blob/main/CONTRIBUTING.md)
→ [Pattern-core skill](https://github.com/pleme-io/blackmatter-pleme/blob/main/skills/pleme-io-pattern-core/SKILL.md)

### 🧭 I want to understand the architecture

The pleme-io substrate is built on:

- **One prime directive**: NO SHELL (everything in Rust + tatara-lisp + Nix + YAML)
- **One compounding directive**: every pattern that appears ≥2 times becomes a macro/library
- **One auto-release directive**: every packaged artifact ships on merge, default-on
- **One typescape**: the Rust type system IS the substrate's source of truth

Theory + frame + 12 pillars:
→ [pleme-io/theory](https://github.com/pleme-io/theory)

The unified vision for the action layer:
→ [substrate/docs/INTERLOCK.md](https://github.com/pleme-io/substrate/blob/main/docs/INTERLOCK.md)

## The published toolchain

Every tool below is itself dogfood-published via the same directive:

| Tool | What | Where |
|---|---|---|
| **actions** | 192 typed GH action primitives | [github.com/pleme-io/actions](https://github.com/pleme-io/actions) |
| **substrate** | Reusable workflows + Nix patterns + typed catalog | [github.com/pleme-io/substrate](https://github.com/pleme-io/substrate) |
| **releaser** | Operator CLI (`pleme-release detect/plan/onboard`) | [crates.io/crates/pleme-io-releaser](https://crates.io/crates/pleme-io-releaser) |
| **pleme-doc-gen** | Rust generator for catalog + docs | [crates.io/crates/pleme-doc-gen](https://crates.io/crates/pleme-doc-gen) |
| **tatara-lisp** | Tatara Lisp runtime (every tlisp action uses it) | [crates.io/crates/tatara-lisp](https://crates.io/crates/tatara-lisp) |
| **engenho** | Typed Rust-native K8s runtime (15 sibling crates) | [github.com/pleme-io/engenho](https://github.com/pleme-io/engenho) |

## What you get adopting the directive

Every adopting repo gets, with **zero ongoing infrastructure cost**:

- ✅ Auto-bump semver on every substantive push
- ✅ Tag + GH Release with auto-generated notes
- ✅ Publish to the right public registry (crates.io / npmjs / pypi / OCI / etc.)
- ✅ Multi-pass dep-order publish (workspaces handled)
- ✅ Skip-already + rate-limit retry baked in
- ✅ PR-time gates: fmt + lint + test + tlisp balance + dry-run publish
- ✅ Security gates: dep vuln scan + SBOM + SPDX header sweep + (optional) cosign sign + trivy scan
- ✅ Container build + push to ghcr with multi-arch (if applicable)
- ✅ NO-SHELL enforcement on every PR (action-shell-lint)
- ✅ Adoption tracking via weekly cron survey

## Discovery

| What | Where |
|---|---|
| Catalog of all 192 typed primitives | [`patterns-full.nix`](https://github.com/pleme-io/substrate/blob/main/lib/release/patterns-full.nix) |
| Per-action README with quickstart | [`pleme-io/actions/*/README.md`](https://github.com/pleme-io/actions) |
| Root catalog index | [`actions/README.md`](https://github.com/pleme-io/actions#readme) |
| Substrate composition vision | [INTERLOCK.md](https://github.com/pleme-io/substrate/blob/main/docs/INTERLOCK.md) |
| Action-as-caixa migration roadmap | [ACTION-AS-CAIXA.md](https://github.com/pleme-io/substrate/blob/main/docs/ACTION-AS-CAIXA.md) |
| Nix-queryable | `nix eval --raw github:pleme-io/substrate#lib.aarch64-darwin.release.patterns` |
| Operator skills (Claude Code) | [pleme-io-action-vocabulary](https://github.com/pleme-io/blackmatter-pleme/blob/main/skills/pleme-io-action-vocabulary/SKILL.md), [pleme-io-pattern-core](https://github.com/pleme-io/blackmatter-pleme/blob/main/skills/pleme-io-pattern-core/SKILL.md), [pleme-io-auto-release](https://github.com/pleme-io/blackmatter-pleme/blob/main/skills/pleme-io-auto-release/SKILL.md), [pleme-io-oss-exposure](https://github.com/pleme-io/blackmatter-pleme/blob/main/skills/pleme-io-oss-exposure/SKILL.md) |

## License

Every public pleme-io repo is **MIT**. Take what you need. Extend
what serves you. Contribute back when it compounds.

## The pattern is the invitation

There is no gatekeeping. There is no operator approval queue.
There is no infrastructure to provision. There is no cost to
participate.

Author a new typed primitive following
[`pleme-io-pattern-core`](https://github.com/pleme-io/blackmatter-pleme/blob/main/skills/pleme-io-pattern-core/SKILL.md).
Open a PR. The substrate handles the rest.

**The OSS commons is the substrate's natural exhaust. Welcome.**
