<!--
Ohart ongi: README hau automatikoki sortu da <https://github.com/YunoHost/apps/tree/master/tools/readme_generator>ri esker
EZ editatu eskuz.
-->

# Conduit YunoHost-erako

[![Integrazio maila](https://apps.yunohost.org/badge/integration/conduit)](https://ci-apps.yunohost.org/ci/apps/conduit/)
![Funtzionamendu egoera](https://apps.yunohost.org/badge/state/conduit)
![Mantentze egoera](https://apps.yunohost.org/badge/maintained/conduit)

[![Instalatu Conduit YunoHost-ekin](https://install-app.yunohost.org/install-with-yunohost.svg)](https://install-app.yunohost.org/?app=conduit)

*[Irakurri README hau beste hizkuntzatan.](./ALL_README.md)*

> *Pakete honek Conduit YunoHost zerbitzari batean azkar eta zailtasunik gabe instalatzea ahalbidetzen dizu.*  
> *YunoHost ez baduzu, kontsultatu [gida](https://yunohost.org/install) nola instalatu ikasteko.*

## Aurreikuspena

Conduit is a lightweight open-source server implementation of the Matrix Specification with a focus on easy setup and low system requirements. That means you can make your own Conduit setup in just a few minutes.
Conduit keeps things simple, it's a single binary with an embedded database and can be much faster than other server implementations in some cases.

**Paketatutako bertsioa:** 0.9.0~ynh1
## Dokumentazioa eta baliabideak

- Aplikazioaren webgune ofiziala: <https://conduit.rs/>
- Administratzaileen dokumentazio ofiziala: <https://docs.conduit.rs/>
- Jatorrizko aplikazioaren kode-gordailua: <https://gitlab.com/famedly/conduit>
- YunoHost Denda: <https://apps.yunohost.org/app/conduit>
- Eman errore baten berri: <https://github.com/YunoHost-Apps/conduit_ynh/issues>

## Garatzaileentzako informazioa

Bidali `pull request`a [`testing` abarrera](https://github.com/YunoHost-Apps/conduit_ynh/tree/testing).

`testing` abarra probatzeko, ondorengoa egin:

```bash
sudo yunohost app install https://github.com/YunoHost-Apps/conduit_ynh/tree/testing --debug
edo
sudo yunohost app upgrade conduit -u https://github.com/YunoHost-Apps/conduit_ynh/tree/testing --debug
```

**Informazio gehiago aplikazioaren paketatzeari buruz:** <https://yunohost.org/packaging_apps>
