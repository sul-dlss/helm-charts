This is meant to store a helm chart for puppetboard, based on the container
packaged at https://github.com/voxpupuli/puppetboard/pkgs/container/puppetboard.
The initial setup for this came from https://github.com/camptocamp/charts and
their puppetboard chart, but that was set for 2.x versions of puppetboard and
assumed that the puppetserver was also in k8s.  This adapts that for more
general use.
