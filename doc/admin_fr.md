### Configuration d'un coturn

Afin de pouvoir profiter des fonctionnalités d'appels audio et video, un serveur coturn est souvent requis. Il est possible d'[installer un serveur coturn dans YunoHost](https://github.com/YunoHost-Apps/coturn_ynh/blob/master/README_fr.md).
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