<!-- ACTIGENCE:delivery-policy:start -->
# Owner instruction: deliver every authorized change

The owner's standing instruction applies to **all Actigence-Code projects on every development server and workstation**: complete every authorized repository change with the relevant checks, a scoped commit, a push to GitHub, and a **published GitHub Release**. This authorization persists across sessions and environments; do not ask for the same commit, push, or release permission again.

1. Inspect the current work and repository conventions. Preserve unrelated changes and existing instructions; never commit secrets, credentials, private datasets, or unrelated generated files.
2. Run the existing checks appropriate to the change and record their actual results. For documentation-only changes, review the documentation and diff; do not invent application tests or claim checks that did not run.
3. Commit only the intended changes with a meaningful conventional message. Push through the repository's required branch and review process, using a pull request and required checks where applicable. Never force-push or bypass branch protections.
4. Publish a GitHub Release with a suitable new, immutable tag/version targeting the **exact verified commit SHA pushed to GitHub**. Follow the repository's versioning and release conventions, include meaningful change and validation notes, and never move an existing release tag. A documentation-only governance release may use a distinct non-application tag and must state that it changes no application code, version, or deployment; keep it separate from the latest application release.
5. Verify the remote branch, commit, tag, and published release and report the commit SHA and release URL. A local commit, an unpushed tag, a draft release, or an unmerged pull request is not completed delivery.

If a check, required review, permission, network connection, or release operation actually blocks delivery, preserve the completed work, report the precise blocker and what remains, and continue any independent authorized work. Do not silently stop at a local change or request authorization already granted. Publishing a release does not by itself authorize an application deployment.

Canonical policy: [Actigence-Code delivery policy](https://github.com/Actigence-Code/actigence-core/blob/main/docs/DELIVERY_POLICY.md).
<!-- ACTIGENCE:delivery-policy:end -->


<!-- ACTIGENCE:mandatory-core:start -->
Core is mandatory in every Actigence-Code project, clone and machine. Core contains only Theme (including UI), Assistance and i18n. Follow core-consumer.json and the mandatory workflow, pinned to immutable Core governance a5a0c1929f81d7eaae6f4f3939075f2e916e6919. All maintained UI uses exact published Theme/UI archives and the common locale controller/cookie actigence_language. Preserve real catalogues, unsupported shared choices and native permissions/data. A historical boundary is not migrated and cannot release UI changes until adapted. Backend/hosted boundaries remain explicit. Independent Theme/UI repositories are retired.
Canonical contract: https://github.com/Actigence-Code/actigence-core/blob/a5a0c1929f81d7eaae6f4f3939075f2e916e6919/docs/CORE-MANDATORY.md
<!-- ACTIGENCE:mandatory-core:end -->

<!-- ACTIGENCE:mandatory-mail:start -->
## Actigence Mail : obligation absolue du propriétaire, 2026-10-22

Aucun courriel des applications Actigence ni des serveurs ne part autrement que via Actigence Mail. Source amont unique : `/etc/actigence/mail/smtp2go.env` sur OVH, relue à chaque remise, sans copie de configuration, secret dans Git, ancien identifiant ni transport de repli. Toutes les notifications, files d'attente, tâches planifiées, scripts, alertes système et serveurs SMTP de workspace sont concernés. Les consommateurs utilisent le relais privé Actigence Mail ; seul celui-ci accède à SMTP2GO. Source absente, illisible ou invalide : refuser, jamais contourner. Préserver permissions, destinataires, anti-doublons et protections de sandbox. Appliquer `docs/MAIL-MANDATORY.md`, `mail-consumer.json` et le contrôle GitHub obligatoire. Cette instruction remplace toute ancienne recommandation de fournisseur ou SMTP privé.
<!-- ACTIGENCE:mandatory-mail:end -->
