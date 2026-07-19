# Provider

## Overview

Media providers are the starting points for the entire Plex Media Server media library API.  It defines the paths for the groups of endpoints.  The `/media/providers` should be the only hard-coded path in clients when accessing the media library.  Non-media library endpoints are outside the scope of the media provider.  See the description in See [the section in API Info](#section/API-Info/Media-Providers) for more information on how to use media providers.
Note: Dynamic proxy paths such as `/{provider}/search`, `/{provider}/metadata`, and other provider-relative routes are resolved through the media provider API.

### Available Operations

* [AddToWatchlist](#addtowatchlist) - Add to Watchlist
* [RemoveFromWatchlist](#removefromwatchlist) - Remove from Watchlist
* [SearchDiscover](#searchdiscover) - Search Discover
* [GetWatchlist](#getwatchlist) - Get Watchlist
* [ListProviders](#listproviders) - Get the list of available media providers
* [AddProvider](#addprovider) - Add a media provider
* [RefreshProviders](#refreshproviders) - Refresh media providers
* [DeleteMediaProvider](#deletemediaprovider) - Delete a media provider

## AddToWatchlist

Add an item to the user's Plex Discover watchlist.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="addToWatchlist" method="post" path="/actions/addToWatchlist" -->
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

AddToWatchlistRequest req = new AddToWatchlistRequest() {
    Uri = "https://frightened-duster.com/",
};

var res = await sdk.Provider.AddToWatchlistAsync(req);

// handle response
```

### Parameters

| Parameter                                                               | Type                                                                    | Required                                                                | Description                                                             |
| ----------------------------------------------------------------------- | ----------------------------------------------------------------------- | ----------------------------------------------------------------------- | ----------------------------------------------------------------------- |
| `request`                                                               | [AddToWatchlistRequest](../../Models/Requests/AddToWatchlistRequest.md) | :heavy_check_mark:                                                      | The request object to use for the request.                              |
| `serverURL`                                                             | *string*                                                                | :heavy_minus_sign:                                                      | An optional server URL to use.                                          |

### Response

**[AddToWatchlistResponse](../../Models/Requests/AddToWatchlistResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## RemoveFromWatchlist

Remove an item from the user's Plex Discover watchlist.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="removeFromWatchlist" method="post" path="/actions/removeFromWatchlist" -->
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

RemoveFromWatchlistRequest req = new RemoveFromWatchlistRequest() {
    Uri = "https://miserable-scrap.net",
};

var res = await sdk.Provider.RemoveFromWatchlistAsync(req);

// handle response
```

### Parameters

| Parameter                                                                         | Type                                                                              | Required                                                                          | Description                                                                       |
| --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- |
| `request`                                                                         | [RemoveFromWatchlistRequest](../../Models/Requests/RemoveFromWatchlistRequest.md) | :heavy_check_mark:                                                                | The request object to use for the request.                                        |
| `serverURL`                                                                       | *string*                                                                          | :heavy_minus_sign:                                                                | An optional server URL to use.                                                    |

### Response

**[RemoveFromWatchlistResponse](../../Models/Requests/RemoveFromWatchlistResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## SearchDiscover

Search movies and shows in Plex Discover.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="searchDiscover" method="get" path="/library/search" -->
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

SearchDiscoverRequest req = new SearchDiscoverRequest() {
    SearchTypes = "movies,tv",
    SearchProviders = "discover,PLEXAVOD,PLEXTVOD",
};

var res = await sdk.Provider.SearchDiscoverAsync(req);

// handle response
```

### Parameters

| Parameter                                                               | Type                                                                    | Required                                                                | Description                                                             |
| ----------------------------------------------------------------------- | ----------------------------------------------------------------------- | ----------------------------------------------------------------------- | ----------------------------------------------------------------------- |
| `request`                                                               | [SearchDiscoverRequest](../../Models/Requests/SearchDiscoverRequest.md) | :heavy_check_mark:                                                      | The request object to use for the request.                              |
| `serverURL`                                                             | *string*                                                                | :heavy_minus_sign:                                                      | An optional server URL to use.                                          |

### Response

**[SearchDiscoverResponse](../../Models/Requests/SearchDiscoverResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetWatchlist

Get the user's Plex Discover watchlist.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getWatchlist" method="get" path="/library/sections/watchlist/all" -->
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

GetWatchlistRequest req = new GetWatchlistRequest() {};

var res = await sdk.Provider.GetWatchlistAsync(req);

// handle response
```

### Parameters

| Parameter                                                           | Type                                                                | Required                                                            | Description                                                         |
| ------------------------------------------------------------------- | ------------------------------------------------------------------- | ------------------------------------------------------------------- | ------------------------------------------------------------------- |
| `request`                                                           | [GetWatchlistRequest](../../Models/Requests/GetWatchlistRequest.md) | :heavy_check_mark:                                                  | The request object to use for the request.                          |
| `serverURL`                                                         | *string*                                                            | :heavy_minus_sign:                                                  | An optional server URL to use.                                      |

### Response

**[GetWatchlistResponse](../../Models/Requests/GetWatchlistResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## ListProviders

Get the list of all available media providers for this PMS.  This will generally include the library provider and possibly EPG if DVR is set up.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="listProviders" method="get" path="/media/providers" -->
```csharp
using LukeHagar.PlexAPI.SDK;
using LukeHagar.PlexAPI.SDK.Models.Components;

var sdk = new PlexAPI(token: "<YOUR_API_KEY_HERE>");

var res = await sdk.Provider.ListProvidersAsync();

// handle response
```

### Response

**[ListProvidersResponse](../../Models/Requests/ListProvidersResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## AddProvider

This endpoint registers a media provider with the server. Once registered, the media server acts as a reverse proxy to the provider, allowing both local and remote providers to work.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="addProvider" method="post" path="/media/providers" -->
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

AddProviderRequest req = new AddProviderRequest() {
    Url = "https://steep-obedience.name/",
};

var res = await sdk.Provider.AddProviderAsync(req);

// handle response
```

### Parameters

| Parameter                                                         | Type                                                              | Required                                                          | Description                                                       |
| ----------------------------------------------------------------- | ----------------------------------------------------------------- | ----------------------------------------------------------------- | ----------------------------------------------------------------- |
| `request`                                                         | [AddProviderRequest](../../Models/Requests/AddProviderRequest.md) | :heavy_check_mark:                                                | The request object to use for the request.                        |

### Response

**[AddProviderResponse](../../Models/Requests/AddProviderResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## RefreshProviders

Refresh all known media providers. This is useful in case a provider has updated features.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="refreshProviders" method="post" path="/media/providers/refresh" -->
```csharp
using LukeHagar.PlexAPI.SDK;
using LukeHagar.PlexAPI.SDK.Models.Components;

var sdk = new PlexAPI(token: "<YOUR_API_KEY_HERE>");

var res = await sdk.Provider.RefreshProvidersAsync();

// handle response
```

### Response

**[RefreshProvidersResponse](../../Models/Requests/RefreshProvidersResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## DeleteMediaProvider

Deletes a media provider with the given id

### Example Usage

<!-- UsageSnippet language="csharp" operationID="deleteMediaProvider" method="delete" path="/media/providers/{provider}" -->
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

DeleteMediaProviderRequest req = new DeleteMediaProviderRequest() {
    Provider = "<value>",
};

var res = await sdk.Provider.DeleteMediaProviderAsync(req);

// handle response
```

### Parameters

| Parameter                                                                         | Type                                                                              | Required                                                                          | Description                                                                       |
| --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- |
| `request`                                                                         | [DeleteMediaProviderRequest](../../Models/Requests/DeleteMediaProviderRequest.md) | :heavy_check_mark:                                                                | The request object to use for the request.                                        |

### Response

**[DeleteMediaProviderResponse](../../Models/Requests/DeleteMediaProviderResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |