# Implementation Notes – WDS Matrix Stack

- Synapse is installed from the official Matrix.org APT repository on Ubuntu.
- Apache serves Element Web from `/var/www/html` and proxies Matrix traffic.
- Federation is exposed on port `8448` with a dedicated vhost.
- Configuration and deployment are managed from a dedicated infrastructure
  repository (WDS Matrix Stack) using `ssh` + `rsync`.
