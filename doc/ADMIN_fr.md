### Se connecter à Conduit

[L'intégration à la base d'utilisateurs YunoHost n'est pas encore disponible.](https://github.com/YunoHost-Apps/conduit_ynh/issues/12) Il faut donc **activer les inscriptions** dans l'onglet de configuration de l'application, puis créer un compte depuis un client Matrix. Une fois le compte créé, vous pouvez désactiver les inscriptions si vous ne voulez pas que tout le monde puisse s'en créer un.

Vous pourrez ensuite vous connecter avec ce compte.

### Configurer Coturn

Pour que les appels audio et vidéo fonctionnent bien, un serveur Coturn est souvent indispensable. Vous pouvez [installer un serveur Coturn sur YunoHost](https://github.com/YunoHost-Apps/coturn-ynh/blob/master/README.md).
Reportez ensuite les informations fournies par Coturn dans le fichier `conduit.toml`, sur le modèle suivant :

```
turn_uris = ["turns:your.turn.url:5349?transport=udp", "turns:your.turn.url:5349?transport=tcp"]
turn_username = "<YOUR_USERNAME>"
turn_password = "<YOUR_PASSWORD>"
```

Si votre Coturn (et non celui de YunoHost) n'utilise pas TLS, adaptez légèrement la configuration :

```
turn_uris = ["turn:your.turn.url:5349?transport=udp", "turn:your.turn.url:5349?transport=tcp"]
```
