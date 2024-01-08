## Usage

[Helm](https://helm.sh) must be installed to use the charts.  Please refer to
Helm's [documentation](https://helm.sh/docs) to get started.

Once Helm has been set up correctly, add the repo as follows:

  helm repo add <alias> https://sul-dlss.github.io/helm-charts

If you had already added this repo earlier, run `helm repo update` to retrieve
the latest versions of the packages.  You can then run `helm search repo
<alias>` to see the charts.

To install the <chart-name> chart:

    helm install my-<chart-name> <alias>/<chart-name>

To uninstall the chart:

    helm delete my-<chart-name>

## Charts

### Puppetboard

Originally based from https://github.com/camptocamp/charts, but moved to use
a more recent version of the puppetboard container from
https://github.com/voxpupuli/puppetboard/pkgs/container/puppetboard.  The
updated container has a new requirement for a session secret key.  The helm
chart also removes the assumption that the puppetserver this is run against is
also in kubernetes.
