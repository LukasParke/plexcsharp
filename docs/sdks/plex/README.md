# Plex

## Overview

Plex Plex operations

### Available Operations

* [GetServerResources](#getserverresources) - Get Server Resources

## GetServerResources

Get Plex server access tokens and server connections

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getServerResources" method="get" path="/resources" -->
```csharp
using LukeHagar.PlexAPI.SDK;
using LukeHagar.PlexAPI.SDK.Models.Components;
using LukeHagar.PlexAPI.SDK.Models.Requests;

var sdk = new PlexAPI(
    accepts: LukeHagar.PlexAPI.SDK.Models.Components.Accepts.ApplicationXml,
    clientIdentifier: "abc123",
    token: "<YOUR_API_KEY_HERE>"
);

GetServerResourcesRequest req = new GetServerResourcesRequest() {
    IncludeHttps = IncludeHttps.True,
    IncludeRelay = IncludeRelay.True,
    IncludeIPv6 = IncludeIPv6.True,
};

var res = await sdk.Plex.GetServerResourcesAsync(req);

// handle response
```

### Parameters

| Parameter                                                                       | Type                                                                            | Required                                                                        | Description                                                                     |
| ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| `request`                                                                       | [GetServerResourcesRequest](../../Models/Requests/GetServerResourcesRequest.md) | :heavy_check_mark:                                                              | The request object to use for the request.                                      |
| `serverURL`                                                                     | *string*                                                                        | :heavy_minus_sign:                                                              | An optional server URL to use.                                                  |

### Response

**[GetServerResourcesResponse](../../Models/Requests/GetServerResourcesResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Unauthorized | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |