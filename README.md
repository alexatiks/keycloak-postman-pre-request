# Postman pre-request script for authentication with Keycloak

This is javascript for use with [Postman](https://www.getpostman.com/)'s pre-request script feature.
It makes POST request to [Keycloak Token Endpoint](https://www.keycloak.org/docs/latest/authorization_services/#_service_overview) to
get a valid token and automatically set the token for all requests in Postman collection.

## Usage

1. Click edit on a collection and copy the content of [keycloak-fetch-token-postman-pre-request.js](keycloak-fetch-token-postman-pre-request.js) into the "Pre-request Script" tab in Postman.

 <p align="center">
  <img src="https://github.com/alexatiks/keycloak-postman-pre-request/raw/master/screenshots/postman-edit-script.png?raw=true" alt="Edit collection"/>
</p>

2. In the Authorization tab set the Type to Bearer Token and Token to {{token}}. This is the token we created and set via the pre-request script.

 <p align="center">
  <img src="https://github.com/alexatiks/keycloak-postman-pre-request/raw/master/screenshots/postman-edit-auth.png?raw=true" alt="Edit collection"/>
</p>
 
3. For all API requests: In the Authorization tab select Type - Inherit auth from parent
4. ENJOY
