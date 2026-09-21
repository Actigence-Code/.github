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

