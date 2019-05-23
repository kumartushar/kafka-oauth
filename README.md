# kafka-oauth
Java library to add OAuth support to Kafka

## Client-Broker Authentication

### Environments
For client-broker authentication, configure the below environment variables:

- OAUTH_WITH_SSL: OAuth server with SSL. Default: "true"
- OAUTH_ACCEPT_UNSECURE_SERVER: OAuth server with self-signed certificate. Default: "false"

- OAUTH_SERVER : Address of oauth server. Example: localhost:4444
- OAUTH_TOKEN_ENDPOINT : Token endpoint of OAuth server. Example: /oauth2/token
- OAUTH_INTROSPECT_ENDPOINT : Instrospect endpoint of oauth server. Example: /oauth2/introspect

- OAUTH_GRANT_TYPE : Grant Type used at OAuth server. Example: client_credentials
- OAUTH_SCOPE : User scope(in case of interbroker). Example: producer.kafka
- OAUTH_AUTHORIZATION : Refresh token of client user. Example: Basic {TOKEN}
