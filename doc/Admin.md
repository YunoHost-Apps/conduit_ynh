###  Coturn configuration

To be able to take advantage of audio and video call functionalities, a coturn server is often required. It is possible to [install a coturn server in YunoHost (https://github.com/YunoHost-Apps/coturn-ynh/blob/master/README-en.md).
It is then necessary to fill in the information provided by the coturn server in the file 'conduit.toml' such as:

```
turn_uris = ["turns:your.turn.url:5349?transport=udp", "turns:your.turn.url:5349?transport=tcp"]
turn_username = "<YOUR_USERNAME>"
turn_password = "<YOUR_PASSWORD>"
```
If your coturn (not Yunohost's one) don't use TLS, you might need to change a little bit like :
```
turn_uris = ["turn:your.turn.url:5349?transport=udp", "turn:your.turn.url:5349?transport=tcp"]
``