# Contributing

First off — thanks for taking the time to contribute! These guidelines apply to
all of my personal repositories unless a repository provides its own
`CONTRIBUTING.md`.

By participating, you agree to abide by the [Code of Conduct](CODE_OF_CONDUCT.md).

## Ways to contribute

- **Report bugs** and **request features** through the issue templates.
- **Improve documentation** — typo fixes and clarifications are always welcome.
- **Submit code** via pull requests (see below).
- **Answer questions** and share ideas in Discussions.

If you plan a large change, please open an issue or discussion first so we can
agree on the approach before you invest significant effort.

## Development setup

Setup varies per project — check the repository's `README.md` for specifics.
Most Python projects here use [`uv`](https://docs.astral.sh/uv/):

```bash
uv sync            # install dependencies
uv run pytest      # run the test suite
uv run ruff check  # lint
uv run ruff format # format
```

## Pull request process

1. **Fork** the repository and create a branch from `main`.
2. Make your change, **add or update tests**, and keep the diff focused.
3. Ensure lint, formatting, and the test suite pass locally.
4. Update relevant documentation.
5. Open a pull request and fill out the template.

Keep pull requests small and single-purpose — it makes review faster and
history cleaner.

## Conventions

These repositories follow a set of naming conventions:

- **Commit messages** — [Conventional Commits v1.0.0](https://www.conventionalcommits.org/en/v1.0.0/)
  (e.g. `feat: add retry option`, `fix: handle empty payload`, `docs: ...`).
- **Branch names** — [Conventional Branch](https://conventional-branch.github.io/)
  (e.g. `feature/...`, `fix/...`, `docs/...`).
- **Pull request titles** — [Conventional Pull Request action format](https://github.com/marketplace/actions/conventional-pull-request).

## Code style

- **Python**: type hints, [PEP 8](https://peps.python.org/pep-0008/),
  formatted and linted with [Ruff](https://docs.astral.sh/ruff/). Prefer the
  standard library unless a third-party dependency is clearly warranted.
- **JavaScript / TypeScript**: use [`bun`](https://bun.sh/).

## License

Unless stated otherwise, contributions are accepted under the same license as
the repository you are contributing to. Check the repository's `LICENSE` file.
