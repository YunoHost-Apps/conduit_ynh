<!--
N.B.: This README was automatically generated by <https://github.com/YunoHost/apps/tree/master/tools/readme_generator>
It shall NOT be edited by hand.
-->

# Conduit for YunoHost

[![Integration level](https://dash.yunohost.org/integration/conduit.svg)](https://dash.yunohost.org/appci/app/conduit) ![Working status](https://ci-apps.yunohost.org/ci/badges/conduit.status.svg) ![Maintenance status](https://ci-apps.yunohost.org/ci/badges/conduit.maintain.svg)

[![Install Conduit with YunoHost](https://install-app.yunohost.org/install-with-yunohost.svg)](https://install-app.yunohost.org/?app=conduit)

*[Read this README in other languages.](./ALL_README.md)*

> *This package allows you to install Conduit quickly and simply on a YunoHost server.*  
> *If you don't have YunoHost, please consult [the guide](https://yunohost.org/install) to learn how to install it.*

## Overview

Conduit is a lightweight open-source server implementation of the Matrix Specification with a focus on easy setup and low system requirements. That means you can make your own Conduit setup in just a few minutes.
Conduit keeps things simple, it's a single binary with an embedded database and can be much faster than other server implementations in some cases.

**Shipped version:** 0.7.0~ynh3
## Documentation and resources

- Official app website: <https://conduit.rs/>
- Official admin documentation: <https://gitlab.com/famedly/conduit>
- Upstream app code repository: <https://gitlab.com/famedly/conduit>
- YunoHost Store: <https://apps.yunohost.org/app/conduit>
- Report a bug: <https://github.com/YunoHost-Apps/conduit_ynh/issues>

## Developer info

Please send your pull request to the [`testing` branch](https://github.com/YunoHost-Apps/conduit_ynh/tree/testing).

To try the `testing` branch, please proceed like that:

```bash
sudo yunohost app install https://github.com/YunoHost-Apps/conduit_ynh/tree/testing --debug
or
sudo yunohost app upgrade conduit -u https://github.com/YunoHost-Apps/conduit_ynh/tree/testing --debug
```

**More info regarding app packaging:** <https://yunohost.org/packaging_apps>
