# Users

## Overview

Plex Users operations

### Available Operations

* [GetLegacyResources](#getlegacyresources) - Get Legacy Resources
* [GetLegacyUsers](#getlegacyusers) - Get Legacy Users
* [GetFriends](#getfriends) - Get Friends
* [GetHome](#gethome) - Get home hubs
* [GetHomeUsers](#gethomeusers) - Get home hubs Users
* [CreateHomeUser](#createhomeuser) - Create Home User
* [GetMyPlexAccount](#getmyplexaccount) - Get MyPlex Account
* [GetUserServer](#getuserserver) - Get User Server Association
* [GetServerUserFeatures](#getserveruserfeatures) - Get Server User Features
* [ShareServer](#shareserver) - Share Server
* [UpdateViewStateSync](#updateviewstatesync) - Update View State Sync
* [GetUsers](#getusers) - Get list of all connected users
* [GetAccountXML](#getaccountxml) - Get Account (XML)
* [GetAccountJSON](#getaccountjson) - Get Account (JSON)
* [DeleteHomeUser](#deletehomeuser) - Delete Home User
* [UpdateHomeUser](#updatehomeuser) - Update Home User
* [UpdateRestrictedUser](#updaterestricteduser) - Update Restricted User
* [GetServerDetails](#getserverdetails) - Get Server Details
* [ShareServerLegacy](#shareserverlegacy) - Share Server (Legacy v1)
* [RemoveShare](#removeshare) - Remove Share
* [UpdateShare](#updateshare) - Update Share
* [GetUserOptOuts](#getuseroptouts) - Get User Opt-Outs

## GetLegacyResources

Get legacy published server connections (XML).

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getLegacyResources" method="get" path="/api/resources" -->
```csharp
using LukeHagar.PlexAPI.SDK;
using LukeHagar.PlexAPI.SDK.Models.Components;

var sdk = new PlexAPI(token: "<YOUR_API_KEY_HERE>");

var res = await sdk.Users.GetLegacyResourcesAsync();

// handle response
```

### Parameters

| Parameter                      | Type                           | Required                       | Description                    |
| ------------------------------ | ------------------------------ | ------------------------------ | ------------------------------ |
| `serverURL`                    | *string*                       | :heavy_minus_sign:             | An optional server URL to use. |

### Response

**[GetLegacyResourcesResponse](../../Models/Requests/GetLegacyResourcesResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetLegacyUsers

Get legacy friends list (XML).

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getLegacyUsers" method="get" path="/api/users/" -->
```csharp
using LukeHagar.PlexAPI.SDK;
using LukeHagar.PlexAPI.SDK.Models.Components;

var sdk = new PlexAPI(token: "<YOUR_API_KEY_HERE>");

var res = await sdk.Users.GetLegacyUsersAsync();

// handle response
```

### Parameters

| Parameter                      | Type                           | Required                       | Description                    |
| ------------------------------ | ------------------------------ | ------------------------------ | ------------------------------ |
| `serverURL`                    | *string*                       | :heavy_minus_sign:             | An optional server URL to use. |

### Response

**[GetLegacyUsersResponse](../../Models/Requests/GetLegacyUsersResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetFriends

Get the list of friends and shared users.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getFriends" method="get" path="/friends" -->
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

GetFriendsRequest req = new GetFriendsRequest() {};

var res = await sdk.Users.GetFriendsAsync(req);

// handle response
```

### Parameters

| Parameter                                                       | Type                                                            | Required                                                        | Description                                                     |
| --------------------------------------------------------------- | --------------------------------------------------------------- | --------------------------------------------------------------- | --------------------------------------------------------------- |
| `request`                                                       | [GetFriendsRequest](../../Models/Requests/GetFriendsRequest.md) | :heavy_check_mark:                                              | The request object to use for the request.                      |
| `serverURL`                                                     | *string*                                                        | :heavy_minus_sign:                                              | An optional server URL to use.                                  |

### Response

**[GetFriendsResponse](../../Models/Requests/GetFriendsResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetHome

Get Plex Home user list.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getHome" method="get" path="/home" -->
```csharp
using LukeHagar.PlexAPI.SDK;
using LukeHagar.PlexAPI.SDK.Models.Components;

var sdk = new PlexAPI(token: "<YOUR_API_KEY_HERE>");

var res = await sdk.Users.GetHomeAsync();

// handle response
```

### Parameters

| Parameter                      | Type                           | Required                       | Description                    |
| ------------------------------ | ------------------------------ | ------------------------------ | ------------------------------ |
| `serverURL`                    | *string*                       | :heavy_minus_sign:             | An optional server URL to use. |

### Response

**[GetHomeResponse](../../Models/Requests/GetHomeResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetHomeUsers

Get the list of Plex Home users.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getHomeUsers" method="get" path="/home/users" -->
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

GetHomeUsersRequest req = new GetHomeUsersRequest() {};

var res = await sdk.Users.GetHomeUsersAsync(req);

// handle response
```

### Parameters

| Parameter                                                           | Type                                                                | Required                                                            | Description                                                         |
| ------------------------------------------------------------------- | ------------------------------------------------------------------- | ------------------------------------------------------------------- | ------------------------------------------------------------------- |
| `request`                                                           | [GetHomeUsersRequest](../../Models/Requests/GetHomeUsersRequest.md) | :heavy_check_mark:                                                  | The request object to use for the request.                          |
| `serverURL`                                                         | *string*                                                            | :heavy_minus_sign:                                                  | An optional server URL to use.                                      |

### Response

**[GetHomeUsersResponse](../../Models/Requests/GetHomeUsersResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## CreateHomeUser

Create a new Plex Home user.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="createHomeUser" method="post" path="/home/users" -->
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

CreateHomeUserRequest req = new CreateHomeUserRequest() {};

var res = await sdk.Users.CreateHomeUserAsync(req);

// handle response
```

### Parameters

| Parameter                                                               | Type                                                                    | Required                                                                | Description                                                             |
| ----------------------------------------------------------------------- | ----------------------------------------------------------------------- | ----------------------------------------------------------------------- | ----------------------------------------------------------------------- |
| `request`                                                               | [CreateHomeUserRequest](../../Models/Requests/CreateHomeUserRequest.md) | :heavy_check_mark:                                                      | The request object to use for the request.                              |
| `serverURL`                                                             | *string*                                                                | :heavy_minus_sign:                                                      | An optional server URL to use.                                          |

### Response

**[CreateHomeUserResponse](../../Models/Requests/CreateHomeUserResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetMyPlexAccount

Get linked MyPlex account info on PMS.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getMyPlexAccount" method="get" path="/myplex/account" -->
```csharp
using LukeHagar.PlexAPI.SDK;
using LukeHagar.PlexAPI.SDK.Models.Components;

var sdk = new PlexAPI(token: "<YOUR_API_KEY_HERE>");

var res = await sdk.Users.GetMyPlexAccountAsync();

// handle response
```

### Response

**[GetMyPlexAccountResponse](../../Models/Requests/GetMyPlexAccountResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetUserServer

Get server association information for the logged-in user.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getUserServer" method="get" path="/server" -->
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

GetUserServerRequest req = new GetUserServerRequest() {};

var res = await sdk.Users.GetUserServerAsync(req);

// handle response
```

### Parameters

| Parameter                                                             | Type                                                                  | Required                                                              | Description                                                           |
| --------------------------------------------------------------------- | --------------------------------------------------------------------- | --------------------------------------------------------------------- | --------------------------------------------------------------------- |
| `request`                                                             | [GetUserServerRequest](../../Models/Requests/GetUserServerRequest.md) | :heavy_check_mark:                                                    | The request object to use for the request.                            |
| `serverURL`                                                           | *string*                                                              | :heavy_minus_sign:                                                    | An optional server URL to use.                                        |

### Response

**[GetUserServerResponse](../../Models/Requests/GetUserServerResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetServerUserFeatures

Get features enabled per shared user for the server.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getServerUserFeatures" method="get" path="/server/users/features" -->
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

GetServerUserFeaturesRequest req = new GetServerUserFeaturesRequest() {};

var res = await sdk.Users.GetServerUserFeaturesAsync(req);

// handle response
```

### Parameters

| Parameter                                                                             | Type                                                                                  | Required                                                                              | Description                                                                           |
| ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- |
| `request`                                                                             | [GetServerUserFeaturesRequest](../../Models/Requests/GetServerUserFeaturesRequest.md) | :heavy_check_mark:                                                                    | The request object to use for the request.                                            |
| `serverURL`                                                                           | *string*                                                                              | :heavy_minus_sign:                                                                    | An optional server URL to use.                                                        |

### Response

**[GetServerUserFeaturesResponse](../../Models/Requests/GetServerUserFeaturesResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## ShareServer

Share a server with a friend or managed user.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="shareServer" method="post" path="/shared_servers" -->
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

ShareServerRequest req = new ShareServerRequest() {};

var res = await sdk.Users.ShareServerAsync(req);

// handle response
```

### Parameters

| Parameter                                                         | Type                                                              | Required                                                          | Description                                                       |
| ----------------------------------------------------------------- | ----------------------------------------------------------------- | ----------------------------------------------------------------- | ----------------------------------------------------------------- |
| `request`                                                         | [ShareServerRequest](../../Models/Requests/ShareServerRequest.md) | :heavy_check_mark:                                                | The request object to use for the request.                        |
| `serverURL`                                                       | *string*                                                          | :heavy_minus_sign:                                                | An optional server URL to use.                                    |

### Response

**[ShareServerResponse](../../Models/Requests/ShareServerResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## UpdateViewStateSync

Enable or disable watch-state sync consent for the logged-in user.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="updateViewStateSync" method="put" path="/user/view_state_sync" -->
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

UpdateViewStateSyncRequest req = new UpdateViewStateSyncRequest() {};

var res = await sdk.Users.UpdateViewStateSyncAsync(req);

// handle response
```

### Parameters

| Parameter                                                                         | Type                                                                              | Required                                                                          | Description                                                                       |
| --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- |
| `request`                                                                         | [UpdateViewStateSyncRequest](../../Models/Requests/UpdateViewStateSyncRequest.md) | :heavy_check_mark:                                                                | The request object to use for the request.                                        |
| `serverURL`                                                                       | *string*                                                                          | :heavy_minus_sign:                                                                | An optional server URL to use.                                                    |

### Response

**[UpdateViewStateSyncResponse](../../Models/Requests/UpdateViewStateSyncResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetUsers

Get list of all users that are friends and have library access with the provided Plex authentication token

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getUsers" method="get" path="/users" -->
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

GetUsersRequest req = new GetUsersRequest() {};

var res = await sdk.Users.GetUsersAsync(req);

// handle response
```

### Parameters

| Parameter                                                   | Type                                                        | Required                                                    | Description                                                 |
| ----------------------------------------------------------- | ----------------------------------------------------------- | ----------------------------------------------------------- | ----------------------------------------------------------- |
| `request`                                                   | [GetUsersRequest](../../Models/Requests/GetUsersRequest.md) | :heavy_check_mark:                                          | The request object to use for the request.                  |
| `serverURL`                                                 | *string*                                                    | :heavy_minus_sign:                                          | An optional server URL to use.                              |

### Response

**[GetUsersResponse](../../Models/Requests/GetUsersResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.BadRequest   | 400                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.Unauthorized | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetAccountXML

Get the logged-in user's account details in XML format (legacy v1 endpoint).

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getAccountXML" method="get" path="/users/account" -->
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

GetAccountXMLRequest req = new GetAccountXMLRequest() {};

var res = await sdk.Users.GetAccountXMLAsync(req);

// handle response
```

### Parameters

| Parameter                                                             | Type                                                                  | Required                                                              | Description                                                           |
| --------------------------------------------------------------------- | --------------------------------------------------------------------- | --------------------------------------------------------------------- | --------------------------------------------------------------------- |
| `request`                                                             | [GetAccountXMLRequest](../../Models/Requests/GetAccountXMLRequest.md) | :heavy_check_mark:                                                    | The request object to use for the request.                            |
| `serverURL`                                                           | *string*                                                              | :heavy_minus_sign:                                                    | An optional server URL to use.                                        |

### Response

**[GetAccountXMLResponse](../../Models/Requests/GetAccountXMLResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetAccountJSON

Get the logged-in user's account details in JSON format (legacy v1 endpoint).

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getAccountJSON" method="get" path="/users/account.json" -->
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

GetAccountJSONRequest req = new GetAccountJSONRequest() {};

var res = await sdk.Users.GetAccountJSONAsync(req);

// handle response
```

### Parameters

| Parameter                                                               | Type                                                                    | Required                                                                | Description                                                             |
| ----------------------------------------------------------------------- | ----------------------------------------------------------------------- | ----------------------------------------------------------------------- | ----------------------------------------------------------------------- |
| `request`                                                               | [GetAccountJSONRequest](../../Models/Requests/GetAccountJSONRequest.md) | :heavy_check_mark:                                                      | The request object to use for the request.                              |
| `serverURL`                                                             | *string*                                                                | :heavy_minus_sign:                                                      | An optional server URL to use.                                          |

### Response

**[GetAccountJSONResponse](../../Models/Requests/GetAccountJSONResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## DeleteHomeUser

Remove a Plex Home user.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="deleteHomeUser" method="delete" path="/home/users/{userId}" -->
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

DeleteHomeUserRequest req = new DeleteHomeUserRequest() {
    UserId = 768153,
};

var res = await sdk.Users.DeleteHomeUserAsync(req);

// handle response
```

### Parameters

| Parameter                                                               | Type                                                                    | Required                                                                | Description                                                             |
| ----------------------------------------------------------------------- | ----------------------------------------------------------------------- | ----------------------------------------------------------------------- | ----------------------------------------------------------------------- |
| `request`                                                               | [DeleteHomeUserRequest](../../Models/Requests/DeleteHomeUserRequest.md) | :heavy_check_mark:                                                      | The request object to use for the request.                              |
| `serverURL`                                                             | *string*                                                                | :heavy_minus_sign:                                                      | An optional server URL to use.                                          |

### Response

**[DeleteHomeUserResponse](../../Models/Requests/DeleteHomeUserResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## UpdateHomeUser

Update a Plex Home user.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="updateHomeUser" method="put" path="/home/users/{userId}" -->
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

UpdateHomeUserRequest req = new UpdateHomeUserRequest() {
    UserId = 187897,
};

var res = await sdk.Users.UpdateHomeUserAsync(req);

// handle response
```

### Parameters

| Parameter                                                               | Type                                                                    | Required                                                                | Description                                                             |
| ----------------------------------------------------------------------- | ----------------------------------------------------------------------- | ----------------------------------------------------------------------- | ----------------------------------------------------------------------- |
| `request`                                                               | [UpdateHomeUserRequest](../../Models/Requests/UpdateHomeUserRequest.md) | :heavy_check_mark:                                                      | The request object to use for the request.                              |
| `serverURL`                                                             | *string*                                                                | :heavy_minus_sign:                                                      | An optional server URL to use.                                          |

### Response

**[UpdateHomeUserResponse](../../Models/Requests/UpdateHomeUserResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## UpdateRestrictedUser

Update restricted (managed) home user settings.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="updateRestrictedUser" method="put" path="/home/users/restricted/{userId}" -->
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

UpdateRestrictedUserRequest req = new UpdateRestrictedUserRequest() {
    UserId = 130660,
};

var res = await sdk.Users.UpdateRestrictedUserAsync(req);

// handle response
```

### Parameters

| Parameter                                                                           | Type                                                                                | Required                                                                            | Description                                                                         |
| ----------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- |
| `request`                                                                           | [UpdateRestrictedUserRequest](../../Models/Requests/UpdateRestrictedUserRequest.md) | :heavy_check_mark:                                                                  | The request object to use for the request.                                          |
| `serverURL`                                                                         | *string*                                                                            | :heavy_minus_sign:                                                                  | An optional server URL to use.                                                      |

### Response

**[UpdateRestrictedUserResponse](../../Models/Requests/UpdateRestrictedUserResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetServerDetails

Get server details for sharing.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getServerDetails" method="get" path="/servers/{machineId}" -->
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

GetServerDetailsRequest req = new GetServerDetailsRequest() {
    MachineId = "<id>",
};

var res = await sdk.Users.GetServerDetailsAsync(req);

// handle response
```

### Parameters

| Parameter                                                                   | Type                                                                        | Required                                                                    | Description                                                                 |
| --------------------------------------------------------------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------------------------- |
| `request`                                                                   | [GetServerDetailsRequest](../../Models/Requests/GetServerDetailsRequest.md) | :heavy_check_mark:                                                          | The request object to use for the request.                                  |
| `serverURL`                                                                 | *string*                                                                    | :heavy_minus_sign:                                                          | An optional server URL to use.                                              |

### Response

**[GetServerDetailsResponse](../../Models/Requests/GetServerDetailsResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## ShareServerLegacy

Share a library with a friend (legacy v1 XML endpoint).

### Example Usage

<!-- UsageSnippet language="csharp" operationID="shareServerLegacy" method="post" path="/servers/{machineId}/shared_servers" -->
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

ShareServerLegacyRequest req = new ShareServerLegacyRequest() {
    MachineId = "<id>",
};

var res = await sdk.Users.ShareServerLegacyAsync(req);

// handle response
```

### Parameters

| Parameter                                                                     | Type                                                                          | Required                                                                      | Description                                                                   |
| ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- |
| `request`                                                                     | [ShareServerLegacyRequest](../../Models/Requests/ShareServerLegacyRequest.md) | :heavy_check_mark:                                                            | The request object to use for the request.                                    |
| `serverURL`                                                                   | *string*                                                                      | :heavy_minus_sign:                                                            | An optional server URL to use.                                                |

### Response

**[ShareServerLegacyResponse](../../Models/Requests/ShareServerLegacyResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## RemoveShare

Remove a share / friend.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="removeShare" method="delete" path="/sharings/{userId}" -->
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

RemoveShareRequest req = new RemoveShareRequest() {
    UserId = 858924,
};

var res = await sdk.Users.RemoveShareAsync(req);

// handle response
```

### Parameters

| Parameter                                                         | Type                                                              | Required                                                          | Description                                                       |
| ----------------------------------------------------------------- | ----------------------------------------------------------------- | ----------------------------------------------------------------- | ----------------------------------------------------------------- |
| `request`                                                         | [RemoveShareRequest](../../Models/Requests/RemoveShareRequest.md) | :heavy_check_mark:                                                | The request object to use for the request.                        |
| `serverURL`                                                       | *string*                                                          | :heavy_minus_sign:                                                | An optional server URL to use.                                    |

### Response

**[RemoveShareResponse](../../Models/Requests/RemoveShareResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## UpdateShare

Update friend filters (allowSync, filterMovies, etc.).

### Example Usage

<!-- UsageSnippet language="csharp" operationID="updateShare" method="put" path="/sharings/{userId}" -->
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

UpdateShareRequest req = new UpdateShareRequest() {
    UserId = 139113,
};

var res = await sdk.Users.UpdateShareAsync(req);

// handle response
```

### Parameters

| Parameter                                                         | Type                                                              | Required                                                          | Description                                                       |
| ----------------------------------------------------------------- | ----------------------------------------------------------------- | ----------------------------------------------------------------- | ----------------------------------------------------------------- |
| `request`                                                         | [UpdateShareRequest](../../Models/Requests/UpdateShareRequest.md) | :heavy_check_mark:                                                | The request object to use for the request.                        |
| `serverURL`                                                       | *string*                                                          | :heavy_minus_sign:                                                | An optional server URL to use.                                    |

### Response

**[UpdateShareResponse](../../Models/Requests/UpdateShareResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetUserOptOuts

Get online media source opt-out settings for a user.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getUserOptOuts" method="get" path="/user/{uuid}/settings/opt_outs" -->
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

GetUserOptOutsRequest req = new GetUserOptOutsRequest() {
    Uuid = "17dd8bb4-eb45-4878-97c7-017f7d9a2384",
};

var res = await sdk.Users.GetUserOptOutsAsync(req);

// handle response
```

### Parameters

| Parameter                                                               | Type                                                                    | Required                                                                | Description                                                             |
| ----------------------------------------------------------------------- | ----------------------------------------------------------------------- | ----------------------------------------------------------------------- | ----------------------------------------------------------------------- |
| `request`                                                               | [GetUserOptOutsRequest](../../Models/Requests/GetUserOptOutsRequest.md) | :heavy_check_mark:                                                      | The request object to use for the request.                              |
| `serverURL`                                                             | *string*                                                                | :heavy_minus_sign:                                                      | An optional server URL to use.                                          |

### Response

**[GetUserOptOutsResponse](../../Models/Requests/GetUserOptOutsResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |