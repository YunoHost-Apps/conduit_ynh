<!--
N.B.: README ini dibuat secara otomatis oleh <https://github.com/YunoHost/apps/tree/master/tools/readme_generator>
Ini TIDAK boleh diedit dengan tangan.
-->

# Conduit untuk YunoHost

[![Tingkat integrasi](https://dash.yunohost.org/integration/conduit.svg)](https://ci-apps.yunohost.org/ci/apps/conduit/) ![Status kerja](https://ci-apps.yunohost.org/ci/badges/conduit.status.svg) ![Status pemeliharaan](https://ci-apps.yunohost.org/ci/badges/conduit.maintain.svg)

[![Pasang Conduit dengan YunoHost](https://install-app.yunohost.org/install-with-yunohost.svg)](https://install-app.yunohost.org/?app=conduit)

*[Baca README ini dengan bahasa yang lain.](./ALL_README.md)*

> *Paket ini memperbolehkan Anda untuk memasang Conduit secara cepat dan mudah pada server YunoHost.*  
> *Bila Anda tidak mempunyai YunoHost, silakan berkonsultasi dengan [panduan](https://yunohost.org/install) untuk mempelajari bagaimana untuk memasangnya.*

## Ringkasan

Conduit is a lightweight open-source server implementation of the Matrix Specification with a focus on easy setup and low system requirements. That means you can make your own Conduit setup in just a few minutes.
Conduit keeps things simple, it's a single binary with an embedded database and can be much faster than other server implementations in some cases.

**Versi terkirim:** 0.8.0~ynh4
## Dokumentasi dan sumber daya

- Website aplikasi resmi: <https://conduit.rs/>
- Dokumentasi admin resmi: <https://docs.conduit.rs/>
- Depot kode aplikasi hulu: <https://gitlab.com/famedly/conduit>
- Gudang YunoHost: <https://apps.yunohost.org/app/conduit>
- Laporkan bug: <https://github.com/YunoHost-Apps/conduit_ynh/issues>

## Info developer

Silakan kirim pull request ke [`testing` branch](https://github.com/YunoHost-Apps/conduit_ynh/tree/testing).

Untuk mencoba branch `testing`, silakan dilanjutkan seperti:

```bash
sudo yunohost app install https://github.com/YunoHost-Apps/conduit_ynh/tree/testing --debug
atau
sudo yunohost app upgrade conduit -u https://github.com/YunoHost-Apps/conduit_ynh/tree/testing --debug
```

**Info lebih lanjut mengenai pemaketan aplikasi:** <https://yunohost.org/packaging_apps>
