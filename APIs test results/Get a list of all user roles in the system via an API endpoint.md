# Get a list of all user roles in the system via an API endpoint

Notes: for the following test requests i used "Postman" app.

request:

```bash
curl -X GET \
  https://kandybarocketchat.tk/api/v1/users.list \
  -H 'cache-control: no-cache' \
  -H 'content-type: application/json' \
  -H 'postman-token: e83fa7ae-ae70-43cf-7fbc-5e4cc6c55f6e' \
  -H 'x-auth-token: U1xXYXGvHwcgI0C7gkZE4y0qXl5eLBgVWnGUljntXCF' \
  -H 'x-user-id: JssTwJoeiJoayuDPT'
```

Response:

```bash
{
    "users": [
        {
            "_id": "JssTwJoeiJoayuDPT",
            "createdAt": "2020-12-30T21:45:13.216Z",
            "emails": [
                {
                    "address": "astafit@gmail.com",
                    "verified": false
                }
            ],
            "type": "user",
            "status": "away",
            "active": true,
            "_updatedAt": "2021-01-02T16:36:39.962Z",
            "roles": [
                "admin"
            ],
            "name": "Pavlo",
            "lastLogin": "2021-01-02T16:28:39.275Z",
            "statusConnection": "away",
            "username": "Kandyba",
            "__rooms": [
                "GENERAL"
            ],
            "utcOffset": 2,
            "banners": {
                "versionUpdate-3_10_0": {
                    "id": "versionUpdate-3_10_0",
                    "priority": 10,
                    "title": "Update_your_RocketChat",
                    "text": "New_version_available_(s)",
                    "textArguments": [
                        "3.10.0"
                    ],
                    "link": "https://github.com/RocketChat/Rocket.Chat/releases/tag/3.10.0"
                },
                "alert-5fd28c37f5204d0905436930": {
                    "id": "alert-5fd28c37f5204d0905436930",
                    "priority": 10,
                    "title": "Warning",
                    "text": "Please note that push to official Rocket.Chat mobile apps is unavailable for non-registered servers. See how to register your server [here], and check our forum for more details. If don't want to receive new notifications and are running version 3.5 or higher, you can turn it off in Administration > General > Updates > Enable the Update Checker.",
                    "textArguments": [],
                    "modifiers": [],
                    "link": "https://docs.rocket.chat/guides/administrator-guides/connectivity-services#introduction"
                }
            }
        },
        {
            "_id": "9YepRcm4v2Y6ptFzJ",
            "createdAt": "2021-01-02T15:22:49.859Z",
            "username": "Testkandyba",
            "emails": [
                {
                    "address": "vsjackals@gmail.com",
                    "verified": true
                }
            ],
            "type": "user",
            "status": "online",
            "active": true,
            "_updatedAt": "2021-01-02T16:27:43.972Z",
            "__rooms": [
                "GENERAL"
            ],
            "roles": [
                "user"
            ],
            "name": "Testkandyba",
            "settings": {},
            "lastLogin": "2021-01-02T15:44:10.418Z",
            "statusText": "Online",
            "statusDefault": "online",
            "requirePasswordChange": false
        },
        {
            "_id": "rocket.cat",
            "createdAt": "2020-12-25T20:52:53.719Z",
            "avatarOrigin": "local",
            "name": "Rocket.Cat",
            "username": "rocket.cat",
            "status": "online",
            "statusDefault": "online",
            "utcOffset": 0,
            "active": true,
            "type": "bot",
            "_updatedAt": "2020-12-25T20:52:54.057Z",
            "roles": [
                "bot"
            ],
            "avatarETag": null
        },
        {
            "_id": "zZEh2ArWTxBWhsecc",
            "createdAt": "2020-12-30T23:12:20.846Z",
            "username": "sajackals",
            "emails": [
                {
                    "address": "sajackals@gmail.com",
                    "verified": true
                }
            ],
            "type": "user",
            "status": "online",
            "active": true,
            "_updatedAt": "2021-01-02T16:18:35.505Z",
            "__rooms": [
                "GENERAL"
            ],
            "roles": [
                "user"
            ],
            "name": "sajackals",
            "settings": {},
            "lastLogin": "2020-12-30T23:16:30.260Z",
            "statusText": "My status update",
            "statusDefault": "online",
            "requirePasswordChange": false
        }
    ],
    "count": 4,
    "offset": 0,
    "total": 4,
    "success": true
}
```
