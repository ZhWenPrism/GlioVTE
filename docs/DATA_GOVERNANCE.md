# Data Governance

The public GlioVTE repository contains no patient data.

## Public-safe materials

- data dictionaries without patient values;
- schemas and validation rules;
- synthetic examples with explicit provenance;
- aggregate tables and figures approved for release;
- code, tests, configurations, and documentation cleared for publication.

## Restricted materials

- identifiers and potentially identifying dates;
- clinical notes, images, reports, and patient-level records;
- private cohort and split manifests;
- institution-specific mappings and internal system details;
- unreviewed predictions, checkpoints, logs, or derived artifacts.

## Release requirements

Every public artifact should record its source, version, creation method, governing approval, and relationship to the code revision that produced it. De-identification and public release require institutional review; removing obvious names is not sufficient.

