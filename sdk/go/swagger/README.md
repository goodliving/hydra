# Go API client for swagger

Please refer to the user guide for in-depth documentation: https://ory.gitbooks.io/hydra/content/   Hydra offers OAuth 2.0 and OpenID Connect Core 1.0 capabilities as a service. Hydra is different, because it works with any existing authentication infrastructure, not just LDAP or SAML. By implementing a consent app (works with any programming language) you build a bridge between Hydra and your authentication infrastructure. Hydra is able to securely manage JSON Web Keys, and has a sophisticated policy-based access control you can use if you want to. Hydra is suitable for green- (new) and brownfield (existing) projects. If you are not familiar with OAuth 2.0 and are working on a greenfield project, we recommend evaluating if OAuth 2.0 really serves your purpose. Knowledge of OAuth 2.0 is imperative in understanding what Hydra does and how it works.   The official repository is located at https://github.com/ory/hydra   ### ATTENTION - IMPORTANT NOTE   The swagger generator used to create this documentation does currently not support example responses. To see request and response payloads click on **\"Show JSON schema\"**: ![Enable JSON Schema on Apiary](https://storage.googleapis.com/ory.am/hydra/json-schema.png)

## Overview
This API client was generated by the [swagger-codegen](https://github.com/swagger-api/swagger-codegen) project.  By using the [swagger-spec](https://github.com/swagger-api/swagger-spec) from a remote server, you can easily generate an API client.

- API version: Latest
- Package version: 1.0.0
- Build package: io.swagger.codegen.languages.GoClientCodegen
For more information, please visit [https://www.ory.am](https://www.ory.am)

## Installation
Put the package under your project folder and add the following in import:
```
    "./swagger"
```

## Documentation for API Endpoints

All URIs are relative to *http://localhost*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*ClientsApi* | [**CreateOAuthClient**](docs/ClientsApi.md#createoauthclient) | **Post** /clients | Creates an OAuth 2.0 Client
*ClientsApi* | [**DeleteOAuthClient**](docs/ClientsApi.md#deleteoauthclient) | **Delete** /clients/{id} | Deletes an OAuth 2.0 Client
*ClientsApi* | [**GetOAuthClient**](docs/ClientsApi.md#getoauthclient) | **Get** /clients/{id} | Fetches an OAuth 2.0 Client.
*ClientsApi* | [**ListOAuthClients**](docs/ClientsApi.md#listoauthclients) | **Get** /clients | Lists OAuth 2.0 Clients
*ClientsApi* | [**UpdateOAuthClient**](docs/ClientsApi.md#updateoauthclient) | **Put** /clients/{id} | Updates an OAuth 2.0 Client
*ConsentApi* | [**AcceptConsentRequest**](docs/ConsentApi.md#acceptconsentrequest) | **Patch** /oauth2/consent/requests/{id}/accept | Accept a consent request
*ConsentApi* | [**GetConsentRequest**](docs/ConsentApi.md#getconsentrequest) | **Get** /oauth2/consent/requests/{id} | Receive consent request information
*ConsentApi* | [**RejectConsentRequest**](docs/ConsentApi.md#rejectconsentrequest) | **Patch** /oauth2/consent/requests/{id}/reject | Reject a consent request
*DefaultApi* | [**Health**](docs/DefaultApi.md#health) | **Get** /health | 
*GroupsApi* | [**AddMembersToGroup**](docs/GroupsApi.md#addmemberstogroup) | **Post** /warden/groups/{id}/members | Add members to a group
*GroupsApi* | [**CreateGroup**](docs/GroupsApi.md#creategroup) | **Post** /warden/groups | Create a group
*GroupsApi* | [**DeleteGroup**](docs/GroupsApi.md#deletegroup) | **Delete** /warden/groups/{id} | Delete a group by id
*GroupsApi* | [**FindGroupsByMember**](docs/GroupsApi.md#findgroupsbymember) | **Get** /warden/groups | Find group IDs by member
*GroupsApi* | [**GetGroup**](docs/GroupsApi.md#getgroup) | **Get** /warden/groups/{id} | Get a group by id
*GroupsApi* | [**RemoveMembersFromGroup**](docs/GroupsApi.md#removemembersfromgroup) | **Delete** /warden/groups/{id}/members | Remove members from a group
*HealthApi* | [**GetStatistics**](docs/HealthApi.md#getstatistics) | **Get** /health/stats | Show instance statistics
*JwksApi* | [**CreateJwkKey**](docs/JwksApi.md#createjwkkey) | **Post** /keys/{set} | Generate a new JSON Web Key
*JwksApi* | [**DeleteJwkKey**](docs/JwksApi.md#deletejwkkey) | **Delete** /keys/{set}/{kid} | Delete a JSON Web Key
*JwksApi* | [**DeleteJwkSet**](docs/JwksApi.md#deletejwkset) | **Delete** /keys/{set} | Delete a JSON Web Key
*JwksApi* | [**GetJwkSet**](docs/JwksApi.md#getjwkset) | **Get** /keys/{set} | Retrieves a JSON Web Key Set matching the set
*JwksApi* | [**GetJwkSetKey**](docs/JwksApi.md#getjwksetkey) | **Get** /keys/{set}/{kid} | Retrieves a JSON Web Key Set matching the set and the kid
*JwksApi* | [**UpdateJwkKey**](docs/JwksApi.md#updatejwkkey) | **Put** /keys/{set}/{kid} | Updates a JSON Web Key
*JwksApi* | [**UpdateJwkSet**](docs/JwksApi.md#updatejwkset) | **Put** /keys/{set} | Updates a JSON Web Key Set
*JwksApi* | [**WellKnown**](docs/JwksApi.md#wellknown) | **Get** /.well-known/jwks.json | Public JWKs
*Oauth2Api* | [**AcceptConsentRequest**](docs/Oauth2Api.md#acceptconsentrequest) | **Patch** /oauth2/consent/requests/{id}/accept | Accept a consent request
*Oauth2Api* | [**CreateOAuthClient**](docs/Oauth2Api.md#createoauthclient) | **Post** /clients | Creates an OAuth 2.0 Client
*Oauth2Api* | [**DeleteOAuthClient**](docs/Oauth2Api.md#deleteoauthclient) | **Delete** /clients/{id} | Deletes an OAuth 2.0 Client
*Oauth2Api* | [**GetConsentRequest**](docs/Oauth2Api.md#getconsentrequest) | **Get** /oauth2/consent/requests/{id} | Receive consent request information
*Oauth2Api* | [**GetOAuthClient**](docs/Oauth2Api.md#getoauthclient) | **Get** /clients/{id} | Fetches an OAuth 2.0 Client.
*Oauth2Api* | [**IntrospectOAuthToken**](docs/Oauth2Api.md#introspectoauthtoken) | **Post** /oauth2/introspect | Introspect an OAuth2 access token
*Oauth2Api* | [**ListOAuthClients**](docs/Oauth2Api.md#listoauthclients) | **Get** /clients | Lists OAuth 2.0 Clients
*Oauth2Api* | [**OauthAuth**](docs/Oauth2Api.md#oauthauth) | **Get** /oauth2/auth | The OAuth 2.0 Auth endpoint
*Oauth2Api* | [**OauthToken**](docs/Oauth2Api.md#oauthtoken) | **Post** /oauth2/token | The OAuth 2.0 Token endpoint
*Oauth2Api* | [**RejectConsentRequest**](docs/Oauth2Api.md#rejectconsentrequest) | **Patch** /oauth2/consent/requests/{id}/reject | Reject a consent request
*Oauth2Api* | [**RevokeOAuthToken**](docs/Oauth2Api.md#revokeoauthtoken) | **Post** /oauth2/revoke | Revoke an OAuth2 access token
*Oauth2Api* | [**UpdateOAuthClient**](docs/Oauth2Api.md#updateoauthclient) | **Put** /clients/{id} | Updates an OAuth 2.0 Client
*Oauth2Api* | [**WellKnown**](docs/Oauth2Api.md#wellknown) | **Get** /.well-known/jwks.json | Public JWKs
*Oauth2Api* | [**WellKnownHandler**](docs/Oauth2Api.md#wellknownhandler) | **Get** /.well-known/openid-configuration | Server well known configuration
*OpenidconnectApi* | [**WellKnown**](docs/OpenidconnectApi.md#wellknown) | **Get** /.well-known/jwks.json | Public JWKs
*OpenidconnectApi* | [**WellKnownHandler**](docs/OpenidconnectApi.md#wellknownhandler) | **Get** /.well-known/openid-configuration | Server well known configuration
*PoliciesApi* | [**CreatePolicy**](docs/PoliciesApi.md#createpolicy) | **Post** /policies | Create an access control policy
*PoliciesApi* | [**DeletePolicy**](docs/PoliciesApi.md#deletepolicy) | **Delete** /policies/{id} | Delete an access control policy
*PoliciesApi* | [**GetPolicy**](docs/PoliciesApi.md#getpolicy) | **Get** /policies/{id} | Get an access control policy
*PoliciesApi* | [**ListPolicies**](docs/PoliciesApi.md#listpolicies) | **Get** /policies | List access control policies
*PoliciesApi* | [**UpdatePolicy**](docs/PoliciesApi.md#updatepolicy) | **Put** /policies/{id} | Update an access control policy
*WardenApi* | [**AddMembersToGroup**](docs/WardenApi.md#addmemberstogroup) | **Post** /warden/groups/{id}/members | Add members to a group
*WardenApi* | [**CreateGroup**](docs/WardenApi.md#creategroup) | **Post** /warden/groups | Create a group
*WardenApi* | [**DeleteGroup**](docs/WardenApi.md#deletegroup) | **Delete** /warden/groups/{id} | Delete a group by id
*WardenApi* | [**FindGroupsByMember**](docs/WardenApi.md#findgroupsbymember) | **Get** /warden/groups | Find group IDs by member
*WardenApi* | [**GetGroup**](docs/WardenApi.md#getgroup) | **Get** /warden/groups/{id} | Get a group by id
*WardenApi* | [**RemoveMembersFromGroup**](docs/WardenApi.md#removemembersfromgroup) | **Delete** /warden/groups/{id}/members | Remove members from a group
*WardenApi* | [**WardenAllowed**](docs/WardenApi.md#wardenallowed) | **Post** /warden/allowed | Check if a subject is allowed to do something
*WardenApi* | [**WardenTokenAllowed**](docs/WardenApi.md#wardentokenallowed) | **Post** /warden/token/allowed | Check if the subject of a token is allowed to do something


## Documentation For Models

 - [AcceptConsentRequestPayload](docs/AcceptConsentRequestPayload.md)
 - [AllowedRequest](docs/AllowedRequest.md)
 - [Body](docs/Body.md)
 - [ConsentRequest](docs/ConsentRequest.md)
 - [ConsentRequestClient](docs/ConsentRequestClient.md)
 - [ConsentRequestManager](docs/ConsentRequestManager.md)
 - [Context](docs/Context.md)
 - [CreateRequest](docs/CreateRequest.md)
 - [Firewall](docs/Firewall.md)
 - [Group](docs/Group.md)
 - [Headers](docs/Headers.md)
 - [IdTokenClaims](docs/IdTokenClaims.md)
 - [InlineResponse200](docs/InlineResponse200.md)
 - [InlineResponse2001](docs/InlineResponse2001.md)
 - [InlineResponse2002](docs/InlineResponse2002.md)
 - [InlineResponse2003](docs/InlineResponse2003.md)
 - [InlineResponse401](docs/InlineResponse401.md)
 - [Jwk](docs/Jwk.md)
 - [JwkSet](docs/JwkSet.md)
 - [Manager](docs/Manager.md)
 - [MembersRequest](docs/MembersRequest.md)
 - [OauthClient](docs/OauthClient.md)
 - [Policy](docs/Policy.md)
 - [PolicyConditions](docs/PolicyConditions.md)
 - [RejectConsentRequestPayload](docs/RejectConsentRequestPayload.md)
 - [Session](docs/Session.md)
 - [SwaggerCreatePolicyParameters](docs/SwaggerCreatePolicyParameters.md)
 - [SwaggerGetPolicyParameters](docs/SwaggerGetPolicyParameters.md)
 - [SwaggerJwkCreateKey](docs/SwaggerJwkCreateKey.md)
 - [SwaggerJwkSetKeyQuery](docs/SwaggerJwkSetKeyQuery.md)
 - [SwaggerJwkSetQuery](docs/SwaggerJwkSetQuery.md)
 - [SwaggerJwkUpdateKey](docs/SwaggerJwkUpdateKey.md)
 - [SwaggerJwkUpdateSet](docs/SwaggerJwkUpdateSet.md)
 - [SwaggerListPolicyParameters](docs/SwaggerListPolicyParameters.md)
 - [SwaggerListPolicyResponse](docs/SwaggerListPolicyResponse.md)
 - [SwaggerUpdatePolicyParameters](docs/SwaggerUpdatePolicyParameters.md)
 - [SwaggerWardenAllowedParameters](docs/SwaggerWardenAllowedParameters.md)
 - [SwaggerWardenAllowedResponse](docs/SwaggerWardenAllowedResponse.md)
 - [SwaggerWardenAllowedResponseBody](docs/SwaggerWardenAllowedResponseBody.md)
 - [SwaggerWardenTokenAllowedParameters](docs/SwaggerWardenTokenAllowedParameters.md)
 - [SwaggerWardenTokenAllowedResponse](docs/SwaggerWardenTokenAllowedResponse.md)
 - [SwaggerWardenTokenAllowedResponseBody](docs/SwaggerWardenTokenAllowedResponseBody.md)
 - [TokenAllowedRequest](docs/TokenAllowedRequest.md)
 - [WardenTokenAllowedBody](docs/WardenTokenAllowedBody.md)
 - [WellKnown](docs/WellKnown.md)


## Documentation For Authorization


## basic

- **Type**: HTTP basic authentication

## oauth2

- **Type**: OAuth
- **Flow**: accessCode
- **Authorization URL**: https://your-hydra-instance.com/oauth2/auth
- **Scopes**: 
 - **hydra.clients**: A scope required to manage OAuth 2.0 Clients
 - **hydra.consent**: A scope required to fetch and modify consent requests
 - **hydra.groups**: A scope required to manage warden groups
 - **hydra.health**: A scope required to get health information
 - **hydra.keys.create**: A scope required to create JSON Web Keys
 - **hydra.keys.delete**: A scope required to delete JSON Web Keys
 - **hydra.keys.get**: A scope required to fetch JSON Web Keys
 - **hydra.keys.update**: A scope required to get JSON Web Keys
 - **hydra.policies**: A scope required to manage access control policies
 - **hydra.warden**: A scope required to make access control inquiries
 - **offline**: A scope required when requesting refresh tokens
 - **openid**: Request an OpenID Connect ID Token


## Author

hi@ory.am
