# Contributing to GlioVTE

GlioVTE is organized for collaborative research development while keeping clinical data and unpublished evidence protected.

## Contributor identity

Use your own GitHub account and an email address associated with that account. Do not share one Git identity across collaborators. When a commit is jointly authored, add one trailer for every co-author:

```text
Co-authored-by: Full Name <account-linked-email@example.org>
```

This preserves authorship in the Git history and GitHub contribution graph.

## Development workflow

1. Synchronize your local `main` branch with the remote repository.
2. Create a focused branch such as `feature/cohort-contract`, `analysis/calibration`, or `docs/outcome-definition`.
3. Keep each commit limited to one coherent change.
4. Run relevant tests and inspect generated research artifacts before pushing.
5. Open a Pull Request describing the scientific or engineering purpose, evidence source, validation performed, and remaining limitations.
6. Resolve review comments before merge.

Direct commits are available to invited collaborators, but Pull Requests are recommended for changes that affect cohort construction, outcome labels, feature timing, model evaluation, tables, figures, or public conclusions.

## Commit messages

Use a short, specific subject with one of these prefixes:

- `feat:` new model or data-pipeline capability
- `fix:` correction to code, schema, or analysis
- `test:` tests or validation fixtures
- `docs:` documentation or protocol changes
- `refactor:` internal restructuring without a scientific change
- `chore:` packaging, automation, or repository maintenance

Do not create empty commits or split one logical change into artificial commits for contribution counting.

## Clinical-data boundary

Never commit:

- patient identifiers or dates that may identify an individual;
- raw or derived clinical records;
- protected imaging or report text;
- credentials, tokens, internal URLs, or access keys;
- private patient-level split manifests;
- trained weights or predictions that have not passed release review;
- institution-specific mappings that could expose restricted systems.

Only public-safe schemas, synthetic fixtures, aggregate outputs, and approved artifacts may be added to the repository.

## Scientific review

Every research Pull Request should state:

- the prediction time and outcome horizon it assumes;
- whether each feature is available at prediction time;
- the cohort and split to which the change applies;
- the source of any reported number, table, or figure;
- the tests or checks that were run;
- limitations and unresolved questions.

Changes to labels, exclusions, endpoint definitions, or evaluation sets require explicit review from the research leads before merge.

