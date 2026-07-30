# Deprecated: Airbyte Helm chart V1

This repository hosts **chart V1**, which is deprecated and no longer receives releases.
The last version published here is `airbyte 1.9.2`.

Airbyte's Helm charts are now published from
[airbytehq/charts](https://github.com/airbytehq/charts):

```sh
helm repo add airbyte-v2 https://airbytehq.github.io/charts
helm repo update
helm search repo airbyte-v2
```

[Upgrade to Helm chart V2](https://docs.airbyte.com/platform/deploying-airbyte/chart-v2-community)
covers both a fresh install and migrating an existing V1 release, including the
`values.yaml` changes V2 requires.

Chart V2 is available on Artifact Hub as
[airbyte-v2/airbyte](https://artifacthub.io/packages/helm/airbyte-v2/airbyte).

## Existing installations keep working

This repository's chart index stays published — no end-of-life date is set.
Existing `helm repo add` remotes, pinned `--version` installs, and Argo CD
applications that point at `https://airbytehq.github.io/helm-charts` continue to
resolve:

```sh
helm install airbyte airbyte/airbyte --version 1.9.2
```

V1 receives no fixes, including for security issues, so plan a migration to V2.

## Issues

Please open Helm issues on the [main Airbyte repo](https://github.com/airbytehq/airbyte).
