---
title: Upgrade
---

Version Upgrade
---------------

### Guidelines to upgrade to the latest DirectPV version

DirectPV version upgrades are seameless and transparent. The resources will be upgraded automatically when you run the latest version over the existing resources. The latest version of DirectPV should be available in [krew](https://github.com/kubernetes-sigs/krew-index). For more details on the installation, Please refer the [Installation guidelines](./installation.md).

The following recording demonstrates the version upgrade path.

[![asciicast](https://asciinema.org/a/2Stv8ugsQg72rWOEWlLUVNWrV.svg)](https://asciinema.org/a/2Stv8ugsQg72rWOEWlLUVNWrV)

NOTE: For the users who don't prefer krew, Please find the latest images in [releases](https://github.com/minio/directpv/releases).

#### Upgrade from v1.4.3 to latest

If the existing version is v1.4.3, please upgrade to v1.4.6 and then to the latest.

#### Upgrade to v3.0.0

in v3.0.0, the csi sidecar images have been updated. If private registry is used for images, please make sure the following images are available in your registry before upgrade.

```
quay.io/minio/csi-provisioner:v2.2.0-go1.18
quay.io/minio/csi-node-driver-registrar:v2.2.0-go1.18
quay.io/minio/livenessprobe:v2.2.0-go1.18
```
