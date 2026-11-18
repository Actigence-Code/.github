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

<!-- ACTIGENCE:urs-mail-20261118:start -->
## URS Actigence Mail · obligatoire

Appliquer l’URS Actigence Mail à chaque e-mail, notamment OTP, vérification,
invitation, création ou changement de mot de passe, notifications, rapports et
envois système. La référence visuelle est le mail Actigence Forms « Code de
vérification ». Le rendu reprend son espacement et le traitement de son bouton
dans les composants publiés du modèle commun.

Utiliser le SDK canonique courant qualifié, ses ressources exactes et le relais
Actigence Mail. L’identité d’envoi reste celle du service. Écarter tout rendu
local ou repli. Qualifier le rendu réel sur le périmètre de clients prévu et
contrôler le reçu exact avant d’émettre, y compris dans les files. Un écart
suspend la famille touchée jusqu’à correction et contre-recette.

[URS Actigence Mail · révision 1.0](https://github.com/Actigence-Code/actigence-links/blob/36bd64b422a142bf47e38eb7842e58a155ccedbe/docs/URS-ACTIGENCE-MAIL.md)
<!-- ACTIGENCE:urs-mail-20261118:end -->

<!-- ACTIGENCE:no-em-dash-20261118:start -->
## Ponctuation Actigence obligatoire

Instruction de Laurent du 18 novembre 2026. Aucun tiret cadratin (Unicode
U+2014) dans les contenus produits ou affichés par Actigence, partout et
en tout temps, dans tous les projets et toutes les langues. Cela couvre
les réponses des agents, la documentation, les interfaces, les rapports,
les notifications, les e-mails et leurs objets. Reformuler avec la ponctuation
courante ou employer le tiret simple pour un séparateur. Contrôler le rendu
avant publication. Préserver l’intégrité des sources et archives immuables.

[Politique de ponctuation Actigence](https://github.com/Actigence-Code/.github/blob/8a24081218f5adab971f735e156985c72855e918/docs/STYLE-POLICY.md)
<!-- ACTIGENCE:no-em-dash-20261118:end -->
