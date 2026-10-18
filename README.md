# lib-fetch-js

`fetch` over the generated WebIDL bindings — JS-host counterpart of `fetch-c`. Bindings vendored under `handl-packages/generated/`.

Part of the `handl-lang` org split (ADR-0128). History is a `git subtree
split` of the platform monorepo's `fetch-js/` (via `web`).

## Layout

```text
src/        the .hnl sources
pkg.hnl     dependencies, when any: `{ deps: { <name>: "branch:<ref>" } }`
```

## Gate

```bash
HNL=../host-cli/target/debug/hnl scripts/hnl-gate.sh
```
