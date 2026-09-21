# Security policy

Report suspected vulnerabilities privately. Do not include exploit details in an issue or pull request, even when the repository is private: repository access can be broader than the incident response group.

## Report a vulnerability

Contact the repository maintainers through an established private channel. If the repository offers **Security → Report a vulnerability**, that channel may also be used. This feature is not assumed to be available on every repository. If you do not have a maintainer contact, use the [Actigence website](https://actigence.eu) to request a private reporting channel without sending sensitive details.

Include the affected release or commit, a description of the security boundary, reproducible steps using synthetic data, and the likely impact. Remove credentials, personal information, customer content, internal addresses and production configuration from attachments.

## Maintenance and disclosure

Report against the current default branch and identify any affected releases. Maintainers assess older versions individually; no blanket long-term support or fixed response deadline is promised. Acknowledge, investigate, agree on a remediation plan, and coordinate disclosure through the private reporting channel.

Test only systems and data you own or are explicitly authorized to test. Prefer an isolated local environment. Do not access another person's data or run disruptive tests against a shared service.

## Protect information

- Keep credentials in an appropriate secret store, outside the repository.
- Use synthetic fixtures and reserved example domains in documentation and tests.
- Do not attach raw logs, database exports, session cookies or unreviewed screenshots.
- If a credential has been exposed, revoke or rotate it; removing a line from a document does not remove Git history, clones or caches.
- Check the project documentation for additional authentication, storage and data-handling requirements.

For ordinary questions, see [Support](SUPPORT.md). For changes, see [Contributing](CONTRIBUTING.md).
