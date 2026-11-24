# AGENTS.md

Rules an AI agent (or a new contributor) follows in this repo.

[Conventional Commits 1.0.0](https://www.conventionalcommits.org/en/v1.0.0/): `type(scope)!: description` — `feat`, `fix`, `docs`, `style`, `refactor`, `perf`, `test`, `build`, `ci`, `chore`, `revert`. One commit per concern; stage files explicitly — never `git add .`.

Git-flow: work on `<kind>/<code>[-slug]` branches cut from the default branch and merged back through a pull request. Kinds: `feature bugfix hotfix release support chore docs refactor test ci perf`. This repo has no `develop` branch.

`platform.toml` registers the repo on the Stackin Action Platform, which imports its releases. `action-platform install` adds local git hooks that check branch names and commit messages; they live in `.git/hooks` of each clone and are never committed.
