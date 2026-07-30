# Deprecated: Airbyte Helm chart V1

This repository hosts **chart V1**, which is deprecated and no longer receives
releases or fixes. The last version published here is `airbyte 1.9.2`.

Airbyte's Helm charts are now published from
[airbytehq/charts](https://github.com/airbytehq/charts).

## Migrate to chart V2

Follow
[Upgrade to Helm chart V2](https://docs.airbyte.com/platform/deploying-airbyte/chart-v2-community),
which covers the `values.yaml` changes V2 requires and the steps to move an
existing release. In short:

```sh
helm repo add airbyte-v2 https://airbytehq.github.io/charts
helm repo update
```

Chart V2 is also on Artifact Hub as
[airbyte-v2/airbyte](https://artifacthub.io/packages/helm/airbyte-v2/airbyte).

This repository's chart index stays published, so existing installations that
point at `https://airbytehq.github.io/helm-charts` keep resolving while you
migrate.

## Issues

Please open Helm issues on the [main Airbyte repo](https://github.com/airbytehq/airbyte).
