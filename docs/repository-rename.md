# Repository rename: AI Engineering Guardrails

The canonical repository is now
[ravisingh11/ai-engineering-guardrails](https://github.com/ravisingh11/ai-engineering-guardrails).
It was previously **AI Software Toolkit** (`ravisingh11/ai-software-toolkit`),
and originally **Engineering Standards** (`ravisingh11/engineering-standards`).
All three names refer to the same GitHub repository, ID `1348591078`.
Existing commits, pull requests, tags and releases retain their original identities.

This is a project/repository rename. **Proof** remains the assurance component.
The earlier [Guardrails-to-Proof migration](proof/migrating-from-guardrails.md)
is a separate runtime migration; the new project name does not restore the
retired `.guardrails/` runtime layout.

## Compatibility names stay stable

Keep the `ai-toolkit` command, `ai-toolkit.pyz` archive, `AI_TOOLKIT_*` settings,
`toolkit.toml`, `toolkit.lock.json`, `.proof/`, `PROOF_*` variables, skill IDs,
and workflow check names. Existing installations keep their paths, selections
and update behavior. Core remains advisory; all checks are optional, and
lifecycle/polyglot execution stays manual. This rename activates no producers,
installs no hooks and changes no branch protection.

The optional Spec Kit preset keeps its `engineering-standards` ID, source path
and independent version. The release-artifact-verification predicate URI also
retains its original `ai-software-toolkit` namespace: it is a versioned contract
identifier, not an outdated download link.

## Clones and forks

For a direct clone, update the remote without moving the checkout:

```sh
git remote -v
git remote set-url origin https://github.com/ravisingh11/ai-engineering-guardrails.git
git fetch origin
```

For a clone of your own fork, keep `origin` pointing at that fork. Update the
actual upstream remote instead, for example:

```sh
git remote set-url upstream https://github.com/ravisingh11/ai-engineering-guardrails.git
git fetch upstream
```

Existing local directory names remain valid. New clone examples use
`ai-engineering-guardrails`; existing evidence and saved workspace paths do not
need moving. GitHub redirects ordinary Git operations and repository links
from old names. Do not create another repository at an old address, which can
remove its redirect. See [GitHub's rename guidance](https://docs.github.com/en/repositories/creating-and-managing-repositories/renaming-a-repository).

## Actions and current integrations

Use the new repository path for Actions and reusable workflows, preserving the
reviewed tag or commit pin:

```yaml
- uses: ravisingh11/ai-engineering-guardrails@<reviewed-tag-or-commit>
```

GitHub Actions does not follow repository redirects for Action/workflow
references, including commit-pinned references. Review explicit checkout
repositories, current download URLs, provider project bindings and repository
allowlists too. See [GitHub's workflow reference](https://docs.github.com/en/actions/reference/workflows-and-actions/reusing-workflow-configurations).

Current source names the composite Action **AI Engineering Guardrails Proof
Attestation**. Published tags keep the metadata they shipped; a new source
label does not republish a release or update Marketplace metadata by itself.

Copied runtime/skill files need only the active display/link refresh, not an
unrelated policy or runtime upgrade. Keep published provenance pins intact and
record any metadata-only source refresh separately. Historical verification
records, screenshots, source hashes, skill captures and run identities retain
the original repository name; a rename does not rerun their checks.

## Pages, badges and About

The current toolkit report address is
[AI Engineering Guardrails scorecard](https://ravisingh11.github.io/ai-engineering-guardrails/)
and its badge is
[proof-badge.svg](https://ravisingh11.github.io/ai-engineering-guardrails/proof-badge.svg).
Old project Pages addresses are not covered by repository redirects. GitHub
About uses the new description, topics and canonical report URL. Public source
navigation and branding use the new name after their PR is reviewed and merged.

The reference application keeps its existing repository, Worker/database
identities and [report address](https://ravisingh11.github.io/ai-software-toolkit-reference-app/).
Its description and current upstream links use AI Engineering Guardrails.
This rename performs no application deployment or live verification.

The publisher requires a fresh trustworthy run for the current repository
identity. Do not relabel an old scorecard as new evidence. The historical
teaching examples keep their original subjects and never enter current scores.
The [social-preview guide](social-preview.md) separates the reviewable image
asset from GitHub's manual image-upload setting.
