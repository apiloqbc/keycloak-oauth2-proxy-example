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
* [Security Configuration](#security-configuration)
* [Links](#links)
* [Help](#help)
* [License](#license)

## Getting Started

To install this example application, run the following commands:

```bash
git clone https://github.com/apiloqbc/keycloak-oauth2-proxy-example.git
cd keycloak-oauth2-proxy-example
```

### Security Configuration

**⚠️ IMPORTANT: Before starting the application, configure your environment variables:**

1. Copy the example environment file:
```bash
cp env.example .env
```

2. Edit `.env` and set secure values for:
   - `KEYCLOAK_ADMIN_PASSWORD`: Strong password for Keycloak admin
   - `OAUTH2_PROXY_CLIENT_SECRET`: Client secret from your Keycloak client
   - `OAUTH2_PROXY_COOKIE_SECRET`: Random 32-character string for cookie encryption

3. **Never commit the `.env` file** - it's already in `.gitignore`

4. **Keycloak Configuration**: 
   - The `imports/realm-export.json` file contains sensitive data and is excluded from version control
   - Use `imports/realm-export.example.json` as a template for your realm configuration
   - Generate your own realm export from Keycloak admin console

### Create an Client in Keycloak

Before you begin, you'll need create a realm in keycloak. 

### Start the Application

To start the application run `docker compose up`. This will build and run the application in containers.

## Links

This example uses the following libraries provided:

* [OAuth2 Proxy](https://oauth2-proxy.github.io/oauth2-proxy/docs/)

## Help

Please post any questions as comments on this repository.

Apache 2.0, see [LICENSE](LICENSE).
