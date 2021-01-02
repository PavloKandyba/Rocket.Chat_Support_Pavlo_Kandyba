## Create a new user via an API endpoint

Notes: for the following test requests i used "Postman" app.

request:

```bash
curl -X POST \
  https://kandybarocketchat.tk/api/v1/users.create \
  -H 'cache-control: no-cache' \
  -H 'content-type: application/json' \
  -H 'postman-token: dcfda1a1-e2ba-7c7a-acaf-daf022d56bca' \
  -H 'x-auth-token: oYuSqLqFof4u2iplJdJ53EbT_Jibdh5KUj2bWxkQntR' \
  -H 'x-user-id: JssTwJoeiJoayuDPT' \
  -d '{"name": "Testkandyba", "email": "vsjackals@gmail.com", "password": "W*jackals4", "username": "TestKandyba"}'
```
Response:

```bash
{
    "user": {
        "_id": "9YepRcm4v2Y6ptFzJ",
        "createdAt": "2021-01-02T15:22:49.859Z",
        "username": "Testkandyba",
        "emails": [
            {
                "address": "vsjackals@gmail.com",
                "verified": false
            }
        ],
        "type": "user",
        "status": "offline",
        "active": true,
        "_updatedAt": "2021-01-02T15:22:50.043Z",
        "__rooms": [
            "GENERAL"
        ],
        "roles": [
            "user"
        ],
        "name": "Testkandyba",
        "settings": {}
    },
    "success": true
}
```
