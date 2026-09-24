# Xcellent Exchange fork

This is a public fork of `cursor/plugins`. The `xcellentexchange/skills` marketplace pins commits on the `xcx` branch for any skill we have changed. Skills we have not changed are pinned to `cursor/plugins` directly.

## Rules

- `main` stays identical to upstream. Sync it with GitHub's "Sync fork" button and never commit to it.
- Our changes live on `xcx`. `git diff main...xcx` shows all of them.
- Bring upstream into `xcx` with a merge, never a rebase. A rebase orphans commits the marketplace has pinned.
- This repo is public. Only edits to upstream skills belong here. Anything about our companies, systems or customers goes in a private `skills-krt-*` repo.
- Open pull requests against this repo, never against `cursor/plugins`. Run `gh repo set-default xcellentexchange/cursor-plugins` once per checkout, because `gh pr create` in a fork defaults to the parent repo.

## Changes carried on xcx

- `pstack/skills/unslop`: removed `disable-model-invocation: true` so the model can use the skill without being asked.
