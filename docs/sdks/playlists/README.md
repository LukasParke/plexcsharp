# Playlists

## Overview

Plex Playlists operations

### Available Operations

* [DeletePlaylistByRatingKey](#deleteplaylistbyratingkey) - Delete Playlist

## DeletePlaylistByRatingKey

Delete a playlist.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="deletePlaylistByRatingKey" method="delete" path="/playlists" -->
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

DeletePlaylistByRatingKeyRequest req = new DeletePlaylistByRatingKeyRequest() {
    RatingKey = 499749,
};

var res = await sdk.Playlists.DeletePlaylistByRatingKeyAsync(req);

// handle response
```

### Parameters

| Parameter                                                                                     | Type                                                                                          | Required                                                                                      | Description                                                                                   |
| --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- |
| `request`                                                                                     | [DeletePlaylistByRatingKeyRequest](../../Models/Requests/DeletePlaylistByRatingKeyRequest.md) | :heavy_check_mark:                                                                            | The request object to use for the request.                                                    |

### Response

**[DeletePlaylistByRatingKeyResponse](../../Models/Requests/DeletePlaylistByRatingKeyResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |