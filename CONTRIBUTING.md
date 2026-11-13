# Contributing to Scouts-Drones

Full rules: the team's Version Control Guidelines. The short version:

- Repos are **private** and live under **Scouts-Drones**. No personal forks.
- Every repo has a README with the 8 required sections (start from `repo-template`).
- **Never push to `main`.** One branch per task from latest `main`: `<type>/<short-description>`
  (`feature/`, `fix/`, `docs/`, `refactor/`, `test/`, `experiment/`, `hw/`), e.g. `fix/42-gps-timeout`.
- Commits follow Conventional Commits: `type(scope): imperative summary` (≤ 72 chars).
  Types: feat, fix, docs, refactor, test, chore, perf, hw, config.
- PRs: 1 approval, all comments resolved, **squash and merge**, delete the branch.
- Safety-critical changes (flight, failsafes, motors, power, battery) need SITL/HITL evidence in the PR.
- Never commit secrets, build outputs, logs, datasets or large binaries. Files > 10 MB: Git LFS or shared drive.
- Commit and push at least once per working day.
- Tags: `vMAJOR.MINOR.PATCH[-alpha.N|-beta.N|-rc.N]`; tag the exact commit before every field test
  (`field-test-YYYY-MM-DD`). Never move or reuse a tag.

## Before every push
- [ ] Not on `main` (`git branch --show-current`)
- [ ] `git status` shows only intended files
- [ ] No secrets / `.env` / keys
- [ ] No build outputs, logs, datasets, large binaries (unless LFS)
- [ ] Builds and tests pass
- [ ] Conventional commit messages
- [ ] README updated if setup, behaviour or results changed
