# LiveTV

## Overview

LiveTV contains the playback sessions of a channel from a DVR device

### Available Operations

* [GetDVRRecordings](#getdvrrecordings) - Get DVR Recordings
* [GetSessions](#getsessions) - Get all sessions
* [GetDVRRecordingsByDVR](#getdvrrecordingsbydvr) - Get DVR Recordings by DVR
* [DeleteLiveTVSession](#deletelivetvsession) - Delete Live TV Session
* [GetLiveTVSession](#getlivetvsession) - Get a single session
* [GetSessionPlaylistIndex](#getsessionplaylistindex) - Get a session playlist index
* [GetSessionSegment](#getsessionsegment) - Get a single session segment

## GetDVRRecordings

List completed DVR recordings.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getDVRRecordings" method="get" path="/livetv/recordings" -->
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

GetDVRRecordingsRequest req = new GetDVRRecordingsRequest() {};

var res = await sdk.LiveTV.GetDVRRecordingsAsync(req);

// handle response
```

### Parameters

| Parameter                                                                   | Type                                                                        | Required                                                                    | Description                                                                 |
| --------------------------------------------------------------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------------------------- |
| `request`                                                                   | [GetDVRRecordingsRequest](../../Models/Requests/GetDVRRecordingsRequest.md) | :heavy_check_mark:                                                          | The request object to use for the request.                                  |

### Response

**[GetDVRRecordingsResponse](../../Models/Requests/GetDVRRecordingsResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetSessions

Get all livetv sessions and metadata

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getSessions" method="get" path="/livetv/sessions" -->
```csharp
using LukeHagar.PlexAPI.SDK;
using LukeHagar.PlexAPI.SDK.Models.Components;

var sdk = new PlexAPI(token: "<YOUR_API_KEY_HERE>");

var res = await sdk.LiveTV.GetSessionsAsync();

// handle response
```

### Parameters

| Parameter             | Type                  | Required              | Description           |
| --------------------- | --------------------- | --------------------- | --------------------- |
| `DvrId`               | *long*                | :heavy_minus_sign:    | Filter by DVR ID.     |
| `Channel`             | *long*                | :heavy_minus_sign:    | Filter by channel ID. |

### Response

**[GetSessionsResponse](../../Models/Requests/GetSessionsResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetDVRRecordingsByDVR

List completed DVR recordings for a specific DVR.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getDVRRecordingsByDVR" method="get" path="/livetv/dvrs/{dvrId}/recordings" -->
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

GetDVRRecordingsByDVRRequest req = new GetDVRRecordingsByDVRRequest() {
    DvrId = 83756,
};

var res = await sdk.LiveTV.GetDVRRecordingsByDVRAsync(req);

// handle response
```

### Parameters

| Parameter                                                                             | Type                                                                                  | Required                                                                              | Description                                                                           |
| ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- |
| `request`                                                                             | [GetDVRRecordingsByDVRRequest](../../Models/Requests/GetDVRRecordingsByDVRRequest.md) | :heavy_check_mark:                                                                    | The request object to use for the request.                                            |

### Response

**[GetDVRRecordingsByDVRResponse](../../Models/Requests/GetDVRRecordingsByDVRResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## DeleteLiveTVSession

Terminate a Live TV session.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="deleteLiveTVSession" method="delete" path="/livetv/sessions/{sessionId}" -->
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

DeleteLiveTVSessionRequest req = new DeleteLiveTVSessionRequest() {
    SessionId = "<id>",
};

var res = await sdk.LiveTV.DeleteLiveTVSessionAsync(req);

// handle response
```

### Parameters

| Parameter                                                                         | Type                                                                              | Required                                                                          | Description                                                                       |
| --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- |
| `request`                                                                         | [DeleteLiveTVSessionRequest](../../Models/Requests/DeleteLiveTVSessionRequest.md) | :heavy_check_mark:                                                                | The request object to use for the request.                                        |

### Response

**[DeleteLiveTVSessionResponse](../../Models/Requests/DeleteLiveTVSessionResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetLiveTVSession

Get a single livetv session and metadata

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getLiveTVSession" method="get" path="/livetv/sessions/{sessionId}" -->
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

GetLiveTVSessionRequest req = new GetLiveTVSessionRequest() {
    SessionId = "<id>",
};

var res = await sdk.LiveTV.GetLiveTVSessionAsync(req);

// handle response
```

### Parameters

| Parameter                                                                   | Type                                                                        | Required                                                                    | Description                                                                 |
| --------------------------------------------------------------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------------------------- |
| `request`                                                                   | [GetLiveTVSessionRequest](../../Models/Requests/GetLiveTVSessionRequest.md) | :heavy_check_mark:                                                          | The request object to use for the request.                                  |

### Response

**[GetLiveTVSessionResponse](../../Models/Requests/GetLiveTVSessionResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetSessionPlaylistIndex

Get a playlist index for playing this session

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getSessionPlaylistIndex" method="get" path="/livetv/sessions/{sessionId}/{consumerId}/index.m3u8" -->
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

GetSessionPlaylistIndexRequest req = new GetSessionPlaylistIndexRequest() {
    SessionId = "<id>",
    ConsumerId = "<id>",
};

var res = await sdk.LiveTV.GetSessionPlaylistIndexAsync(req);

// handle response
```

### Parameters

| Parameter                                                                                 | Type                                                                                      | Required                                                                                  | Description                                                                               |
| ----------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------- |
| `request`                                                                                 | [GetSessionPlaylistIndexRequest](../../Models/Requests/GetSessionPlaylistIndexRequest.md) | :heavy_check_mark:                                                                        | The request object to use for the request.                                                |

### Response

**[GetSessionPlaylistIndexResponse](../../Models/Requests/GetSessionPlaylistIndexResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetSessionSegment

Get a single LiveTV session segment

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getSessionSegment" method="get" path="/livetv/sessions/{sessionId}/{consumerId}/{segmentId}" -->
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

GetSessionSegmentRequest req = new GetSessionSegmentRequest() {
    SessionId = "<id>",
    ConsumerId = "<id>",
    SegmentId = "<id>",
};

var res = await sdk.LiveTV.GetSessionSegmentAsync(req);

// handle response
```

### Parameters

| Parameter                                                                     | Type                                                                          | Required                                                                      | Description                                                                   |
| ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- |
| `request`                                                                     | [GetSessionSegmentRequest](../../Models/Requests/GetSessionSegmentRequest.md) | :heavy_check_mark:                                                            | The request object to use for the request.                                    |

### Response

**[GetSessionSegmentResponse](../../Models/Requests/GetSessionSegmentResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |