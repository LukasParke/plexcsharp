# Authentication

## Overview

Plex Authentication operations

### Available Operations

* [RegisterDeviceJWK](#registerdevicejwk) - Register Device JWK
* [GetAuthKeys](#getauthkeys) - Get Auth Keys
* [GetAuthNonce](#getauthnonce) - Get Auth Nonce
* [ExchangeJWTToken](#exchangejwttoken) - Exchange JWT Token
* [GetClaimToken](#getclaimtoken) - Get Claim Token
* [GetFeatures](#getfeatures) - Get Features
* [Ping](#ping) - Ping the server
* [CreateOAuthPin](#createoauthpin) - Create OAuth PIN
* [CreateLegacyPin](#createlegacypin) - Create Legacy PIN
* [LinkOAuthPin](#linkoauthpin) - Link OAuth PIN
* [GetServerAccessTokens](#getserveraccesstokens) - Get Server Access Tokens
* [GetTokenDetails](#gettokendetails) - Get Token Details
* [ChangePassword](#changepassword) - Change Password
* [PostUsersSignInData](#postuserssignindata) - Get User Sign In Data
* [SignOut](#signout) - Sign Out
* [SwitchHomeUser](#switchhomeuser) - Switch Home User
* [GetOAuthPin](#getoauthpin) - Get OAuth PIN Status

## RegisterDeviceJWK

Register a device public key (JWK) for JWT-based authentication.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="registerDeviceJWK" method="post" path="/auth/jwk" -->
```csharp
using LukeHagar.PlexAPI.SDK;
using LukeHagar.PlexAPI.SDK.Models.Components;
using LukeHagar.PlexAPI.SDK.Models.Requests;

var sdk = new PlexAPI(
    accepts: LukeHagar.PlexAPI.SDK.Models.Components.Accepts.ApplicationXml,
    clientIdentifier: "abc123",
    product: "Plex for Roku",
    version: "2.4.1",
    platform: "Roku",
    platformVersion: "4.3 build 1057",
    device: "Roku 3",
    model: "4200X",
    deviceVendor: "Roku",
    deviceName: "Living Room TV",
    marketplace: "googlePlay",
    token: "<YOUR_API_KEY_HERE>"
);

RegisterDeviceJWKRequest req = new RegisterDeviceJWKRequest() {
    JWKRegistrationRequest = new JWKRegistrationRequest() {
        Jwk = new Jwk() {
            Crv = "string value",
            Kid = "string value",
            Kty = "string value",
            X = "string value",
        },
    },
};

var res = await sdk.Authentication.RegisterDeviceJWKAsync(req);

// handle response
```

### Parameters

| Parameter                                                                     | Type                                                                          | Required                                                                      | Description                                                                   |
| ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- |
| `request`                                                                     | [RegisterDeviceJWKRequest](../../Models/Requests/RegisterDeviceJWKRequest.md) | :heavy_check_mark:                                                            | The request object to use for the request.                                    |
| `serverURL`                                                                   | *string*                                                                      | :heavy_minus_sign:                                                            | An optional server URL to use.                                                |

### Response

**[RegisterDeviceJWKResponse](../../Models/Requests/RegisterDeviceJWKResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetAuthKeys

Get Plex public JWKs for signature verification.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getAuthKeys" method="get" path="/auth/keys" -->
```csharp
using LukeHagar.PlexAPI.SDK;
using LukeHagar.PlexAPI.SDK.Models.Components;
using LukeHagar.PlexAPI.SDK.Models.Requests;

var sdk = new PlexAPI(
    accepts: LukeHagar.PlexAPI.SDK.Models.Components.Accepts.ApplicationXml,
    clientIdentifier: "abc123",
    product: "Plex for Roku",
    version: "2.4.1",
    platform: "Roku",
    platformVersion: "4.3 build 1057",
    device: "Roku 3",
    model: "4200X",
    deviceVendor: "Roku",
    deviceName: "Living Room TV",
    marketplace: "googlePlay",
    token: "<YOUR_API_KEY_HERE>"
);

GetAuthKeysRequest req = new GetAuthKeysRequest() {};

var res = await sdk.Authentication.GetAuthKeysAsync(req);

// handle response
```

### Parameters

| Parameter                                                         | Type                                                              | Required                                                          | Description                                                       |
| ----------------------------------------------------------------- | ----------------------------------------------------------------- | ----------------------------------------------------------------- | ----------------------------------------------------------------- |
| `request`                                                         | [GetAuthKeysRequest](../../Models/Requests/GetAuthKeysRequest.md) | :heavy_check_mark:                                                | The request object to use for the request.                        |
| `serverURL`                                                       | *string*                                                          | :heavy_minus_sign:                                                | An optional server URL to use.                                    |

### Response

**[GetAuthKeysResponse](../../Models/Requests/GetAuthKeysResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetAuthNonce

Get a nonce to sign in client JWT authentication flow.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getAuthNonce" method="get" path="/auth/nonce" -->
```csharp
using LukeHagar.PlexAPI.SDK;
using LukeHagar.PlexAPI.SDK.Models.Components;
using LukeHagar.PlexAPI.SDK.Models.Requests;

var sdk = new PlexAPI(
    accepts: LukeHagar.PlexAPI.SDK.Models.Components.Accepts.ApplicationXml,
    clientIdentifier: "abc123",
    product: "Plex for Roku",
    version: "2.4.1",
    platform: "Roku",
    platformVersion: "4.3 build 1057",
    device: "Roku 3",
    model: "4200X",
    deviceVendor: "Roku",
    deviceName: "Living Room TV",
    marketplace: "googlePlay",
    token: "<YOUR_API_KEY_HERE>"
);

GetAuthNonceRequest req = new GetAuthNonceRequest() {};

var res = await sdk.Authentication.GetAuthNonceAsync(req);

// handle response
```

### Parameters

| Parameter                                                           | Type                                                                | Required                                                            | Description                                                         |
| ------------------------------------------------------------------- | ------------------------------------------------------------------- | ------------------------------------------------------------------- | ------------------------------------------------------------------- |
| `request`                                                           | [GetAuthNonceRequest](../../Models/Requests/GetAuthNonceRequest.md) | :heavy_check_mark:                                                  | The request object to use for the request.                          |
| `serverURL`                                                         | *string*                                                            | :heavy_minus_sign:                                                  | An optional server URL to use.                                      |

### Response

**[GetAuthNonceResponse](../../Models/Requests/GetAuthNonceResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## ExchangeJWTToken

Exchange a signed client JWT for a Plex JWT token.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="exchangeJWTToken" method="post" path="/auth/token" -->
```csharp
using LukeHagar.PlexAPI.SDK;
using LukeHagar.PlexAPI.SDK.Models.Components;
using LukeHagar.PlexAPI.SDK.Models.Requests;

var sdk = new PlexAPI(
    accepts: LukeHagar.PlexAPI.SDK.Models.Components.Accepts.ApplicationXml,
    clientIdentifier: "abc123",
    product: "Plex for Roku",
    version: "2.4.1",
    platform: "Roku",
    platformVersion: "4.3 build 1057",
    device: "Roku 3",
    model: "4200X",
    deviceVendor: "Roku",
    deviceName: "Living Room TV",
    marketplace: "googlePlay",
    token: "<YOUR_API_KEY_HERE>"
);

ExchangeJWTTokenRequest req = new ExchangeJWTTokenRequest() {
    TokenExchangeRequest = new TokenExchangeRequest() {
        ClientIdentifier = "string value",
        Jwt = "string value",
        Scope = "string value",
    },
};

var res = await sdk.Authentication.ExchangeJWTTokenAsync(req);

// handle response
```

### Parameters

| Parameter                                                                   | Type                                                                        | Required                                                                    | Description                                                                 |
| --------------------------------------------------------------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------------------------- |
| `request`                                                                   | [ExchangeJWTTokenRequest](../../Models/Requests/ExchangeJWTTokenRequest.md) | :heavy_check_mark:                                                          | The request object to use for the request.                                  |
| `serverURL`                                                                 | *string*                                                                    | :heavy_minus_sign:                                                          | An optional server URL to use.                                              |

### Response

**[ExchangeJWTTokenResponse](../../Models/Requests/ExchangeJWTTokenResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetClaimToken

Get a claim token for new server setup.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getClaimToken" method="get" path="/claim/token.json" -->
```csharp
using LukeHagar.PlexAPI.SDK;
using LukeHagar.PlexAPI.SDK.Models.Components;
using LukeHagar.PlexAPI.SDK.Models.Requests;

var sdk = new PlexAPI(
    accepts: LukeHagar.PlexAPI.SDK.Models.Components.Accepts.ApplicationXml,
    clientIdentifier: "abc123",
    product: "Plex for Roku",
    version: "2.4.1",
    platform: "Roku",
    platformVersion: "4.3 build 1057",
    device: "Roku 3",
    model: "4200X",
    deviceVendor: "Roku",
    deviceName: "Living Room TV",
    marketplace: "googlePlay",
    token: "<YOUR_API_KEY_HERE>"
);

GetClaimTokenRequest req = new GetClaimTokenRequest() {};

var res = await sdk.Authentication.GetClaimTokenAsync(req);

// handle response
```

### Parameters

| Parameter                                                             | Type                                                                  | Required                                                              | Description                                                           |
| --------------------------------------------------------------------- | --------------------------------------------------------------------- | --------------------------------------------------------------------- | --------------------------------------------------------------------- |
| `request`                                                             | [GetClaimTokenRequest](../../Models/Requests/GetClaimTokenRequest.md) | :heavy_check_mark:                                                    | The request object to use for the request.                            |
| `serverURL`                                                           | *string*                                                              | :heavy_minus_sign:                                                    | An optional server URL to use.                                        |

### Response

**[GetClaimTokenResponse](../../Models/Requests/GetClaimTokenResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetFeatures

Get Plex Pass feature flags for the logged-in user.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getFeatures" method="get" path="/features" -->
```csharp
using LukeHagar.PlexAPI.SDK;
using LukeHagar.PlexAPI.SDK.Models.Components;

var sdk = new PlexAPI(token: "<YOUR_API_KEY_HERE>");

var res = await sdk.Authentication.GetFeaturesAsync();

// handle response
```

### Parameters

| Parameter                      | Type                           | Required                       | Description                    |
| ------------------------------ | ------------------------------ | ------------------------------ | ------------------------------ |
| `serverURL`                    | *string*                       | :heavy_minus_sign:             | An optional server URL to use. |

### Response

**[GetFeaturesResponse](../../Models/Requests/GetFeaturesResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## Ping

Health / latency check. No authentication required.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="ping" method="get" path="/ping" -->
```csharp
using LukeHagar.PlexAPI.SDK;

var sdk = new PlexAPI();

var res = await sdk.Authentication.PingAsync();

// handle response
```

### Parameters

| Parameter                      | Type                           | Required                       | Description                    |
| ------------------------------ | ------------------------------ | ------------------------------ | ------------------------------ |
| `serverURL`                    | *string*                       | :heavy_minus_sign:             | An optional server URL to use. |

### Response

**[PingResponse](../../Models/Requests/PingResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## CreateOAuthPin

Create a 4-character PIN for device linking via OAuth. The user must visit https://plex.tv/link and enter the PIN to authorize the device.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="createOAuthPin" method="post" path="/pins" -->
```csharp
using LukeHagar.PlexAPI.SDK;
using LukeHagar.PlexAPI.SDK.Models.Requests;

var sdk = new PlexAPI(
    accepts: LukeHagar.PlexAPI.SDK.Models.Components.Accepts.ApplicationXml,
    clientIdentifier: "abc123",
    product: "Plex for Roku",
    version: "2.4.1",
    platform: "Roku",
    platformVersion: "4.3 build 1057",
    device: "Roku 3",
    model: "4200X",
    deviceVendor: "Roku",
    deviceName: "Living Room TV",
    marketplace: "googlePlay"
);

CreateOAuthPinRequest req = new CreateOAuthPinRequest() {};

var res = await sdk.Authentication.CreateOAuthPinAsync(
    security: new CreateOAuthPinSecurity() {
        ClientIdentifier = "<YOUR_API_KEY_HERE>",
    },
    request: req
);

// handle response
```

### Parameters

| Parameter                                                                 | Type                                                                      | Required                                                                  | Description                                                               |
| ------------------------------------------------------------------------- | ------------------------------------------------------------------------- | ------------------------------------------------------------------------- | ------------------------------------------------------------------------- |
| `request`                                                                 | [CreateOAuthPinRequest](../../Models/Requests/CreateOAuthPinRequest.md)   | :heavy_check_mark:                                                        | The request object to use for the request.                                |
| `security`                                                                | [CreateOAuthPinSecurity](../../Models/Requests/CreateOAuthPinSecurity.md) | :heavy_check_mark:                                                        | The security requirements to use for the request.                         |
| `serverURL`                                                               | *string*                                                                  | :heavy_minus_sign:                                                        | An optional server URL to use.                                            |

### Response

**[CreateOAuthPinResponse](../../Models/Requests/CreateOAuthPinResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## CreateLegacyPin

Legacy PIN creation (XML).

### Example Usage

<!-- UsageSnippet language="csharp" operationID="createLegacyPin" method="post" path="/pins.xml" -->
```csharp
using LukeHagar.PlexAPI.SDK;
using LukeHagar.PlexAPI.SDK.Models.Components;

var sdk = new PlexAPI(token: "<YOUR_API_KEY_HERE>");

var res = await sdk.Authentication.CreateLegacyPinAsync();

// handle response
```

### Parameters

| Parameter                      | Type                           | Required                       | Description                    |
| ------------------------------ | ------------------------------ | ------------------------------ | ------------------------------ |
| `serverURL`                    | *string*                       | :heavy_minus_sign:             | An optional server URL to use. |

### Response

**[CreateLegacyPinResponse](../../Models/Requests/CreateLegacyPinResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## LinkOAuthPin

Link a PIN to an account (OAuth completion).

### Example Usage

<!-- UsageSnippet language="csharp" operationID="linkOAuthPin" method="put" path="/pins/link" -->
```csharp
using LukeHagar.PlexAPI.SDK;
using LukeHagar.PlexAPI.SDK.Models.Components;
using LukeHagar.PlexAPI.SDK.Models.Requests;

var sdk = new PlexAPI(token: "<YOUR_API_KEY_HERE>");

LinkOAuthPinAuthenticationRequestBody req = new LinkOAuthPinAuthenticationRequestBody() {
    AuthToken = "example",
    Pin = "example",
};

var res = await sdk.Authentication.LinkOAuthPinAsync(req);

// handle response
```

### Parameters

| Parameter                                                                                               | Type                                                                                                    | Required                                                                                                | Description                                                                                             |
| ------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------- |
| `request`                                                                                               | [LinkOAuthPinAuthenticationRequestBody](../../Models/Requests/LinkOAuthPinAuthenticationRequestBody.md) | :heavy_check_mark:                                                                                      | The request object to use for the request.                                                              |
| `serverURL`                                                                                             | *string*                                                                                                | :heavy_minus_sign:                                                                                      | An optional server URL to use.                                                                          |

### Response

**[LinkOAuthPinResponse](../../Models/Requests/LinkOAuthPinResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetServerAccessTokens

List access tokens for the server.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getServerAccessTokens" method="get" path="/server/access_tokens" -->
```csharp
using LukeHagar.PlexAPI.SDK;
using LukeHagar.PlexAPI.SDK.Models.Components;
using LukeHagar.PlexAPI.SDK.Models.Requests;

var sdk = new PlexAPI(
    accepts: LukeHagar.PlexAPI.SDK.Models.Components.Accepts.ApplicationXml,
    clientIdentifier: "abc123",
    product: "Plex for Roku",
    version: "2.4.1",
    platform: "Roku",
    platformVersion: "4.3 build 1057",
    device: "Roku 3",
    model: "4200X",
    deviceVendor: "Roku",
    deviceName: "Living Room TV",
    marketplace: "googlePlay",
    token: "<YOUR_API_KEY_HERE>"
);

GetServerAccessTokensRequest req = new GetServerAccessTokensRequest() {};

var res = await sdk.Authentication.GetServerAccessTokensAsync(req);

// handle response
```

### Parameters

| Parameter                                                                             | Type                                                                                  | Required                                                                              | Description                                                                           |
| ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- |
| `request`                                                                             | [GetServerAccessTokensRequest](../../Models/Requests/GetServerAccessTokensRequest.md) | :heavy_check_mark:                                                                    | The request object to use for the request.                                            |
| `serverURL`                                                                           | *string*                                                                              | :heavy_minus_sign:                                                                    | An optional server URL to use.                                                        |

### Response

**[GetServerAccessTokensResponse](../../Models/Requests/GetServerAccessTokensResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetTokenDetails

Get the User data from the provided X-Plex-Token

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getTokenDetails" method="get" path="/user" -->
```csharp
using LukeHagar.PlexAPI.SDK;
using LukeHagar.PlexAPI.SDK.Models.Components;
using LukeHagar.PlexAPI.SDK.Models.Requests;

var sdk = new PlexAPI(
    accepts: LukeHagar.PlexAPI.SDK.Models.Components.Accepts.ApplicationXml,
    clientIdentifier: "abc123",
    product: "Plex for Roku",
    version: "2.4.1",
    platform: "Roku",
    platformVersion: "4.3 build 1057",
    device: "Roku 3",
    model: "4200X",
    deviceVendor: "Roku",
    deviceName: "Living Room TV",
    marketplace: "googlePlay",
    token: "<YOUR_API_KEY_HERE>"
);

GetTokenDetailsRequest req = new GetTokenDetailsRequest() {};

var res = await sdk.Authentication.GetTokenDetailsAsync(req);

// handle response
```

### Parameters

| Parameter                                                                 | Type                                                                      | Required                                                                  | Description                                                               |
| ------------------------------------------------------------------------- | ------------------------------------------------------------------------- | ------------------------------------------------------------------------- | ------------------------------------------------------------------------- |
| `request`                                                                 | [GetTokenDetailsRequest](../../Models/Requests/GetTokenDetailsRequest.md) | :heavy_check_mark:                                                        | The request object to use for the request.                                |
| `serverURL`                                                               | *string*                                                                  | :heavy_minus_sign:                                                        | An optional server URL to use.                                            |

### Response

**[GetTokenDetailsResponse](../../Models/Requests/GetTokenDetailsResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.BadRequest   | 400                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.Unauthorized | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## ChangePassword

Change or reset the logged-in user's password.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="changePassword" method="post" path="/users/password" -->
```csharp
using LukeHagar.PlexAPI.SDK;
using LukeHagar.PlexAPI.SDK.Models.Components;
using LukeHagar.PlexAPI.SDK.Models.Requests;

var sdk = new PlexAPI(
    accepts: LukeHagar.PlexAPI.SDK.Models.Components.Accepts.ApplicationXml,
    clientIdentifier: "abc123",
    product: "Plex for Roku",
    version: "2.4.1",
    platform: "Roku",
    platformVersion: "4.3 build 1057",
    device: "Roku 3",
    model: "4200X",
    deviceVendor: "Roku",
    deviceName: "Living Room TV",
    marketplace: "googlePlay",
    token: "<YOUR_API_KEY_HERE>"
);

ChangePasswordRequest req = new ChangePasswordRequest() {};

var res = await sdk.Authentication.ChangePasswordAsync(req);

// handle response
```

### Parameters

| Parameter                                                               | Type                                                                    | Required                                                                | Description                                                             |
| ----------------------------------------------------------------------- | ----------------------------------------------------------------------- | ----------------------------------------------------------------------- | ----------------------------------------------------------------------- |
| `request`                                                               | [ChangePasswordRequest](../../Models/Requests/ChangePasswordRequest.md) | :heavy_check_mark:                                                      | The request object to use for the request.                              |
| `serverURL`                                                             | *string*                                                                | :heavy_minus_sign:                                                      | An optional server URL to use.                                          |

### Response

**[ChangePasswordResponse](../../Models/Requests/ChangePasswordResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## PostUsersSignInData

Sign in user with username and password and return user data with Plex authentication token

### Example Usage

<!-- UsageSnippet language="csharp" operationID="postUsersSignInData" method="post" path="/users/signin" -->
```csharp
using LukeHagar.PlexAPI.SDK;
using LukeHagar.PlexAPI.SDK.Models.Requests;

var sdk = new PlexAPI(
    accepts: LukeHagar.PlexAPI.SDK.Models.Components.Accepts.ApplicationXml,
    clientIdentifier: "abc123",
    product: "Plex for Roku",
    version: "2.4.1",
    platform: "Roku",
    platformVersion: "4.3 build 1057",
    device: "Roku 3",
    model: "4200X",
    deviceVendor: "Roku",
    deviceName: "Living Room TV",
    marketplace: "googlePlay"
);

PostUsersSignInDataRequest req = new PostUsersSignInDataRequest() {
    RequestBody = new PostUsersSignInDataRequestBody() {
        Login = "username@email.com",
        Password = "password123",
        RememberMe = true,
        VerificationCode = "123456",
    },
};

var res = await sdk.Authentication.PostUsersSignInDataAsync(req);

// handle response
```

### Parameters

| Parameter                                                                         | Type                                                                              | Required                                                                          | Description                                                                       |
| --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- |
| `request`                                                                         | [PostUsersSignInDataRequest](../../Models/Requests/PostUsersSignInDataRequest.md) | :heavy_check_mark:                                                                | The request object to use for the request.                                        |
| `serverURL`                                                                       | *string*                                                                          | :heavy_minus_sign:                                                                | An optional server URL to use.                                                    |

### Response

**[PostUsersSignInDataResponse](../../Models/Requests/PostUsersSignInDataResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.BadRequest   | 400                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.Unauthorized | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## SignOut

Invalidate the current authentication token.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="signOut" method="delete" path="/users/signout" -->
```csharp
using LukeHagar.PlexAPI.SDK;
using LukeHagar.PlexAPI.SDK.Models.Components;
using LukeHagar.PlexAPI.SDK.Models.Requests;

var sdk = new PlexAPI(
    accepts: LukeHagar.PlexAPI.SDK.Models.Components.Accepts.ApplicationXml,
    clientIdentifier: "abc123",
    product: "Plex for Roku",
    version: "2.4.1",
    platform: "Roku",
    platformVersion: "4.3 build 1057",
    device: "Roku 3",
    model: "4200X",
    deviceVendor: "Roku",
    deviceName: "Living Room TV",
    marketplace: "googlePlay",
    token: "<YOUR_API_KEY_HERE>"
);

SignOutRequest req = new SignOutRequest() {};

var res = await sdk.Authentication.SignOutAsync(req);

// handle response
```

### Parameters

| Parameter                                                 | Type                                                      | Required                                                  | Description                                               |
| --------------------------------------------------------- | --------------------------------------------------------- | --------------------------------------------------------- | --------------------------------------------------------- |
| `request`                                                 | [SignOutRequest](../../Models/Requests/SignOutRequest.md) | :heavy_check_mark:                                        | The request object to use for the request.                |
| `serverURL`                                               | *string*                                                  | :heavy_minus_sign:                                        | An optional server URL to use.                            |

### Response

**[SignOutResponse](../../Models/Requests/SignOutResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## SwitchHomeUser

Switch to a Plex Home user and return a new auth token.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="switchHomeUser" method="post" path="/home/users/{id}/switch" -->
```csharp
using LukeHagar.PlexAPI.SDK;
using LukeHagar.PlexAPI.SDK.Models.Components;
using LukeHagar.PlexAPI.SDK.Models.Requests;

var sdk = new PlexAPI(
    accepts: LukeHagar.PlexAPI.SDK.Models.Components.Accepts.ApplicationXml,
    clientIdentifier: "abc123",
    product: "Plex for Roku",
    version: "2.4.1",
    platform: "Roku",
    platformVersion: "4.3 build 1057",
    device: "Roku 3",
    model: "4200X",
    deviceVendor: "Roku",
    deviceName: "Living Room TV",
    marketplace: "googlePlay",
    token: "<YOUR_API_KEY_HERE>"
);

SwitchHomeUserRequest req = new SwitchHomeUserRequest() {
    Id = 135337,
};

var res = await sdk.Authentication.SwitchHomeUserAsync(req);

// handle response
```

### Parameters

| Parameter                                                               | Type                                                                    | Required                                                                | Description                                                             |
| ----------------------------------------------------------------------- | ----------------------------------------------------------------------- | ----------------------------------------------------------------------- | ----------------------------------------------------------------------- |
| `request`                                                               | [SwitchHomeUserRequest](../../Models/Requests/SwitchHomeUserRequest.md) | :heavy_check_mark:                                                      | The request object to use for the request.                              |
| `serverURL`                                                             | *string*                                                                | :heavy_minus_sign:                                                      | An optional server URL to use.                                          |

### Response

**[SwitchHomeUserResponse](../../Models/Requests/SwitchHomeUserResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetOAuthPin

Poll the PIN status. Returns authToken when the user has linked the device.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getOAuthPin" method="get" path="/pins/{pinId}" -->
```csharp
using LukeHagar.PlexAPI.SDK;
using LukeHagar.PlexAPI.SDK.Models.Requests;

var sdk = new PlexAPI(
    accepts: LukeHagar.PlexAPI.SDK.Models.Components.Accepts.ApplicationXml,
    clientIdentifier: "abc123",
    product: "Plex for Roku",
    version: "2.4.1",
    platform: "Roku",
    platformVersion: "4.3 build 1057",
    device: "Roku 3",
    model: "4200X",
    deviceVendor: "Roku",
    deviceName: "Living Room TV",
    marketplace: "googlePlay"
);

GetOAuthPinRequest req = new GetOAuthPinRequest() {
    PinId = 876892,
};

var res = await sdk.Authentication.GetOAuthPinAsync(
    security: new GetOAuthPinSecurity() {
        ClientIdentifier = "<YOUR_API_KEY_HERE>",
    },
    request: req
);

// handle response
```

### Parameters

| Parameter                                                           | Type                                                                | Required                                                            | Description                                                         |
| ------------------------------------------------------------------- | ------------------------------------------------------------------- | ------------------------------------------------------------------- | ------------------------------------------------------------------- |
| `request`                                                           | [GetOAuthPinRequest](../../Models/Requests/GetOAuthPinRequest.md)   | :heavy_check_mark:                                                  | The request object to use for the request.                          |
| `security`                                                          | [GetOAuthPinSecurity](../../Models/Requests/GetOAuthPinSecurity.md) | :heavy_check_mark:                                                  | The security requirements to use for the request.                   |
| `serverURL`                                                         | *string*                                                            | :heavy_minus_sign:                                                  | An optional server URL to use.                                      |

### Response

**[GetOAuthPinResponse](../../Models/Requests/GetOAuthPinResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |