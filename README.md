# T EMQX SERVICE

El repositorio es una documentación de como usar un servidor emqx con mongoDB


### mongo collections in db emqx_auth
#### mqtt_user
```
[{
  "username": "turing",
  "password_hash": "e99a18c428cb38d5f260853678922e03",
  "salt": "",
  "password": "turing",
  "is_superuser": false
}]

```

#### mqtt_authorization 
```
[
  {
    "username": "turing",
    "permission": "allow",
    "action": "publish",
    "topics": ["sensors/temperature", "sensors/humidity", "devices/+/status"]
  },
  {
    "username": "turing",
    "permission": "allow",
    "action": "subscribe",
    "topics": ["alerts/#", "notifications/general", "notifications/errors"]
  }
]
```