# OAuth2 Proxy Example
 
This example app shows how to use OAuth2 Proxy with Keycloak.

**Prerequisites:** 
* [Docker](https://docs.docker.com/get-docker/)
* [Docker Compose](https://docs.docker.com/compose/install/)
* [Httpie](https://httpie.io/cli) (A user friendly HTTP client)
* [Java 17](https://sdkman.io/) (optional)

> [Keycloak](https://keycloak.org/) Open Source Identity and Access Management
Add authentication to applications and secure services with minimum effort.
No need to deal with storing users or authenticating users.
Keycloak provides user federation, strong authentication, user management, fine-grained authorization, and more.

* [Getting Started](#getting-started)
* [Links](#links)
* [Help](#help)
* [License](#license)

## Getting Started

To install this example application, run the following commands:

```bash
git clone https://github.com/apiloqbc/keycloak-oauth2-proxy-example.git
cd keycloak-oauth2-proxy-example
```



### Create an Client in Keycloak

Before you begin, you’ll need create a realm in keycloak. 

### Start the Application

To start the applciatin run `docker compose up`.  This will build and run the application in containers.

## Links

This example uses the following libraries provided:

* [OAuth2 Proxy](https://oauth2-proxy.github.io/oauth2-proxy/docs/)

## Help

Please post any questions as comments on this repository.

Apache 2.0, see [LICENSE](LICENSE).
