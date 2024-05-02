<!--
Nota bene : ce README est automatiquement généré par <https://github.com/YunoHost/apps/tree/master/tools/readme_generator>
Il NE doit PAS être modifié à la main.
-->

# Conduit pour YunoHost

[![Niveau d’intégration](https://dash.yunohost.org/integration/conduit.svg)](https://dash.yunohost.org/appci/app/conduit) ![Statut du fonctionnement](https://ci-apps.yunohost.org/ci/badges/conduit.status.svg) ![Statut de maintenance](https://ci-apps.yunohost.org/ci/badges/conduit.maintain.svg)

[![Installer Conduit avec YunoHost](https://install-app.yunohost.org/install-with-yunohost.svg)](https://install-app.yunohost.org/?app=conduit)

*[Lire le README dans d'autres langues.](./ALL_README.md)*

> *Ce package vous permet d’installer Conduit rapidement et simplement sur un serveur YunoHost.*  
> *Si vous n’avez pas YunoHost, consultez [ce guide](https://yunohost.org/install) pour savoir comment l’installer et en profiter.*

## Vue d’ensemble

Conduit est une implémentation de serveur open source légère de la spécification Matrix avec un accent sur une configuration facile et des exigences système faibles. Cela signifie que vous pouvez créer votre propre configuration Conduit en quelques minutes seulement.
Conduit garde les choses simples, c'est un binaire unique avec une base de données intégrée et peut être beaucoup plus rapide que d'autres implémentations de serveur dans certains cas.

**Version incluse :** 0.6.0~ynh6
## Avertissements / informations importantes

## Configuration

### Configuration d'un coturn
Afin de pouvoir profiter des fonctionnalités d'appels audio et video, un serveur coturn est souvent requis. Il est possible d'[installer un serveur coturn dans Yunohost](https://github.com/YunoHost-Apps/coturn_ynh/blob/master/README_fr.md).
Il est ensuite nécessaire de renseigner les informations fournies par le serveur coturn dans le fichier `conduit.toml` tel que :
```
turn_uris = ["turns:your.turn.url:5349?transport=udp", "turns:your.turn.url:5349?transport=tcp"]
turn_username = "<YOUR_USERNAME>"
turn_password = "<YOUR_PASSWORD>"
```
Si votre serveur coturn (autre que celui de Yunohost) n'utilise pas une connection TLS, vous devrez ajuster ainsi :
```
turn_uris = ["turn:your.turn.url:5349?transport=udp", "turn:your.turn.url:5349?transport=tcp"]
```


## Documentations et ressources

- Site officiel de l’app : <https://conduit.rs/>
- Documentation officielle de l’admin : <https://gitlab.com/famedly/conduit>
- Dépôt de code officiel de l’app : <https://gitlab.com/famedly/conduit>
- YunoHost Store : <https://apps.yunohost.org/app/conduit>
- Signaler un bug : <https://github.com/YunoHost-Apps/conduit_ynh/issues>

## Informations pour les développeurs

Merci de faire vos pull request sur la [branche `testing`](https://github.com/YunoHost-Apps/conduit_ynh/tree/testing).

Pour essayer la branche `testing`, procédez comme suit :

```bash
sudo yunohost app install https://github.com/YunoHost-Apps/conduit_ynh/tree/testing --debug
ou
sudo yunohost app upgrade conduit -u https://github.com/YunoHost-Apps/conduit_ynh/tree/testing --debug
```

**Plus d’infos sur le packaging d’applications :** <https://yunohost.org/packaging_apps>
