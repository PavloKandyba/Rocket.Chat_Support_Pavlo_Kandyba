# Get the room information via an API endpoint

Notes: for the following test requests i used "Postman" app.

request:

```bash
curl -X GET \
  'https://kandybarocketchat.tk/api/v1/rooms.info?roomId=GENERAL' \
  -H 'cache-control: no-cache' \
  -H 'content-type: application/json' \
  -H 'postman-token: 1fc7847a-bd50-3558-72c8-09422d74ecf6' \
  -H 'x-auth-token: U1xXYXGvHwcgI0C7gkZE4y0qXl5eLBgVWnGUljntXCF' \
  -H 'x-user-id: JssTwJoeiJoayuDPT'
```

Response:

```bash
{
    "room": {
        "_id": "GENERAL",
        "ts": "2020-12-25T20:52:53.711Z",
        "t": "c",
        "name": "general",
        "usernames": [],
        "msgs": 6,
        "usersCount": 3,
        "default": true,
        "_updatedAt": "2021-01-02T16:28:01.401Z",
        "description": "test",
        "lastMessage": {
            "_id": "ThFm9Nn59Wue8hYtY",
            "rid": "GENERAL",
            "msg": "test",
            "ts": "2021-01-02T16:28:01.368Z",
            "u": {
                "_id": "JssTwJoeiJoayuDPT",
                "username": "Kandyba",
                "name": "Pavlo"
            },
            "_updatedAt": "2021-01-02T16:28:01.392Z",
            "mentions": [],
            "channels": []
        },
        "lm": "2021-01-02T16:28:01.368Z"
    },
    "success": true
}
```
