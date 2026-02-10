This Repository provides Helm charts for cloudflare tunnels.
This is based on https://github.com/cloudflare/argo-tunnel-examples but updated with sligtly updated and improved
support for cloudflare tunnels generated via:
* web ui - with auth via TUNEL_TOKEN env variable
* cloudflare tunnel create - with auth via mounts credentials.json file

## OCI Chart (GHCR)

This chart is also published as an OCI Helm chart in GitHub Container Registry (GHCR),
alongside the existing chart-releaser/GitHub Pages publication.

Example commands:

```sh
# pull a specific chart version from GHCR
helm pull oci://ghcr.io/kit-ar/helm--cloudflare-tunnel-v3/cf-tunnel-v3 --version <chart-version>

# install directly from GHCR
helm install cf-tunnel-v3 oci://ghcr.io/kit-ar/helm--cloudflare-tunnel-v3/cf-tunnel-v3 --version <chart-version>
```
