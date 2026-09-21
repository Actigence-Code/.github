# Contributing

Start with the [README](README.md) and [documentation index](docs/README.md). They describe the implementation, prerequisites and project-specific checks.

## Prepare a focused change

1. Work from the repository's current default branch. Keep one concern per branch and pull request.
2. Explain the user-visible problem and the intended result. Link an existing issue when relevant.
3. Keep application-specific behavior in the application. Place reusable, application-independent standards and contracts in Actigence Core.
4. Consider Actigence Logger for Python logging. Other runtimes should follow the shared logging contract through their native logging tools; do not add a Python service solely for logging.
5. Run the checks appropriate to the change and record the commands and results. Do not describe unexecuted checks as passing.

## Documentation and examples

Use clear English, descriptive headings and relative links. Show commands that match the tracked source and distinguish implemented behavior from plans. Keep the README focused on getting oriented and started; place detailed guides in `docs/`.

Treat every committed file as potentially public. Use synthetic data, `example.com`, loopback addresses and configurable paths. Never include personal details, client identities, production endpoints, internal machine paths, credentials or operational exports. Inspect logs and screenshots before attaching them.

## Review and licensing

Describe what changed, why, how it was checked and any remaining limits. Use concise commits such as `docs: clarify local setup` or `fix: preserve structured log fields`. Avoid unrelated formatting and generated-file churn.

First-party contributions are covered by the repository's [MIT license](LICENSE). Preserve third-party license notices and attribution; adding a root license does not relicense dependencies, media or imported content.

Follow the [code of conduct](CODE_OF_CONDUCT.md). Report security issues through [SECURITY.md](SECURITY.md), not through a normal issue.
