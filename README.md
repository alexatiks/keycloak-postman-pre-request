# Postman pre-request script for authentication with Keycloak

This is javascript for use with [Postman](https://www.getpostman.com/)'s pre-request script feature.
It makes POST request to [Keycloak Token Endpoint](http://www.keycloak.org/docs/3.2/securing_apps/topics/oidc/oidc-generic.html) to
get a valid token and automatically set the token for all requests in Postman collection.

## Usage

1. Click edit on a collection and copy the content of [keycloak-fetch-token-postman-pre-request.js](keycloak-fetch-token-postman-pre-request.js) into the "Pre-request Script" tab in Postman.

 ![Edit collection](/screenshots/postman-edit-script.png?raw=true)

2. In the Authorization tab set the Type to Bearer Token and Token to {{token}}. This is the token we created and set via the pre-request script.

  ![Manage Environments](/screenshots/postman-edit-auth.png?raw=true)

3. For all API requests: In the Authorization tab select Type - Inherit auth from parent