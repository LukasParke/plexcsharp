# Library

## Overview

Library endpoints which are outside of the Media Provider API.  Typically this is manipulation of the library (adding/removing sections, modifying preferences, etc).

### Available Operations

* [GetRootLibrary](#getrootlibrary) - Get Root Library
* [GetLibraryItems](#getlibraryitems) - Get all items in library
* [DeleteCaches](#deletecaches) - Delete library caches
* [CleanBundles](#cleanbundles) - Clean bundles
* [IngestTransientItem](#ingesttransientitem) - Ingest a transient item
* [GetLibraryMatches](#getlibrarymatches) - Get library matches
* [OptimizeLibrary](#optimizelibrary) - Get Optimize Library
* [OptimizeLibraryPost](#optimizelibrarypost) - Optimize Library
* [OptimizeDatabase](#optimizedatabase) - Optimize the Database
* [GetRandomArtwork](#getrandomartwork) - Get random artwork
* [GetRecentlyAddedGlobal](#getrecentlyaddedglobal) - Get Global Recently Added
* [GetLibrarySectionsFallback](#getlibrarysectionsfallback) - Get Library Sections (Fallback)
* [GetSections](#getsections) - Get library sections (main Media Provider Only)
* [AddSection](#addsection) - Add a library section
* [StopAllRefreshes](#stopallrefreshes) - Stop refresh
* [GetSectionsPrefs](#getsectionsprefs) - Get section prefs
* [RefreshSectionsMetadata](#refreshsectionsmetadata) - Refresh all sections
* [GetTags](#gettags) - Get all library tags of a type
* [UploadArt](#uploadart) - Upload media art Art
* [GetMetadataChildren](#getmetadatachildren) - Get Metadata Children
* [ComputeSonicPath](#computesonicpath) - Compute Sonic Path
* [GetMetadataGrandchildren](#getmetadatagrandchildren) - Get Metadata Grandchildren
* [GetMetadataGrandparent](#getmetadatagrandparent) - Get Metadata Grandparent
* [GetNearestMetadata](#getnearestmetadata) - Get Nearest Metadata
* [GetMetadataOnDeck](#getmetadataondeck) - Get Metadata On Deck
* [GetMetadataParent](#getmetadataparent) - Get Metadata Parent
* [UploadPoster](#uploadposter) - Upload media art Poster
* [GetMetadataReviews](#getmetadatareviews) - Get Metadata Reviews
* [DeleteMetadataItem](#deletemetadataitem) - Delete a metadata item
* [EditMetadataItem](#editmetadataitem) - Edit a metadata item
* [DetectAds](#detectads) - Ad-detect an item
* [GetAllItemLeaves](#getallitemleaves) - Get the leaves of an item
* [AnalyzeMetadata](#analyzemetadata) - Analyze an item
* [GenerateThumbs](#generatethumbs) - Generate thumbs of chapters for an item
* [DetectCredits](#detectcredits) - Credit detect a metadata item
* [GetExtras](#getextras) - Get an item's extras
* [AddExtras](#addextras) - Add to an item's extras
* [GetFile](#getfile) - Get a file from a metadata or media bundle
* [StartBifGeneration](#startbifgeneration) - Start BIF generation of an item
* [DetectIntros](#detectintros) - Intro detect an item
* [CreateMarker](#createmarker) - Create a marker
* [MatchItem](#matchitem) - Match a metadata item
* [ListMatches](#listmatches) - Get metadata matches for an item
* [MergeItems](#mergeitems) - Merge a metadata item
* [SetItemPreferences](#setitempreferences) - Set metadata preferences
* [RefreshItemsMetadata](#refreshitemsmetadata) - Refresh a metadata item
* [GetRelatedItems](#getrelateditems) - Get related items
* [ListSimilar](#listsimilar) - Get similar items
* [SplitItem](#splititem) - Split a metadata item
* [GetSubtitles](#getsubtitles) - Get subtitles
* [GetItemTree](#getitemtree) - Get metadata items as a tree
* [Unmatch](#unmatch) - Unmatch a metadata item
* [ListTopUsers](#listtopusers) - Get metadata top users
* [DetectVoiceActivity](#detectvoiceactivity) - Detect voice activity
* [GetAugmentationStatus](#getaugmentationstatus) - Get augmentation status
* [SetStreamSelection](#setstreamselection) - Set stream selection
* [GetPerson](#getperson) - Get person details
* [ListPersonMedia](#listpersonmedia) - Get media for a person
* [DeleteLibrarySection](#deletelibrarysection) - Delete a library section
* [GetLibraryDetails](#getlibrarydetails) - Get a library section by id
* [EditSection](#editsection) - Edit a library section
* [GetSectionAgents](#getsectionagents) - Get Section Agents
* [UpdateItems](#updateitems) - Set the fields of the filtered items
* [StartAnalysis](#startanalysis) - Analyze a section
* [GetSectionArtists](#getsectionartists) - Get Section Artists
* [Autocomplete](#autocomplete) - Get autocompletions for search
* [GetByContentRating](#getbycontentrating) - Get By Content Rating
* [GetByDecade](#getbydecade) - Get By Decade
* [GetByFolder](#getbyfolder) - Get By Folder
* [GetByResolution](#getbyresolution) - Get By Resolution
* [GetByYear](#getbyyear) - Get By Year
* [GetSectionClips](#getsectionclips) - Get Section Clips
* [GetCollections](#getcollections) - Get collections in a section
* [GetCommon](#getcommon) - Get common fields for items
* [GetSectionEdit](#getsectionedit) - Edit Section
* [EditLibrarySection](#editlibrarysection) - Edit Section
* [EmptyTrash](#emptytrash) - Get Empty Trash
* [EmptyTrashPost](#emptytrashpost) - Empty Trash
* [EmptyTrashPut](#emptytrashput) - Empty section trash
* [GetSectionEpisodes](#getsectionepisodes) - Get Section Episodes
* [GetSectionFilters](#getsectionfilters) - Get section filters
* [GetFirstCharacters](#getfirstcharacters) - Get list of first characters
* [GetLibrarySectionHubs](#getlibrarysectionhubs) - Get Section Hubs
* [DeleteIndexes](#deleteindexes) - Delete section indexes
* [DeleteIntros](#deleteintros) - Delete section intro markers
* [GetSectionLabels](#getsectionlabels) - Get Section Labels
* [MatchSectionItems](#matchsectionitems) - Match Section Items
* [MoveSection](#movesection) - Move Section
* [GetSectionMovies](#getsectionmovies) - Get Section Movies
* [GetNewestForSection](#getnewestforsection) - Get Newest for Section
* [GetOnDeckForSection](#getondeckforsection) - Get On Deck for Section
* [OptimizeSection](#optimizesection) - Get Optimize Section
* [OptimizeSectionPost](#optimizesectionpost) - Optimize Section
* [GetSectionPhotos](#getsectionphotos) - Get Section Photos
* [GetSectionPlaylists](#getsectionplaylists) - Get Section Playlists
* [GetSectionPreferences](#getsectionpreferences) - Get section prefs
* [SetSectionPreferences](#setsectionpreferences) - Set section prefs
* [GetRecentlyAddedForSection](#getrecentlyaddedforsection) - Get Recently Added for Section
* [CancelRefresh](#cancelrefresh) - Cancel section refresh
* [RefreshSection](#refreshsection) - Get Refresh Section
* [RefreshSectionPost](#refreshsectionpost) - Refresh Section
* [SearchSection](#searchsection) - Search Section
* [GetSectionSettings](#getsectionsettings) - Get Section Settings
* [GetSectionShows](#getsectionshows) - Get Section Shows
* [GetAvailableSorts](#getavailablesorts) - Get a section sorts
* [GetSectionTags](#getsectiontags) - Get Section Tags
* [GetSectionTimeline](#getsectiontimeline) - Get Section Timeline
* [UnmatchSectionItems](#unmatchsectionitems) - Unmatch Section Items
* [GetUnwatchedForSection](#getunwatchedforsection) - Get Unwatched for Section
* [GetStreamLevels](#getstreamlevels) - Get loudness about a stream in json
* [GetStreamLoudness](#getstreamloudness) - Get loudness about a stream
* [GetChapterImage](#getchapterimage) - Get a chapter image
* [SetItemArtwork](#setitemartwork) - Set an item's artwork, theme, etc
* [UpdateItemArtwork](#updateitemartwork) - Set an item's artwork, theme, etc
* [DeleteMarker](#deletemarker) - Delete a marker
* [EditMarker](#editmarker) - Edit a marker
* [DeleteMediaItem](#deletemediaitem) - Delete a media item
* [GetPartIndex](#getpartindex) - Get BIF index for a part
* [DeleteCollection](#deletecollection) - Delete a collection
* [GetSectionImage](#getsectionimage) - Get a section composite image
* [DeleteStream](#deletestream) - Delete a stream
* [GetStream](#getstream) - Get a stream
* [SetStreamOffset](#setstreamoffset) - Set a stream offset
* [GetItemArtwork](#getitemartwork) - Get an item's artwork, theme, etc
* [GetMediaPart](#getmediapart) - Get a media part
* [GetImageFromBif](#getimagefrombif) - Get an image from part BIF

## GetRootLibrary

Get the root library object.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getRootLibrary" method="get" path="/library" -->
```csharp
using LukeHagar.PlexAPI.SDK;
using LukeHagar.PlexAPI.SDK.Models.Components;

var sdk = new PlexAPI(token: "<YOUR_API_KEY_HERE>");

var res = await sdk.Library.GetRootLibraryAsync();

// handle response
```

### Response

**[GetRootLibraryResponse](../../Models/Requests/GetRootLibraryResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetLibraryItems

Request all metadata items according to a query.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getLibraryItems" method="get" path="/library/all" -->
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

GetLibraryItemsRequest req = new GetLibraryItemsRequest() {
    MediaQuery = new MediaQuery() {
        Type = MediaType.Episode,
        Sort = "duration:desc,index",
        SourceType = 2,
    },
};

var res = await sdk.Library.GetLibraryItemsAsync(req);

// handle response
```

### Parameters

| Parameter                                                                 | Type                                                                      | Required                                                                  | Description                                                               |
| ------------------------------------------------------------------------- | ------------------------------------------------------------------------- | ------------------------------------------------------------------------- | ------------------------------------------------------------------------- |
| `request`                                                                 | [GetLibraryItemsRequest](../../Models/Requests/GetLibraryItemsRequest.md) | :heavy_check_mark:                                                        | The request object to use for the request.                                |

### Response

**[GetLibraryItemsResponse](../../Models/Requests/GetLibraryItemsResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## DeleteCaches

Delete the hub caches so they are recomputed on next request

### Example Usage

<!-- UsageSnippet language="csharp" operationID="deleteCaches" method="delete" path="/library/caches" -->
```csharp
using LukeHagar.PlexAPI.SDK;
using LukeHagar.PlexAPI.SDK.Models.Components;

var sdk = new PlexAPI(token: "<YOUR_API_KEY_HERE>");

var res = await sdk.Library.DeleteCachesAsync();

// handle response
```

### Response

**[DeleteCachesResponse](../../Models/Requests/DeleteCachesResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## CleanBundles

Clean out any now unused bundles. Bundles can become unused when media is deleted

### Example Usage

<!-- UsageSnippet language="csharp" operationID="cleanBundles" method="put" path="/library/clean/bundles" -->
```csharp
using LukeHagar.PlexAPI.SDK;
using LukeHagar.PlexAPI.SDK.Models.Components;

var sdk = new PlexAPI(token: "<YOUR_API_KEY_HERE>");

var res = await sdk.Library.CleanBundlesAsync();

// handle response
```

### Response

**[CleanBundlesResponse](../../Models/Requests/CleanBundlesResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## IngestTransientItem

This endpoint takes a file path specified in the `url` parameter, matches it using the scanner's match mechanism, downloads rich metadata, and then ingests the item as a transient item (without a library section). In the case where the file represents an episode, the entire tree (show, season, and episode) is added as transient items. At this time, movies and episodes are the only supported types, which are gleaned automatically from the file path.
Note that any of the parameters passed to the metadata details endpoint (e.g. `includeExtras=1`) work here.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="ingestTransientItem" method="post" path="/library/file" -->
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

IngestTransientItemRequest req = new IngestTransientItemRequest() {
    Url = "file:///storage%2Femulated%2F0%2FArcher-S01E01.mkv",
    VirtualFilePath = "/Avatar.mkv",
    ComputeHashes = BoolInt.True,
    IngestNonMatches = BoolInt.True,
};

var res = await sdk.Library.IngestTransientItemAsync(req);

// handle response
```

### Parameters

| Parameter                                                                         | Type                                                                              | Required                                                                          | Description                                                                       |
| --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- |
| `request`                                                                         | [IngestTransientItemRequest](../../Models/Requests/IngestTransientItemRequest.md) | :heavy_check_mark:                                                                | The request object to use for the request.                                        |

### Response

**[IngestTransientItemResponse](../../Models/Requests/IngestTransientItemResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetLibraryMatches

The matches endpoint is used to match content external to the library with content inside the library. This is done by passing a series of semantic "hints" about the content (its type, name, or release year). Each type (e.g. movie) has a canonical set of minimal required hints.
This ability to match content is useful in a variety of scenarios. For example, in the DVR, the EPG uses the endpoint to match recording rules against airing content. And in the cloud, the UMP uses the endpoint to match up a piece of media with rich metadata.
The endpoint response can including multiple matches, if there is ambiguity, each one containing a `score` from 0 to 100. For somewhat historical reasons, anything over 85 is considered a positive match (we prefer false negatives over false positives in general for matching).
The `guid` hint is somewhat special, in that it generally represents a unique identity for a piece of media (e.g. the IMDB `ttXXX`) identifier, in contrast with other hints which can be much more ambiguous (e.g. a title of `Jane Eyre`, which could refer to the 1943 or the 2011 version).
Episodes require either a season/episode pair, or an air date (or both). Either the path must be sent, or the show title

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getLibraryMatches" method="get" path="/library/matches" -->
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

GetLibraryMatchesRequest req = new GetLibraryMatchesRequest() {
    Type = MediaType.TvShow,
    IncludeFullMetadata = BoolInt.True,
    IncludeAncestorMetadata = BoolInt.True,
    IncludeAlternateMetadataSources = BoolInt.True,
};

var res = await sdk.Library.GetLibraryMatchesAsync(req);

// handle response
```

### Parameters

| Parameter                                                                     | Type                                                                          | Required                                                                      | Description                                                                   |
| ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- |
| `request`                                                                     | [GetLibraryMatchesRequest](../../Models/Requests/GetLibraryMatchesRequest.md) | :heavy_check_mark:                                                            | The request object to use for the request.                                    |

### Response

**[GetLibraryMatchesResponse](../../Models/Requests/GetLibraryMatchesResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## OptimizeLibrary

Optimize the database globally across all library sections.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="optimizeLibrary" method="get" path="/library/optimize" -->
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

OptimizeLibraryRequest req = new OptimizeLibraryRequest() {};

var res = await sdk.Library.OptimizeLibraryAsync(req);

// handle response
```

### Parameters

| Parameter                                                                 | Type                                                                      | Required                                                                  | Description                                                               |
| ------------------------------------------------------------------------- | ------------------------------------------------------------------------- | ------------------------------------------------------------------------- | ------------------------------------------------------------------------- |
| `request`                                                                 | [OptimizeLibraryRequest](../../Models/Requests/OptimizeLibraryRequest.md) | :heavy_check_mark:                                                        | The request object to use for the request.                                |

### Response

**[OptimizeLibraryResponse](../../Models/Requests/OptimizeLibraryResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## OptimizeLibraryPost

Optimize the database globally across all library sections.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="optimizeLibraryPost" method="post" path="/library/optimize" -->
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

OptimizeLibraryPostRequest req = new OptimizeLibraryPostRequest() {};

var res = await sdk.Library.OptimizeLibraryPostAsync(req);

// handle response
```

### Parameters

| Parameter                                                                         | Type                                                                              | Required                                                                          | Description                                                                       |
| --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- |
| `request`                                                                         | [OptimizeLibraryPostRequest](../../Models/Requests/OptimizeLibraryPostRequest.md) | :heavy_check_mark:                                                                | The request object to use for the request.                                        |

### Response

**[OptimizeLibraryPostResponse](../../Models/Requests/OptimizeLibraryPostResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## OptimizeDatabase

Initiate optimize on the database.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="optimizeDatabase" method="put" path="/library/optimize" -->
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

OptimizeDatabaseRequest req = new OptimizeDatabaseRequest() {
    Async = BoolInt.True,
};

var res = await sdk.Library.OptimizeDatabaseAsync(req);

// handle response
```

### Parameters

| Parameter                                                                   | Type                                                                        | Required                                                                    | Description                                                                 |
| --------------------------------------------------------------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------------------------- |
| `request`                                                                   | [OptimizeDatabaseRequest](../../Models/Requests/OptimizeDatabaseRequest.md) | :heavy_check_mark:                                                          | The request object to use for the request.                                  |

### Response

**[OptimizeDatabaseResponse](../../Models/Requests/OptimizeDatabaseResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetRandomArtwork

Get random artwork across sections.  This is commonly used for a screensaver.

This retrieves 100 random artwork paths in the specified sections and returns them.  Restrictions are put in place to not return artwork for items the user is not allowed to access.  Artwork will be for Movies, Shows, and Artists only.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getRandomArtwork" method="get" path="/library/randomArtwork" -->
```csharp
using LukeHagar.PlexAPI.SDK;
using LukeHagar.PlexAPI.SDK.Models.Components;
using LukeHagar.PlexAPI.SDK.Models.Requests;
using System.Collections.Generic;

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

GetRandomArtworkRequest req = new GetRandomArtworkRequest() {
    Sections = new List<long>() {
        5,
        6,
    },
};

var res = await sdk.Library.GetRandomArtworkAsync(req);

// handle response
```

### Parameters

| Parameter                                                                   | Type                                                                        | Required                                                                    | Description                                                                 |
| --------------------------------------------------------------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------------------------- |
| `request`                                                                   | [GetRandomArtworkRequest](../../Models/Requests/GetRandomArtworkRequest.md) | :heavy_check_mark:                                                          | The request object to use for the request.                                  |

### Response

**[GetRandomArtworkResponse](../../Models/Requests/GetRandomArtworkResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetRecentlyAddedGlobal

Get recently added items across all library sections.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getRecentlyAddedGlobal" method="get" path="/library/recentlyAdded" -->
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

GetRecentlyAddedGlobalRequest req = new GetRecentlyAddedGlobalRequest() {};

var res = await sdk.Library.GetRecentlyAddedGlobalAsync(req);

// handle response
```

### Parameters

| Parameter                                                                               | Type                                                                                    | Required                                                                                | Description                                                                             |
| --------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- |
| `request`                                                                               | [GetRecentlyAddedGlobalRequest](../../Models/Requests/GetRecentlyAddedGlobalRequest.md) | :heavy_check_mark:                                                                      | The request object to use for the request.                                              |

### Response

**[GetRecentlyAddedGlobalResponse](../../Models/Requests/GetRecentlyAddedGlobalResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetLibrarySectionsFallback

Fallback for non-owners to list library sections.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getLibrarySectionsFallback" method="get" path="/library/sections/" -->
```csharp
using LukeHagar.PlexAPI.SDK;
using LukeHagar.PlexAPI.SDK.Models.Components;

var sdk = new PlexAPI(token: "<YOUR_API_KEY_HERE>");

var res = await sdk.Library.GetLibrarySectionsFallbackAsync();

// handle response
```

### Response

**[GetLibrarySectionsFallbackResponse](../../Models/Requests/GetLibrarySectionsFallbackResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetSections

A library section (commonly referred to as just a library) is a collection of media. Libraries are typed, and depending on their type provide either a flat or a hierarchical view of the media. For example, a music library has an artist > albums > tracks structure, whereas a movie library is flat.
Libraries have features beyond just being a collection of media; for starters, they include information about supported types, filters and sorts. This allows a client to provide a rich interface around the media (e.g. allow sorting movies by release year).

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getSections" method="get" path="/library/sections/all" -->
```csharp
using LukeHagar.PlexAPI.SDK;
using LukeHagar.PlexAPI.SDK.Models.Components;

var sdk = new PlexAPI(token: "<YOUR_API_KEY_HERE>");

var res = await sdk.Library.GetSectionsAsync();

// handle response
```

### Response

**[GetSectionsResponse](../../Models/Requests/GetSectionsResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## AddSection

Add a new library section to the server

### Example Usage

<!-- UsageSnippet language="csharp" operationID="addSection" method="post" path="/library/sections/all" -->
```csharp
using LukeHagar.PlexAPI.SDK;
using LukeHagar.PlexAPI.SDK.Models.Components;
using LukeHagar.PlexAPI.SDK.Models.Requests;
using System.Collections.Generic;

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

AddSectionRequest req = new AddSectionRequest() {
    Name = "<value>",
    MediaType = 39544,
    Agent = "<value>",
    Language = "<value>",
    Locations = new List<string>() {
        "O:\\fatboy\\Media\\Ripped\\Music",
        "O:\\fatboy\\Media\\My Music",
    },
    Prefs = new QueryParamPrefs() {},
    Relative = BoolInt.True,
    ImportFromiTunes = BoolInt.True,
};

var res = await sdk.Library.AddSectionAsync(req);

// handle response
```

### Parameters

| Parameter                                                       | Type                                                            | Required                                                        | Description                                                     |
| --------------------------------------------------------------- | --------------------------------------------------------------- | --------------------------------------------------------------- | --------------------------------------------------------------- |
| `request`                                                       | [AddSectionRequest](../../Models/Requests/AddSectionRequest.md) | :heavy_check_mark:                                              | The request object to use for the request.                      |

### Response

**[AddSectionResponse](../../Models/Requests/AddSectionResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## StopAllRefreshes

Stop all refreshes across all sections

### Example Usage

<!-- UsageSnippet language="csharp" operationID="stopAllRefreshes" method="delete" path="/library/sections/all/refresh" -->
```csharp
using LukeHagar.PlexAPI.SDK;
using LukeHagar.PlexAPI.SDK.Models.Components;

var sdk = new PlexAPI(token: "<YOUR_API_KEY_HERE>");

var res = await sdk.Library.StopAllRefreshesAsync();

// handle response
```

### Response

**[StopAllRefreshesResponse](../../Models/Requests/StopAllRefreshesResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetSectionsPrefs

Get a section's preferences for a metadata type

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getSectionsPrefs" method="get" path="/library/sections/prefs" -->
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

GetSectionsPrefsRequest req = new GetSectionsPrefsRequest() {
    MediaType = 460221,
};

var res = await sdk.Library.GetSectionsPrefsAsync(req);

// handle response
```

### Parameters

| Parameter                                                                   | Type                                                                        | Required                                                                    | Description                                                                 |
| --------------------------------------------------------------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------------------------- |
| `request`                                                                   | [GetSectionsPrefsRequest](../../Models/Requests/GetSectionsPrefsRequest.md) | :heavy_check_mark:                                                          | The request object to use for the request.                                  |

### Response

**[GetSectionsPrefsResponse](../../Models/Requests/GetSectionsPrefsResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## RefreshSectionsMetadata

Tell PMS to refresh all section metadata

### Example Usage

<!-- UsageSnippet language="csharp" operationID="refreshSectionsMetadata" method="post" path="/library/sections/refresh" -->
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

RefreshSectionsMetadataRequest req = new RefreshSectionsMetadataRequest() {};

var res = await sdk.Library.RefreshSectionsMetadataAsync(req);

// handle response
```

### Parameters

| Parameter                                                                                 | Type                                                                                      | Required                                                                                  | Description                                                                               |
| ----------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------- |
| `request`                                                                                 | [RefreshSectionsMetadataRequest](../../Models/Requests/RefreshSectionsMetadataRequest.md) | :heavy_check_mark:                                                                        | The request object to use for the request.                                                |

### Response

**[RefreshSectionsMetadataResponse](../../Models/Requests/RefreshSectionsMetadataResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetTags

Get all library tags of a type

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getTags" method="get" path="/library/tags" -->
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

GetTagsRequest req = new GetTagsRequest() {
    Type = MediaType.TvShow,
};

var res = await sdk.Library.GetTagsAsync(req);

// handle response
```

### Parameters

| Parameter                                                 | Type                                                      | Required                                                  | Description                                               |
| --------------------------------------------------------- | --------------------------------------------------------- | --------------------------------------------------------- | --------------------------------------------------------- |
| `request`                                                 | [GetTagsRequest](../../Models/Requests/GetTagsRequest.md) | :heavy_check_mark:                                        | The request object to use for the request.                |

### Response

**[GetTagsResponse](../../Models/Requests/GetTagsResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## UploadArt

Upload custom background art for a metadata item.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="uploadArt" method="post" path="/library/metadata/{id}/arts" -->
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

UploadArtRequest req = new UploadArtRequest() {
    Id = 996758,
    RequestBody = new UploadArtRequestBody() {
        File = new LukeHagar.PlexAPI.SDK.Models.Requests.File() {
            FileName = "example.file",
            Content = System.IO.File.ReadAllBytes("example.file"),
        },
    },
};

var res = await sdk.Library.UploadArtAsync(req);

// handle response
```

### Parameters

| Parameter                                                     | Type                                                          | Required                                                      | Description                                                   |
| ------------------------------------------------------------- | ------------------------------------------------------------- | ------------------------------------------------------------- | ------------------------------------------------------------- |
| `request`                                                     | [UploadArtRequest](../../Models/Requests/UploadArtRequest.md) | :heavy_check_mark:                                            | The request object to use for the request.                    |

### Response

**[UploadArtResponse](../../Models/Requests/UploadArtResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetMetadataChildren

Get children of a show, season, artist, or album.

### Example Usage: include-stream

<!-- UsageSnippet language="csharp" operationID="getMetadataChildren" method="get" path="/library/metadata/{id}/children" example="include-stream" -->
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

GetMetadataChildrenRequest req = new GetMetadataChildrenRequest() {
    Id = 240367,
};

var res = await sdk.Library.GetMetadataChildrenAsync(req);

// handle response
```
### Example Usage: include-stream-otheritem

<!-- UsageSnippet language="csharp" operationID="getMetadataChildren" method="get" path="/library/metadata/{id}/children" example="include-stream-otheritem" -->
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

GetMetadataChildrenRequest req = new GetMetadataChildrenRequest() {
    Id = 240367,
};

var res = await sdk.Library.GetMetadataChildrenAsync(req);

// handle response
```
### Example Usage: include-stream-otheritem-anotheritem

<!-- UsageSnippet language="csharp" operationID="getMetadataChildren" method="get" path="/library/metadata/{id}/children" example="include-stream-otheritem-anotheritem" -->
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

GetMetadataChildrenRequest req = new GetMetadataChildrenRequest() {
    Id = 240367,
};

var res = await sdk.Library.GetMetadataChildrenAsync(req);

// handle response
```

### Parameters

| Parameter                                                                         | Type                                                                              | Required                                                                          | Description                                                                       |
| --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- |
| `request`                                                                         | [GetMetadataChildrenRequest](../../Models/Requests/GetMetadataChildrenRequest.md) | :heavy_check_mark:                                                                | The request object to use for the request.                                        |

### Response

**[GetMetadataChildrenResponse](../../Models/Requests/GetMetadataChildrenResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## ComputeSonicPath

Compute a sonic adventure path from a starting track.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="computeSonicPath" method="get" path="/library/metadata/{id}/computePath" -->
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

ComputeSonicPathRequest req = new ComputeSonicPathRequest() {
    Id = 622554,
};

var res = await sdk.Library.ComputeSonicPathAsync(req);

// handle response
```

### Parameters

| Parameter                                                                   | Type                                                                        | Required                                                                    | Description                                                                 |
| --------------------------------------------------------------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------------------------- |
| `request`                                                                   | [ComputeSonicPathRequest](../../Models/Requests/ComputeSonicPathRequest.md) | :heavy_check_mark:                                                          | The request object to use for the request.                                  |

### Response

**[ComputeSonicPathResponse](../../Models/Requests/ComputeSonicPathResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetMetadataGrandchildren

Get grandchildren (e.g. episodes under a show).

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getMetadataGrandchildren" method="get" path="/library/metadata/{id}/grandchildren" -->
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

GetMetadataGrandchildrenRequest req = new GetMetadataGrandchildrenRequest() {
    Id = 679910,
};

var res = await sdk.Library.GetMetadataGrandchildrenAsync(req);

// handle response
```

### Parameters

| Parameter                                                                                   | Type                                                                                        | Required                                                                                    | Description                                                                                 |
| ------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------- |
| `request`                                                                                   | [GetMetadataGrandchildrenRequest](../../Models/Requests/GetMetadataGrandchildrenRequest.md) | :heavy_check_mark:                                                                          | The request object to use for the request.                                                  |

### Response

**[GetMetadataGrandchildrenResponse](../../Models/Requests/GetMetadataGrandchildrenResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetMetadataGrandparent

Get grandparent metadata shortcut.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getMetadataGrandparent" method="get" path="/library/metadata/{id}/grandparent" -->
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

GetMetadataGrandparentRequest req = new GetMetadataGrandparentRequest() {
    Id = 191152,
};

var res = await sdk.Library.GetMetadataGrandparentAsync(req);

// handle response
```

### Parameters

| Parameter                                                                               | Type                                                                                    | Required                                                                                | Description                                                                             |
| --------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- |
| `request`                                                                               | [GetMetadataGrandparentRequest](../../Models/Requests/GetMetadataGrandparentRequest.md) | :heavy_check_mark:                                                                      | The request object to use for the request.                                              |

### Response

**[GetMetadataGrandparentResponse](../../Models/Requests/GetMetadataGrandparentResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetNearestMetadata

Get sonically similar items for a music track.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getNearestMetadata" method="get" path="/library/metadata/{id}/nearest" -->
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

GetNearestMetadataRequest req = new GetNearestMetadataRequest() {
    Id = 62697,
};

var res = await sdk.Library.GetNearestMetadataAsync(req);

// handle response
```

### Parameters

| Parameter                                                                       | Type                                                                            | Required                                                                        | Description                                                                     |
| ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| `request`                                                                       | [GetNearestMetadataRequest](../../Models/Requests/GetNearestMetadataRequest.md) | :heavy_check_mark:                                                              | The request object to use for the request.                                      |

### Response

**[GetNearestMetadataResponse](../../Models/Requests/GetNearestMetadataResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetMetadataOnDeck

Get On Deck status for a show or season.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getMetadataOnDeck" method="get" path="/library/metadata/{id}/onDeck" -->
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

GetMetadataOnDeckRequest req = new GetMetadataOnDeckRequest() {
    Id = 883975,
};

var res = await sdk.Library.GetMetadataOnDeckAsync(req);

// handle response
```

### Parameters

| Parameter                                                                     | Type                                                                          | Required                                                                      | Description                                                                   |
| ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- |
| `request`                                                                     | [GetMetadataOnDeckRequest](../../Models/Requests/GetMetadataOnDeckRequest.md) | :heavy_check_mark:                                                            | The request object to use for the request.                                    |

### Response

**[GetMetadataOnDeckResponse](../../Models/Requests/GetMetadataOnDeckResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetMetadataParent

Get parent metadata shortcut.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getMetadataParent" method="get" path="/library/metadata/{id}/parent" -->
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

GetMetadataParentRequest req = new GetMetadataParentRequest() {
    Id = 352555,
};

var res = await sdk.Library.GetMetadataParentAsync(req);

// handle response
```

### Parameters

| Parameter                                                                     | Type                                                                          | Required                                                                      | Description                                                                   |
| ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- |
| `request`                                                                     | [GetMetadataParentRequest](../../Models/Requests/GetMetadataParentRequest.md) | :heavy_check_mark:                                                            | The request object to use for the request.                                    |

### Response

**[GetMetadataParentResponse](../../Models/Requests/GetMetadataParentResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## UploadPoster

Upload a custom poster image for a metadata item.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="uploadPoster" method="post" path="/library/metadata/{id}/posters" -->
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

UploadPosterRequest req = new UploadPosterRequest() {
    Id = 316927,
    RequestBody = new UploadPosterRequestBody() {
        File = new UploadPosterFile() {
            FileName = "example.file",
            Content = System.IO.File.ReadAllBytes("example.file"),
        },
    },
};

var res = await sdk.Library.UploadPosterAsync(req);

// handle response
```

### Parameters

| Parameter                                                           | Type                                                                | Required                                                            | Description                                                         |
| ------------------------------------------------------------------- | ------------------------------------------------------------------- | ------------------------------------------------------------------- | ------------------------------------------------------------------- |
| `request`                                                           | [UploadPosterRequest](../../Models/Requests/UploadPosterRequest.md) | :heavy_check_mark:                                                  | The request object to use for the request.                          |

### Response

**[UploadPosterResponse](../../Models/Requests/UploadPosterResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetMetadataReviews

Get user reviews for a metadata item.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getMetadataReviews" method="get" path="/library/metadata/{id}/reviews" -->
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

GetMetadataReviewsRequest req = new GetMetadataReviewsRequest() {
    Id = 146091,
};

var res = await sdk.Library.GetMetadataReviewsAsync(req);

// handle response
```

### Parameters

| Parameter                                                                       | Type                                                                            | Required                                                                        | Description                                                                     |
| ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| `request`                                                                       | [GetMetadataReviewsRequest](../../Models/Requests/GetMetadataReviewsRequest.md) | :heavy_check_mark:                                                              | The request object to use for the request.                                      |

### Response

**[GetMetadataReviewsResponse](../../Models/Requests/GetMetadataReviewsResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## DeleteMetadataItem

Delete a single metadata item from the library, deleting media as well

### Example Usage

<!-- UsageSnippet language="csharp" operationID="deleteMetadataItem" method="delete" path="/library/metadata/{ids}" -->
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

DeleteMetadataItemRequest req = new DeleteMetadataItemRequest() {
    Ids = "<value>",
    Proxy = BoolInt.True,
};

var res = await sdk.Library.DeleteMetadataItemAsync(req);

// handle response
```

### Parameters

| Parameter                                                                       | Type                                                                            | Required                                                                        | Description                                                                     |
| ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| `request`                                                                       | [DeleteMetadataItemRequest](../../Models/Requests/DeleteMetadataItemRequest.md) | :heavy_check_mark:                                                              | The request object to use for the request.                                      |

### Response

**[DeleteMetadataItemResponse](../../Models/Requests/DeleteMetadataItemResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## EditMetadataItem

Edit metadata items setting fields

### Example Usage

<!-- UsageSnippet language="csharp" operationID="editMetadataItem" method="put" path="/library/metadata/{ids}" -->
```csharp
using LukeHagar.PlexAPI.SDK;
using LukeHagar.PlexAPI.SDK.Models.Components;
using LukeHagar.PlexAPI.SDK.Models.Requests;
using System.Collections.Generic;

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

EditMetadataItemRequest req = new EditMetadataItemRequest() {
    Ids = new List<string>() {
        "<value 1>",
        "<value 2>",
    },
};

var res = await sdk.Library.EditMetadataItemAsync(req);

// handle response
```

### Parameters

| Parameter                                                                   | Type                                                                        | Required                                                                    | Description                                                                 |
| --------------------------------------------------------------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------------------------- |
| `request`                                                                   | [EditMetadataItemRequest](../../Models/Requests/EditMetadataItemRequest.md) | :heavy_check_mark:                                                          | The request object to use for the request.                                  |

### Response

**[EditMetadataItemResponse](../../Models/Requests/EditMetadataItemResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## DetectAds

Start the detection of ads in a metadata item

### Example Usage

<!-- UsageSnippet language="csharp" operationID="detectAds" method="put" path="/library/metadata/{ids}/addetect" -->
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

DetectAdsRequest req = new DetectAdsRequest() {
    Ids = "<value>",
};

var res = await sdk.Library.DetectAdsAsync(req);

// handle response
```

### Parameters

| Parameter                                                     | Type                                                          | Required                                                      | Description                                                   |
| ------------------------------------------------------------- | ------------------------------------------------------------- | ------------------------------------------------------------- | ------------------------------------------------------------- |
| `request`                                                     | [DetectAdsRequest](../../Models/Requests/DetectAdsRequest.md) | :heavy_check_mark:                                            | The request object to use for the request.                    |

### Response

**[DetectAdsResponse](../../Models/Requests/DetectAdsResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetAllItemLeaves

Get the leaves for a metadata item such as the episodes in a show

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getAllItemLeaves" method="get" path="/library/metadata/{ids}/allLeaves" -->
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

GetAllItemLeavesRequest req = new GetAllItemLeavesRequest() {
    Ids = "<value>",
};

var res = await sdk.Library.GetAllItemLeavesAsync(req);

// handle response
```

### Parameters

| Parameter                                                                   | Type                                                                        | Required                                                                    | Description                                                                 |
| --------------------------------------------------------------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------------------------- |
| `request`                                                                   | [GetAllItemLeavesRequest](../../Models/Requests/GetAllItemLeavesRequest.md) | :heavy_check_mark:                                                          | The request object to use for the request.                                  |

### Response

**[GetAllItemLeavesResponse](../../Models/Requests/GetAllItemLeavesResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## AnalyzeMetadata

Start the analysis of a metadata item

### Example Usage

<!-- UsageSnippet language="csharp" operationID="analyzeMetadata" method="put" path="/library/metadata/{ids}/analyze" -->
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

AnalyzeMetadataRequest req = new AnalyzeMetadataRequest() {
    Ids = "<value>",
};

var res = await sdk.Library.AnalyzeMetadataAsync(req);

// handle response
```

### Parameters

| Parameter                                                                 | Type                                                                      | Required                                                                  | Description                                                               |
| ------------------------------------------------------------------------- | ------------------------------------------------------------------------- | ------------------------------------------------------------------------- | ------------------------------------------------------------------------- |
| `request`                                                                 | [AnalyzeMetadataRequest](../../Models/Requests/AnalyzeMetadataRequest.md) | :heavy_check_mark:                                                        | The request object to use for the request.                                |

### Response

**[AnalyzeMetadataResponse](../../Models/Requests/AnalyzeMetadataResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GenerateThumbs

Start the chapter thumb generation for an item

### Example Usage

<!-- UsageSnippet language="csharp" operationID="generateThumbs" method="put" path="/library/metadata/{ids}/chapterThumbs" -->
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

GenerateThumbsRequest req = new GenerateThumbsRequest() {
    Ids = "<value>",
    Force = BoolInt.True,
};

var res = await sdk.Library.GenerateThumbsAsync(req);

// handle response
```

### Parameters

| Parameter                                                               | Type                                                                    | Required                                                                | Description                                                             |
| ----------------------------------------------------------------------- | ----------------------------------------------------------------------- | ----------------------------------------------------------------------- | ----------------------------------------------------------------------- |
| `request`                                                               | [GenerateThumbsRequest](../../Models/Requests/GenerateThumbsRequest.md) | :heavy_check_mark:                                                      | The request object to use for the request.                              |

### Response

**[GenerateThumbsResponse](../../Models/Requests/GenerateThumbsResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## DetectCredits

Start credit detection on a metadata item

### Example Usage

<!-- UsageSnippet language="csharp" operationID="detectCredits" method="put" path="/library/metadata/{ids}/credits" -->
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

DetectCreditsRequest req = new DetectCreditsRequest() {
    Ids = "<value>",
    Force = BoolInt.True,
    Manual = BoolInt.True,
};

var res = await sdk.Library.DetectCreditsAsync(req);

// handle response
```

### Parameters

| Parameter                                                             | Type                                                                  | Required                                                              | Description                                                           |
| --------------------------------------------------------------------- | --------------------------------------------------------------------- | --------------------------------------------------------------------- | --------------------------------------------------------------------- |
| `request`                                                             | [DetectCreditsRequest](../../Models/Requests/DetectCreditsRequest.md) | :heavy_check_mark:                                                    | The request object to use for the request.                            |

### Response

**[DetectCreditsResponse](../../Models/Requests/DetectCreditsResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetExtras

Get the extras for a metadata item

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getExtras" method="get" path="/library/metadata/{ids}/extras" -->
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

GetExtrasRequest req = new GetExtrasRequest() {
    Ids = "<value>",
};

var res = await sdk.Library.GetExtrasAsync(req);

// handle response
```

### Parameters

| Parameter                                                     | Type                                                          | Required                                                      | Description                                                   |
| ------------------------------------------------------------- | ------------------------------------------------------------- | ------------------------------------------------------------- | ------------------------------------------------------------- |
| `request`                                                     | [GetExtrasRequest](../../Models/Requests/GetExtrasRequest.md) | :heavy_check_mark:                                            | The request object to use for the request.                    |

### Response

**[GetExtrasResponse](../../Models/Requests/GetExtrasResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## AddExtras

Add an extra to a metadata item

### Example Usage

<!-- UsageSnippet language="csharp" operationID="addExtras" method="post" path="/library/metadata/{ids}/extras" -->
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

AddExtrasRequest req = new AddExtrasRequest() {
    Ids = "<value>",
    Url = "https://super-mortise.biz/",
};

var res = await sdk.Library.AddExtrasAsync(req);

// handle response
```

### Parameters

| Parameter                                                     | Type                                                          | Required                                                      | Description                                                   |
| ------------------------------------------------------------- | ------------------------------------------------------------- | ------------------------------------------------------------- | ------------------------------------------------------------- |
| `request`                                                     | [AddExtrasRequest](../../Models/Requests/AddExtrasRequest.md) | :heavy_check_mark:                                            | The request object to use for the request.                    |

### Response

**[AddExtrasResponse](../../Models/Requests/AddExtrasResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetFile

Get a bundle file for a metadata or media item.  This is either an image or a mp3 (for a show's theme)

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getFile" method="get" path="/library/metadata/{ids}/file" -->
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

GetFileRequest req = new GetFileRequest() {
    Ids = "<value>",
};

var res = await sdk.Library.GetFileAsync(req);

// handle response
```

### Parameters

| Parameter                                                 | Type                                                      | Required                                                  | Description                                               |
| --------------------------------------------------------- | --------------------------------------------------------- | --------------------------------------------------------- | --------------------------------------------------------- |
| `request`                                                 | [GetFileRequest](../../Models/Requests/GetFileRequest.md) | :heavy_check_mark:                                        | The request object to use for the request.                |

### Response

**[GetFileResponse](../../Models/Requests/GetFileResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## StartBifGeneration

Start the indexing (BIF generation) of an item

### Example Usage

<!-- UsageSnippet language="csharp" operationID="startBifGeneration" method="put" path="/library/metadata/{ids}/index" -->
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

StartBifGenerationRequest req = new StartBifGenerationRequest() {
    Ids = "<value>",
    Force = BoolInt.True,
};

var res = await sdk.Library.StartBifGenerationAsync(req);

// handle response
```

### Parameters

| Parameter                                                                       | Type                                                                            | Required                                                                        | Description                                                                     |
| ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| `request`                                                                       | [StartBifGenerationRequest](../../Models/Requests/StartBifGenerationRequest.md) | :heavy_check_mark:                                                              | The request object to use for the request.                                      |

### Response

**[StartBifGenerationResponse](../../Models/Requests/StartBifGenerationResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## DetectIntros

Start the detection of intros in a metadata item

### Example Usage

<!-- UsageSnippet language="csharp" operationID="detectIntros" method="put" path="/library/metadata/{ids}/intro" -->
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

DetectIntrosRequest req = new DetectIntrosRequest() {
    Ids = "<value>",
    Force = BoolInt.True,
};

var res = await sdk.Library.DetectIntrosAsync(req);

// handle response
```

### Parameters

| Parameter                                                           | Type                                                                | Required                                                            | Description                                                         |
| ------------------------------------------------------------------- | ------------------------------------------------------------------- | ------------------------------------------------------------------- | ------------------------------------------------------------------- |
| `request`                                                           | [DetectIntrosRequest](../../Models/Requests/DetectIntrosRequest.md) | :heavy_check_mark:                                                  | The request object to use for the request.                          |

### Response

**[DetectIntrosResponse](../../Models/Requests/DetectIntrosResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## CreateMarker

Create a marker for this user on the metadata item

### Example Usage

<!-- UsageSnippet language="csharp" operationID="createMarker" method="post" path="/library/metadata/{ids}/marker" -->
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

CreateMarkerRequest req = new CreateMarkerRequest() {
    Ids = "<value>",
    MediaType = 248391,
    StartTimeOffset = 535191,
    Attributes = new Attributes() {},
};

var res = await sdk.Library.CreateMarkerAsync(req);

// handle response
```

### Parameters

| Parameter                                                           | Type                                                                | Required                                                            | Description                                                         |
| ------------------------------------------------------------------- | ------------------------------------------------------------------- | ------------------------------------------------------------------- | ------------------------------------------------------------------- |
| `request`                                                           | [CreateMarkerRequest](../../Models/Requests/CreateMarkerRequest.md) | :heavy_check_mark:                                                  | The request object to use for the request.                          |

### Response

**[CreateMarkerResponse](../../Models/Requests/CreateMarkerResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## MatchItem

Match a metadata item to a guid

### Example Usage

<!-- UsageSnippet language="csharp" operationID="matchItem" method="put" path="/library/metadata/{ids}/match" -->
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

MatchItemRequest req = new MatchItemRequest() {
    Ids = "<value>",
};

var res = await sdk.Library.MatchItemAsync(req);

// handle response
```

### Parameters

| Parameter                                                     | Type                                                          | Required                                                      | Description                                                   |
| ------------------------------------------------------------- | ------------------------------------------------------------- | ------------------------------------------------------------- | ------------------------------------------------------------- |
| `request`                                                     | [MatchItemRequest](../../Models/Requests/MatchItemRequest.md) | :heavy_check_mark:                                            | The request object to use for the request.                    |

### Response

**[MatchItemResponse](../../Models/Requests/MatchItemResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## ListMatches

Get the list of metadata matches for a metadata item

### Example Usage

<!-- UsageSnippet language="csharp" operationID="listMatches" method="put" path="/library/metadata/{ids}/matches" -->
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

ListMatchesRequest req = new ListMatchesRequest() {
    Ids = "<value>",
    Manual = BoolInt.True,
};

var res = await sdk.Library.ListMatchesAsync(req);

// handle response
```

### Parameters

| Parameter                                                         | Type                                                              | Required                                                          | Description                                                       |
| ----------------------------------------------------------------- | ----------------------------------------------------------------- | ----------------------------------------------------------------- | ----------------------------------------------------------------- |
| `request`                                                         | [ListMatchesRequest](../../Models/Requests/ListMatchesRequest.md) | :heavy_check_mark:                                                | The request object to use for the request.                        |

### Response

**[ListMatchesResponse](../../Models/Requests/ListMatchesResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## MergeItems

Merge a metadata item with other items

### Example Usage

<!-- UsageSnippet language="csharp" operationID="mergeItems" method="put" path="/library/metadata/{ids}/merge" -->
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

MergeItemsRequest req = new MergeItemsRequest() {
    IdsPathParameter = "<value>",
};

var res = await sdk.Library.MergeItemsAsync(req);

// handle response
```

### Parameters

| Parameter                                                       | Type                                                            | Required                                                        | Description                                                     |
| --------------------------------------------------------------- | --------------------------------------------------------------- | --------------------------------------------------------------- | --------------------------------------------------------------- |
| `request`                                                       | [MergeItemsRequest](../../Models/Requests/MergeItemsRequest.md) | :heavy_check_mark:                                              | The request object to use for the request.                      |

### Response

**[MergeItemsResponse](../../Models/Requests/MergeItemsResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## SetItemPreferences

Set the preferences on a metadata item

### Example Usage

<!-- UsageSnippet language="csharp" operationID="setItemPreferences" method="put" path="/library/metadata/{ids}/prefs" -->
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

SetItemPreferencesRequest req = new SetItemPreferencesRequest() {
    Ids = "<value>",
};

var res = await sdk.Library.SetItemPreferencesAsync(req);

// handle response
```

### Parameters

| Parameter                                                                       | Type                                                                            | Required                                                                        | Description                                                                     |
| ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| `request`                                                                       | [SetItemPreferencesRequest](../../Models/Requests/SetItemPreferencesRequest.md) | :heavy_check_mark:                                                              | The request object to use for the request.                                      |

### Response

**[SetItemPreferencesResponse](../../Models/Requests/SetItemPreferencesResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## RefreshItemsMetadata

Refresh a metadata item from the agent

### Example Usage

<!-- UsageSnippet language="csharp" operationID="refreshItemsMetadata" method="put" path="/library/metadata/{ids}/refresh" -->
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

RefreshItemsMetadataRequest req = new RefreshItemsMetadataRequest() {
    Ids = "<value>",
    MarkUpdated = BoolInt.True,
    SkipRefresh = BoolInt.True,
};

var res = await sdk.Library.RefreshItemsMetadataAsync(req);

// handle response
```

### Parameters

| Parameter                                                                           | Type                                                                                | Required                                                                            | Description                                                                         |
| ----------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- |
| `request`                                                                           | [RefreshItemsMetadataRequest](../../Models/Requests/RefreshItemsMetadataRequest.md) | :heavy_check_mark:                                                                  | The request object to use for the request.                                          |

### Response

**[RefreshItemsMetadataResponse](../../Models/Requests/RefreshItemsMetadataResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetRelatedItems

Get a hub of related items to a metadata item

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getRelatedItems" method="get" path="/library/metadata/{ids}/related" -->
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

GetRelatedItemsRequest req = new GetRelatedItemsRequest() {
    Ids = "<value>",
};

var res = await sdk.Library.GetRelatedItemsAsync(req);

// handle response
```

### Parameters

| Parameter                                                                 | Type                                                                      | Required                                                                  | Description                                                               |
| ------------------------------------------------------------------------- | ------------------------------------------------------------------------- | ------------------------------------------------------------------------- | ------------------------------------------------------------------------- |
| `request`                                                                 | [GetRelatedItemsRequest](../../Models/Requests/GetRelatedItemsRequest.md) | :heavy_check_mark:                                                        | The request object to use for the request.                                |

### Response

**[GetRelatedItemsResponse](../../Models/Requests/GetRelatedItemsResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## ListSimilar

Get a list of similar items to a metadata item

### Example Usage

<!-- UsageSnippet language="csharp" operationID="listSimilar" method="get" path="/library/metadata/{ids}/similar" -->
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

ListSimilarRequest req = new ListSimilarRequest() {
    Ids = "<value>",
};

var res = await sdk.Library.ListSimilarAsync(req);

// handle response
```

### Parameters

| Parameter                                                         | Type                                                              | Required                                                          | Description                                                       |
| ----------------------------------------------------------------- | ----------------------------------------------------------------- | ----------------------------------------------------------------- | ----------------------------------------------------------------- |
| `request`                                                         | [ListSimilarRequest](../../Models/Requests/ListSimilarRequest.md) | :heavy_check_mark:                                                | The request object to use for the request.                        |

### Response

**[ListSimilarResponse](../../Models/Requests/ListSimilarResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## SplitItem

Split a metadata item into multiple items

### Example Usage

<!-- UsageSnippet language="csharp" operationID="splitItem" method="put" path="/library/metadata/{ids}/split" -->
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

SplitItemRequest req = new SplitItemRequest() {
    Ids = "<value>",
};

var res = await sdk.Library.SplitItemAsync(req);

// handle response
```

### Parameters

| Parameter                                                     | Type                                                          | Required                                                      | Description                                                   |
| ------------------------------------------------------------- | ------------------------------------------------------------- | ------------------------------------------------------------- | ------------------------------------------------------------- |
| `request`                                                     | [SplitItemRequest](../../Models/Requests/SplitItemRequest.md) | :heavy_check_mark:                                            | The request object to use for the request.                    |

### Response

**[SplitItemResponse](../../Models/Requests/SplitItemResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetSubtitles

Add a subtitle to a metadata item

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getSubtitles" method="get" path="/library/metadata/{ids}/subtitles" -->
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

GetSubtitlesRequest req = new GetSubtitlesRequest() {
    Ids = "<value>",
    Forced = BoolInt.True,
    HearingImpaired = BoolInt.True,
};

var res = await sdk.Library.GetSubtitlesAsync(req);

// handle response
```

### Parameters

| Parameter                                                           | Type                                                                | Required                                                            | Description                                                         |
| ------------------------------------------------------------------- | ------------------------------------------------------------------- | ------------------------------------------------------------------- | ------------------------------------------------------------------- |
| `request`                                                           | [GetSubtitlesRequest](../../Models/Requests/GetSubtitlesRequest.md) | :heavy_check_mark:                                                  | The request object to use for the request.                          |

### Response

**[GetSubtitlesResponse](../../Models/Requests/GetSubtitlesResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetItemTree

Get a tree of metadata items, such as the seasons/episodes of a show

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getItemTree" method="get" path="/library/metadata/{ids}/tree" -->
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

GetItemTreeRequest req = new GetItemTreeRequest() {
    Ids = "<value>",
};

var res = await sdk.Library.GetItemTreeAsync(req);

// handle response
```

### Parameters

| Parameter                                                         | Type                                                              | Required                                                          | Description                                                       |
| ----------------------------------------------------------------- | ----------------------------------------------------------------- | ----------------------------------------------------------------- | ----------------------------------------------------------------- |
| `request`                                                         | [GetItemTreeRequest](../../Models/Requests/GetItemTreeRequest.md) | :heavy_check_mark:                                                | The request object to use for the request.                        |

### Response

**[GetItemTreeResponse](../../Models/Requests/GetItemTreeResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## Unmatch

Unmatch a metadata item to info fetched from the agent

### Example Usage

<!-- UsageSnippet language="csharp" operationID="unmatch" method="put" path="/library/metadata/{ids}/unmatch" -->
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

UnmatchRequest req = new UnmatchRequest() {
    Ids = "<value>",
};

var res = await sdk.Library.UnmatchAsync(req);

// handle response
```

### Parameters

| Parameter                                                 | Type                                                      | Required                                                  | Description                                               |
| --------------------------------------------------------- | --------------------------------------------------------- | --------------------------------------------------------- | --------------------------------------------------------- |
| `request`                                                 | [UnmatchRequest](../../Models/Requests/UnmatchRequest.md) | :heavy_check_mark:                                        | The request object to use for the request.                |

### Response

**[UnmatchResponse](../../Models/Requests/UnmatchResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## ListTopUsers

Get the list of users which have played this item starting with the most

### Example Usage

<!-- UsageSnippet language="csharp" operationID="listTopUsers" method="get" path="/library/metadata/{ids}/users/top" -->
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

ListTopUsersRequest req = new ListTopUsersRequest() {
    Ids = "<value>",
};

var res = await sdk.Library.ListTopUsersAsync(req);

// handle response
```

### Parameters

| Parameter                                                           | Type                                                                | Required                                                            | Description                                                         |
| ------------------------------------------------------------------- | ------------------------------------------------------------------- | ------------------------------------------------------------------- | ------------------------------------------------------------------- |
| `request`                                                           | [ListTopUsersRequest](../../Models/Requests/ListTopUsersRequest.md) | :heavy_check_mark:                                                  | The request object to use for the request.                          |

### Response

**[ListTopUsersResponse](../../Models/Requests/ListTopUsersResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## DetectVoiceActivity

Start the detection of voice in a metadata item

### Example Usage

<!-- UsageSnippet language="csharp" operationID="detectVoiceActivity" method="put" path="/library/metadata/{ids}/voiceActivity" -->
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

DetectVoiceActivityRequest req = new DetectVoiceActivityRequest() {
    Ids = "<value>",
    Force = BoolInt.True,
    Manual = BoolInt.True,
};

var res = await sdk.Library.DetectVoiceActivityAsync(req);

// handle response
```

### Parameters

| Parameter                                                                         | Type                                                                              | Required                                                                          | Description                                                                       |
| --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- |
| `request`                                                                         | [DetectVoiceActivityRequest](../../Models/Requests/DetectVoiceActivityRequest.md) | :heavy_check_mark:                                                                | The request object to use for the request.                                        |

### Response

**[DetectVoiceActivityResponse](../../Models/Requests/DetectVoiceActivityResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetAugmentationStatus

Get augmentation status and potentially wait for completion

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getAugmentationStatus" method="get" path="/library/metadata/augmentations/{augmentationId}" -->
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

GetAugmentationStatusRequest req = new GetAugmentationStatusRequest() {
    AugmentationId = "<id>",
    Wait = BoolInt.True,
};

var res = await sdk.Library.GetAugmentationStatusAsync(req);

// handle response
```

### Parameters

| Parameter                                                                             | Type                                                                                  | Required                                                                              | Description                                                                           |
| ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- |
| `request`                                                                             | [GetAugmentationStatusRequest](../../Models/Requests/GetAugmentationStatusRequest.md) | :heavy_check_mark:                                                                    | The request object to use for the request.                                            |

### Response

**[GetAugmentationStatusResponse](../../Models/Requests/GetAugmentationStatusResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## SetStreamSelection

Set which streams (audio/subtitle) are selected by this user

### Example Usage

<!-- UsageSnippet language="csharp" operationID="setStreamSelection" method="put" path="/library/parts/{partId}" -->
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

SetStreamSelectionRequest req = new SetStreamSelectionRequest() {
    PartId = 360489,
    AllParts = BoolInt.True,
};

var res = await sdk.Library.SetStreamSelectionAsync(req);

// handle response
```

### Parameters

| Parameter                                                                       | Type                                                                            | Required                                                                        | Description                                                                     |
| ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| `request`                                                                       | [SetStreamSelectionRequest](../../Models/Requests/SetStreamSelectionRequest.md) | :heavy_check_mark:                                                              | The request object to use for the request.                                      |

### Response

**[SetStreamSelectionResponse](../../Models/Requests/SetStreamSelectionResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetPerson

Get details for a single actor.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getPerson" method="get" path="/library/people/{personId}" -->
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

GetPersonRequest req = new GetPersonRequest() {
    PersonId = "<id>",
};

var res = await sdk.Library.GetPersonAsync(req);

// handle response
```

### Parameters

| Parameter                                                     | Type                                                          | Required                                                      | Description                                                   |
| ------------------------------------------------------------- | ------------------------------------------------------------- | ------------------------------------------------------------- | ------------------------------------------------------------- |
| `request`                                                     | [GetPersonRequest](../../Models/Requests/GetPersonRequest.md) | :heavy_check_mark:                                            | The request object to use for the request.                    |

### Response

**[GetPersonResponse](../../Models/Requests/GetPersonResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## ListPersonMedia

Get all the media for a single actor.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="listPersonMedia" method="get" path="/library/people/{personId}/media" -->
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

ListPersonMediaRequest req = new ListPersonMediaRequest() {
    PersonId = "<id>",
};

var res = await sdk.Library.ListPersonMediaAsync(req);

// handle response
```

### Parameters

| Parameter                                                                 | Type                                                                      | Required                                                                  | Description                                                               |
| ------------------------------------------------------------------------- | ------------------------------------------------------------------------- | ------------------------------------------------------------------------- | ------------------------------------------------------------------------- |
| `request`                                                                 | [ListPersonMediaRequest](../../Models/Requests/ListPersonMediaRequest.md) | :heavy_check_mark:                                                        | The request object to use for the request.                                |

### Response

**[ListPersonMediaResponse](../../Models/Requests/ListPersonMediaResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## DeleteLibrarySection

Delete a library section by id

### Example Usage

<!-- UsageSnippet language="csharp" operationID="deleteLibrarySection" method="delete" path="/library/sections/{sectionId}" -->
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

DeleteLibrarySectionRequest req = new DeleteLibrarySectionRequest() {
    SectionId = "<id>",
    Async = BoolInt.True,
};

var res = await sdk.Library.DeleteLibrarySectionAsync(req);

// handle response
```

### Parameters

| Parameter                                                                           | Type                                                                                | Required                                                                            | Description                                                                         |
| ----------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- |
| `request`                                                                           | [DeleteLibrarySectionRequest](../../Models/Requests/DeleteLibrarySectionRequest.md) | :heavy_check_mark:                                                                  | The request object to use for the request.                                          |

### Response

**[DeleteLibrarySectionResponse](../../Models/Requests/DeleteLibrarySectionResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetLibraryDetails

Returns details for the library. This can be thought of as an interstitial endpoint because it contains information about the library, rather than content itself. It often contains a list of `Directory` metadata objects: These used to be used by clients to build a menuing system.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getLibraryDetails" method="get" path="/library/sections/{sectionId}" -->
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

GetLibraryDetailsRequest req = new GetLibraryDetailsRequest() {
    SectionId = "<id>",
    IncludeDetails = BoolInt.True,
};

var res = await sdk.Library.GetLibraryDetailsAsync(req);

// handle response
```

### Parameters

| Parameter                                                                     | Type                                                                          | Required                                                                      | Description                                                                   |
| ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- |
| `request`                                                                     | [GetLibraryDetailsRequest](../../Models/Requests/GetLibraryDetailsRequest.md) | :heavy_check_mark:                                                            | The request object to use for the request.                                    |

### Response

**[GetLibraryDetailsResponse](../../Models/Requests/GetLibraryDetailsResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## EditSection

Edit a library section by id setting parameters

### Example Usage

<!-- UsageSnippet language="csharp" operationID="editSection" method="put" path="/library/sections/{sectionId}" -->
```csharp
using LukeHagar.PlexAPI.SDK;
using LukeHagar.PlexAPI.SDK.Models.Components;
using LukeHagar.PlexAPI.SDK.Models.Requests;
using System.Collections.Generic;

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

EditSectionRequest req = new EditSectionRequest() {
    SectionId = "<id>",
    Agent = "<value>",
    Locations = new List<string>() {
        "O:\\fatboy\\Media\\Ripped\\Music",
        "O:\\fatboy\\Media\\My Music",
    },
    Prefs = new EditSectionQueryParamPrefs() {},
};

var res = await sdk.Library.EditSectionAsync(req);

// handle response
```

### Parameters

| Parameter                                                         | Type                                                              | Required                                                          | Description                                                       |
| ----------------------------------------------------------------- | ----------------------------------------------------------------- | ----------------------------------------------------------------- | ----------------------------------------------------------------- |
| `request`                                                         | [EditSectionRequest](../../Models/Requests/EditSectionRequest.md) | :heavy_check_mark:                                                | The request object to use for the request.                        |

### Response

**[EditSectionResponse](../../Models/Requests/EditSectionResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetSectionAgents

Get available metadata agents for a library section.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getSectionAgents" method="get" path="/library/sections/{sectionId}/agents" -->
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

GetSectionAgentsRequest req = new GetSectionAgentsRequest() {
    SectionId = 757906,
};

var res = await sdk.Library.GetSectionAgentsAsync(req);

// handle response
```

### Parameters

| Parameter                                                                   | Type                                                                        | Required                                                                    | Description                                                                 |
| --------------------------------------------------------------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------------------------- |
| `request`                                                                   | [GetSectionAgentsRequest](../../Models/Requests/GetSectionAgentsRequest.md) | :heavy_check_mark:                                                          | The request object to use for the request.                                  |

### Response

**[GetSectionAgentsResponse](../../Models/Requests/GetSectionAgentsResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## UpdateItems

This endpoint takes an large possible set of values.  Here are some examples.
- **Parameters, extra documentation**
  - artist.title.value
      - When used with track, both artist.title.value and album.title.value need to be specified
  - title.value usage
      - Summary
          - Tracks always rename and never merge
          - Albums and Artists
              - if single item and item without title does not exist, it is renamed.
              - if single item and item with title does exist they are merged.
              - if multiple they are always merged.
      - Tracks
          - Works as expected will update the track's title
          - Single track:    `/library/sections/{id}/all?type=10&id=42&title.value=NewName`
          - Multiple tracks: `/library/sections/{id}/all?type=10&id=42,43,44&title.value=NewName`
          - All tracks:      `/library/sections/{id}/all?type=10&title.value=NewName`
      - Albums
          - Functionality changes depending on the existence of an album with the same title
          - Album exists
              - Single album: `/library/sections/{id}/all?type=9&id=42&title.value=Album 2`
                  - Album with id 42 is merged into album titled "Album 2"
              - Multiple/All albums: `/library/sections/{id}/all?type=9&title.value=Moo Album`
                  - All albums are merged into the existing album titled "Moo Album"
          - Album does not exist
              - Single album: `/library/sections/{id}/all?type=9&id=42&title.value=NewAlbumTitle`
                  - Album with id 42 has title modified to "NewAlbumTitle"
              - Multiple/All albums: `/library/sections/{id}/all?type=9&title.value=NewAlbumTitle`
                  - All albums are merged into a new album with title="NewAlbumTitle"
      - Artists
          - Functionaly changes depending on the existence of an artist with the same title.
          - Artist exists
              - Single artist: `/library/sections/{id}/all?type=8&id=42&title.value=Artist 2`
                  - Artist with id 42 is merged into existing artist titled "Artist 2"
              - Multiple/All artists: `/library/sections/{id}/all?type=8&title.value=Artist 3`
                  - All artists are merged into the existing artist titled "Artist 3"
          - Artist does not exist
              - Single artist: `/library/sections/{id}/all?type=8&id=42&title.value=NewArtistTitle`
                  - Artist with id 42 has title modified to "NewArtistTitle"
              - Multiple/All artists: `/library/sections/{id}/all?type=8&title.value=NewArtistTitle`
                  - All artists are merged into a new artist with title="NewArtistTitle"

- **Notes**
    - Technically square brackets are not allowed in an URI except the Internet Protocol Literal Address
    - RFC3513: A host identified by an Internet Protocol literal address, version 6 [RFC3513] or later, is distinguished by enclosing the IP literal within square brackets ("[" and "]"). This is the only place where square bracket characters are allowed in the URI syntax.
    - Escaped square brackets are allowed, but don't render well

### Example Usage

<!-- UsageSnippet language="csharp" operationID="updateItems" method="put" path="/library/sections/{sectionId}/all" -->
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

UpdateItemsRequest req = new UpdateItemsRequest() {
    SectionId = "<id>",
    FieldLocked = BoolInt.True,
};

var res = await sdk.Library.UpdateItemsAsync(req);

// handle response
```

### Parameters

| Parameter                                                         | Type                                                              | Required                                                          | Description                                                       |
| ----------------------------------------------------------------- | ----------------------------------------------------------------- | ----------------------------------------------------------------- | ----------------------------------------------------------------- |
| `request`                                                         | [UpdateItemsRequest](../../Models/Requests/UpdateItemsRequest.md) | :heavy_check_mark:                                                | The request object to use for the request.                        |

### Response

**[UpdateItemsResponse](../../Models/Requests/UpdateItemsResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## StartAnalysis

Start analysis of all items in a section.  If BIF generation is enabled, this will also be started on this section

### Example Usage

<!-- UsageSnippet language="csharp" operationID="startAnalysis" method="put" path="/library/sections/{sectionId}/analyze" -->
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

StartAnalysisRequest req = new StartAnalysisRequest() {
    SectionId = 158829,
};

var res = await sdk.Library.StartAnalysisAsync(req);

// handle response
```

### Parameters

| Parameter                                                             | Type                                                                  | Required                                                              | Description                                                           |
| --------------------------------------------------------------------- | --------------------------------------------------------------------- | --------------------------------------------------------------------- | --------------------------------------------------------------------- |
| `request`                                                             | [StartAnalysisRequest](../../Models/Requests/StartAnalysisRequest.md) | :heavy_check_mark:                                                    | The request object to use for the request.                            |

### Response

**[StartAnalysisResponse](../../Models/Requests/StartAnalysisResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetSectionArtists

Get artists for a music library section.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getSectionArtists" method="get" path="/library/sections/{sectionId}/artists" -->
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

GetSectionArtistsRequest req = new GetSectionArtistsRequest() {
    SectionId = 716398,
};

var res = await sdk.Library.GetSectionArtistsAsync(req);

// handle response
```

### Parameters

| Parameter                                                                     | Type                                                                          | Required                                                                      | Description                                                                   |
| ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- |
| `request`                                                                     | [GetSectionArtistsRequest](../../Models/Requests/GetSectionArtistsRequest.md) | :heavy_check_mark:                                                            | The request object to use for the request.                                    |

### Response

**[GetSectionArtistsResponse](../../Models/Requests/GetSectionArtistsResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## Autocomplete

The field to autocomplete on is specified by the `{field}.query` parameter. For example `genre.query` or `title.query`.
Returns a set of items from the filtered items whose `{field}` starts with `{field}.query`.  In the results, a `{field}.queryRange` will be present to express the range of the match

### Example Usage

<!-- UsageSnippet language="csharp" operationID="autocomplete" method="get" path="/library/sections/{sectionId}/autocomplete" -->
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

AutocompleteRequest req = new AutocompleteRequest() {
    MediaQuery = new MediaQuery() {
        Type = MediaType.Episode,
        Sort = "duration:desc,index",
        SourceType = 2,
    },
    SectionId = 942007,
};

var res = await sdk.Library.AutocompleteAsync(req);

// handle response
```

### Parameters

| Parameter                                                           | Type                                                                | Required                                                            | Description                                                         |
| ------------------------------------------------------------------- | ------------------------------------------------------------------- | ------------------------------------------------------------------- | ------------------------------------------------------------------- |
| `request`                                                           | [AutocompleteRequest](../../Models/Requests/AutocompleteRequest.md) | :heavy_check_mark:                                                  | The request object to use for the request.                          |

### Response

**[AutocompleteResponse](../../Models/Requests/AutocompleteResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetByContentRating

Browse items in a library section grouped by content rating.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getByContentRating" method="get" path="/library/sections/{sectionId}/byContentRating" -->
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

GetByContentRatingRequest req = new GetByContentRatingRequest() {
    SectionId = 586837,
};

var res = await sdk.Library.GetByContentRatingAsync(req);

// handle response
```

### Parameters

| Parameter                                                                       | Type                                                                            | Required                                                                        | Description                                                                     |
| ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| `request`                                                                       | [GetByContentRatingRequest](../../Models/Requests/GetByContentRatingRequest.md) | :heavy_check_mark:                                                              | The request object to use for the request.                                      |

### Response

**[GetByContentRatingResponse](../../Models/Requests/GetByContentRatingResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetByDecade

Browse items in a library section grouped by decade.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getByDecade" method="get" path="/library/sections/{sectionId}/byDecade" -->
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

GetByDecadeRequest req = new GetByDecadeRequest() {
    SectionId = 212187,
};

var res = await sdk.Library.GetByDecadeAsync(req);

// handle response
```

### Parameters

| Parameter                                                         | Type                                                              | Required                                                          | Description                                                       |
| ----------------------------------------------------------------- | ----------------------------------------------------------------- | ----------------------------------------------------------------- | ----------------------------------------------------------------- |
| `request`                                                         | [GetByDecadeRequest](../../Models/Requests/GetByDecadeRequest.md) | :heavy_check_mark:                                                | The request object to use for the request.                        |

### Response

**[GetByDecadeResponse](../../Models/Requests/GetByDecadeResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetByFolder

Browse items in a library section by underlying filesystem folder.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getByFolder" method="get" path="/library/sections/{sectionId}/byFolder" -->
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

GetByFolderRequest req = new GetByFolderRequest() {
    SectionId = 352088,
};

var res = await sdk.Library.GetByFolderAsync(req);

// handle response
```

### Parameters

| Parameter                                                         | Type                                                              | Required                                                          | Description                                                       |
| ----------------------------------------------------------------- | ----------------------------------------------------------------- | ----------------------------------------------------------------- | ----------------------------------------------------------------- |
| `request`                                                         | [GetByFolderRequest](../../Models/Requests/GetByFolderRequest.md) | :heavy_check_mark:                                                | The request object to use for the request.                        |

### Response

**[GetByFolderResponse](../../Models/Requests/GetByFolderResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetByResolution

Browse items in a library section grouped by resolution.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getByResolution" method="get" path="/library/sections/{sectionId}/byResolution" -->
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

GetByResolutionRequest req = new GetByResolutionRequest() {
    SectionId = 139174,
};

var res = await sdk.Library.GetByResolutionAsync(req);

// handle response
```

### Parameters

| Parameter                                                                 | Type                                                                      | Required                                                                  | Description                                                               |
| ------------------------------------------------------------------------- | ------------------------------------------------------------------------- | ------------------------------------------------------------------------- | ------------------------------------------------------------------------- |
| `request`                                                                 | [GetByResolutionRequest](../../Models/Requests/GetByResolutionRequest.md) | :heavy_check_mark:                                                        | The request object to use for the request.                                |

### Response

**[GetByResolutionResponse](../../Models/Requests/GetByResolutionResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetByYear

Browse items in a library section grouped by year.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getByYear" method="get" path="/library/sections/{sectionId}/byYear" -->
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

GetByYearRequest req = new GetByYearRequest() {
    SectionId = 14634,
};

var res = await sdk.Library.GetByYearAsync(req);

// handle response
```

### Parameters

| Parameter                                                     | Type                                                          | Required                                                      | Description                                                   |
| ------------------------------------------------------------- | ------------------------------------------------------------- | ------------------------------------------------------------- | ------------------------------------------------------------- |
| `request`                                                     | [GetByYearRequest](../../Models/Requests/GetByYearRequest.md) | :heavy_check_mark:                                            | The request object to use for the request.                    |

### Response

**[GetByYearResponse](../../Models/Requests/GetByYearResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetSectionClips

Get clips for a library section.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getSectionClips" method="get" path="/library/sections/{sectionId}/clips" -->
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

GetSectionClipsRequest req = new GetSectionClipsRequest() {
    SectionId = 407860,
};

var res = await sdk.Library.GetSectionClipsAsync(req);

// handle response
```

### Parameters

| Parameter                                                                 | Type                                                                      | Required                                                                  | Description                                                               |
| ------------------------------------------------------------------------- | ------------------------------------------------------------------------- | ------------------------------------------------------------------------- | ------------------------------------------------------------------------- |
| `request`                                                                 | [GetSectionClipsRequest](../../Models/Requests/GetSectionClipsRequest.md) | :heavy_check_mark:                                                        | The request object to use for the request.                                |

### Response

**[GetSectionClipsResponse](../../Models/Requests/GetSectionClipsResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetCollections

Get all collections in a section

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getCollections" method="get" path="/library/sections/{sectionId}/collections" -->
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

GetCollectionsRequest req = new GetCollectionsRequest() {
    MediaQuery = new MediaQuery() {
        Type = MediaType.Episode,
        Sort = "duration:desc,index",
        SourceType = 2,
    },
    SectionId = 348838,
};

var res = await sdk.Library.GetCollectionsAsync(req);

// handle response
```

### Parameters

| Parameter                                                               | Type                                                                    | Required                                                                | Description                                                             |
| ----------------------------------------------------------------------- | ----------------------------------------------------------------------- | ----------------------------------------------------------------------- | ----------------------------------------------------------------------- |
| `request`                                                               | [GetCollectionsRequest](../../Models/Requests/GetCollectionsRequest.md) | :heavy_check_mark:                                                      | The request object to use for the request.                              |

### Response

**[GetCollectionsResponse](../../Models/Requests/GetCollectionsResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetCommon

Represents a "Common" item. It contains only the common attributes of the items selected by the provided filter
Fields which are not common will be expressed in the `mixedFields` field

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getCommon" method="get" path="/library/sections/{sectionId}/common" -->
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

GetCommonRequest req = new GetCommonRequest() {
    MediaQuery = new MediaQuery() {
        Type = MediaType.Episode,
        Sort = "duration:desc,index",
        SourceType = 2,
    },
    SectionId = 298154,
};

var res = await sdk.Library.GetCommonAsync(req);

// handle response
```

### Parameters

| Parameter                                                     | Type                                                          | Required                                                      | Description                                                   |
| ------------------------------------------------------------- | ------------------------------------------------------------- | ------------------------------------------------------------- | ------------------------------------------------------------- |
| `request`                                                     | [GetCommonRequest](../../Models/Requests/GetCommonRequest.md) | :heavy_check_mark:                                            | The request object to use for the request.                    |

### Response

**[GetCommonResponse](../../Models/Requests/GetCommonResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetSectionEdit

Get library section metadata.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getSectionEdit" method="get" path="/library/sections/{sectionId}/edit" -->
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

GetSectionEditRequest req = new GetSectionEditRequest() {
    SectionId = 223075,
};

var res = await sdk.Library.GetSectionEditAsync(req);

// handle response
```

### Parameters

| Parameter                                                               | Type                                                                    | Required                                                                | Description                                                             |
| ----------------------------------------------------------------------- | ----------------------------------------------------------------------- | ----------------------------------------------------------------------- | ----------------------------------------------------------------------- |
| `request`                                                               | [GetSectionEditRequest](../../Models/Requests/GetSectionEditRequest.md) | :heavy_check_mark:                                                      | The request object to use for the request.                              |

### Response

**[GetSectionEditResponse](../../Models/Requests/GetSectionEditResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## EditLibrarySection

Update library section metadata.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="editLibrarySection" method="put" path="/library/sections/{sectionId}/edit" -->
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

EditLibrarySectionRequest req = new EditLibrarySectionRequest() {
    SectionId = 834094,
};

var res = await sdk.Library.EditLibrarySectionAsync(req);

// handle response
```

### Parameters

| Parameter                                                                       | Type                                                                            | Required                                                                        | Description                                                                     |
| ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| `request`                                                                       | [EditLibrarySectionRequest](../../Models/Requests/EditLibrarySectionRequest.md) | :heavy_check_mark:                                                              | The request object to use for the request.                                      |

### Response

**[EditLibrarySectionResponse](../../Models/Requests/EditLibrarySectionResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## EmptyTrash

Permanently remove items from the trash for a library section.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="emptyTrash" method="get" path="/library/sections/{sectionId}/emptyTrash" -->
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

EmptyTrashRequest req = new EmptyTrashRequest() {
    SectionId = 30052,
};

var res = await sdk.Library.EmptyTrashAsync(req);

// handle response
```

### Parameters

| Parameter                                                       | Type                                                            | Required                                                        | Description                                                     |
| --------------------------------------------------------------- | --------------------------------------------------------------- | --------------------------------------------------------------- | --------------------------------------------------------------- |
| `request`                                                       | [EmptyTrashRequest](../../Models/Requests/EmptyTrashRequest.md) | :heavy_check_mark:                                              | The request object to use for the request.                      |

### Response

**[EmptyTrashResponse](../../Models/Requests/EmptyTrashResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## EmptyTrashPost

Permanently remove items from the trash for a library section.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="emptyTrashPost" method="post" path="/library/sections/{sectionId}/emptyTrash" -->
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

EmptyTrashPostRequest req = new EmptyTrashPostRequest() {
    SectionId = 537157,
};

var res = await sdk.Library.EmptyTrashPostAsync(req);

// handle response
```

### Parameters

| Parameter                                                               | Type                                                                    | Required                                                                | Description                                                             |
| ----------------------------------------------------------------------- | ----------------------------------------------------------------------- | ----------------------------------------------------------------------- | ----------------------------------------------------------------------- |
| `request`                                                               | [EmptyTrashPostRequest](../../Models/Requests/EmptyTrashPostRequest.md) | :heavy_check_mark:                                                      | The request object to use for the request.                              |

### Response

**[EmptyTrashPostResponse](../../Models/Requests/EmptyTrashPostResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## EmptyTrashPut

Empty trash in the section, permanently deleting media/metadata for missing media

### Example Usage

<!-- UsageSnippet language="csharp" operationID="emptyTrashPut" method="put" path="/library/sections/{sectionId}/emptyTrash" -->
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

EmptyTrashPutRequest req = new EmptyTrashPutRequest() {
    SectionId = 642296,
};

var res = await sdk.Library.EmptyTrashPutAsync(req);

// handle response
```

### Parameters

| Parameter                                                             | Type                                                                  | Required                                                              | Description                                                           |
| --------------------------------------------------------------------- | --------------------------------------------------------------------- | --------------------------------------------------------------------- | --------------------------------------------------------------------- |
| `request`                                                             | [EmptyTrashPutRequest](../../Models/Requests/EmptyTrashPutRequest.md) | :heavy_check_mark:                                                    | The request object to use for the request.                            |

### Response

**[EmptyTrashPutResponse](../../Models/Requests/EmptyTrashPutResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetSectionEpisodes

Get episodes for a TV library section.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getSectionEpisodes" method="get" path="/library/sections/{sectionId}/episodes" -->
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

GetSectionEpisodesRequest req = new GetSectionEpisodesRequest() {
    SectionId = 229495,
};

var res = await sdk.Library.GetSectionEpisodesAsync(req);

// handle response
```

### Parameters

| Parameter                                                                       | Type                                                                            | Required                                                                        | Description                                                                     |
| ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| `request`                                                                       | [GetSectionEpisodesRequest](../../Models/Requests/GetSectionEpisodesRequest.md) | :heavy_check_mark:                                                              | The request object to use for the request.                                      |

### Response

**[GetSectionEpisodesResponse](../../Models/Requests/GetSectionEpisodesResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetSectionFilters

Get common filters on a section

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getSectionFilters" method="get" path="/library/sections/{sectionId}/filters" -->
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

GetSectionFiltersRequest req = new GetSectionFiltersRequest() {
    SectionId = 380557,
};

var res = await sdk.Library.GetSectionFiltersAsync(req);

// handle response
```

### Parameters

| Parameter                                                                     | Type                                                                          | Required                                                                      | Description                                                                   |
| ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- |
| `request`                                                                     | [GetSectionFiltersRequest](../../Models/Requests/GetSectionFiltersRequest.md) | :heavy_check_mark:                                                            | The request object to use for the request.                                    |

### Response

**[GetSectionFiltersResponse](../../Models/Requests/GetSectionFiltersResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetFirstCharacters

Get list of first characters in this section

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getFirstCharacters" method="get" path="/library/sections/{sectionId}/firstCharacters" -->
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

GetFirstCharactersRequest req = new GetFirstCharactersRequest() {
    MediaQuery = new MediaQuery() {
        Type = MediaType.Episode,
        Sort = "duration:desc,index",
        SourceType = 2,
    },
    SectionId = 3947,
};

var res = await sdk.Library.GetFirstCharactersAsync(req);

// handle response
```

### Parameters

| Parameter                                                                       | Type                                                                            | Required                                                                        | Description                                                                     |
| ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| `request`                                                                       | [GetFirstCharactersRequest](../../Models/Requests/GetFirstCharactersRequest.md) | :heavy_check_mark:                                                              | The request object to use for the request.                                      |

### Response

**[GetFirstCharactersResponse](../../Models/Requests/GetFirstCharactersResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetLibrarySectionHubs

Get hubs for a library section.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getLibrarySectionHubs" method="get" path="/library/sections/{sectionId}/hubs" -->
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

GetLibrarySectionHubsRequest req = new GetLibrarySectionHubsRequest() {
    SectionId = 426468,
};

var res = await sdk.Library.GetLibrarySectionHubsAsync(req);

// handle response
```

### Parameters

| Parameter                                                                             | Type                                                                                  | Required                                                                              | Description                                                                           |
| ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- |
| `request`                                                                             | [GetLibrarySectionHubsRequest](../../Models/Requests/GetLibrarySectionHubsRequest.md) | :heavy_check_mark:                                                                    | The request object to use for the request.                                            |

### Response

**[GetLibrarySectionHubsResponse](../../Models/Requests/GetLibrarySectionHubsResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## DeleteIndexes

Delete all the indexes in a section

### Example Usage

<!-- UsageSnippet language="csharp" operationID="deleteIndexes" method="delete" path="/library/sections/{sectionId}/indexes" -->
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

DeleteIndexesRequest req = new DeleteIndexesRequest() {
    SectionId = 588437,
};

var res = await sdk.Library.DeleteIndexesAsync(req);

// handle response
```

### Parameters

| Parameter                                                             | Type                                                                  | Required                                                              | Description                                                           |
| --------------------------------------------------------------------- | --------------------------------------------------------------------- | --------------------------------------------------------------------- | --------------------------------------------------------------------- |
| `request`                                                             | [DeleteIndexesRequest](../../Models/Requests/DeleteIndexesRequest.md) | :heavy_check_mark:                                                    | The request object to use for the request.                            |

### Response

**[DeleteIndexesResponse](../../Models/Requests/DeleteIndexesResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## DeleteIntros

Delete all the intro markers in a section

### Example Usage

<!-- UsageSnippet language="csharp" operationID="deleteIntros" method="delete" path="/library/sections/{sectionId}/intros" -->
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

DeleteIntrosRequest req = new DeleteIntrosRequest() {
    SectionId = 498656,
};

var res = await sdk.Library.DeleteIntrosAsync(req);

// handle response
```

### Parameters

| Parameter                                                           | Type                                                                | Required                                                            | Description                                                         |
| ------------------------------------------------------------------- | ------------------------------------------------------------------- | ------------------------------------------------------------------- | ------------------------------------------------------------------- |
| `request`                                                           | [DeleteIntrosRequest](../../Models/Requests/DeleteIntrosRequest.md) | :heavy_check_mark:                                                  | The request object to use for the request.                          |

### Response

**[DeleteIntrosResponse](../../Models/Requests/DeleteIntrosResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetSectionLabels

Get labels for a library section.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getSectionLabels" method="get" path="/library/sections/{sectionId}/label" -->
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

GetSectionLabelsRequest req = new GetSectionLabelsRequest() {
    SectionId = 705342,
};

var res = await sdk.Library.GetSectionLabelsAsync(req);

// handle response
```

### Parameters

| Parameter                                                                   | Type                                                                        | Required                                                                    | Description                                                                 |
| --------------------------------------------------------------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------------------------- |
| `request`                                                                   | [GetSectionLabelsRequest](../../Models/Requests/GetSectionLabelsRequest.md) | :heavy_check_mark:                                                          | The request object to use for the request.                                  |

### Response

**[GetSectionLabelsResponse](../../Models/Requests/GetSectionLabelsResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## MatchSectionItems

Match items in a library section against metadata providers.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="matchSectionItems" method="get" path="/library/sections/{sectionId}/match" -->
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

MatchSectionItemsRequest req = new MatchSectionItemsRequest() {
    SectionId = 31032,
};

var res = await sdk.Library.MatchSectionItemsAsync(req);

// handle response
```

### Parameters

| Parameter                                                                     | Type                                                                          | Required                                                                      | Description                                                                   |
| ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- |
| `request`                                                                     | [MatchSectionItemsRequest](../../Models/Requests/MatchSectionItemsRequest.md) | :heavy_check_mark:                                                            | The request object to use for the request.                                    |

### Response

**[MatchSectionItemsResponse](../../Models/Requests/MatchSectionItemsResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## MoveSection

Move library section paths.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="moveSection" method="put" path="/library/sections/{sectionId}/move" -->
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

MoveSectionRequest req = new MoveSectionRequest() {
    SectionId = 483061,
};

var res = await sdk.Library.MoveSectionAsync(req);

// handle response
```

### Parameters

| Parameter                                                         | Type                                                              | Required                                                          | Description                                                       |
| ----------------------------------------------------------------- | ----------------------------------------------------------------- | ----------------------------------------------------------------- | ----------------------------------------------------------------- |
| `request`                                                         | [MoveSectionRequest](../../Models/Requests/MoveSectionRequest.md) | :heavy_check_mark:                                                | The request object to use for the request.                        |

### Response

**[MoveSectionResponse](../../Models/Requests/MoveSectionResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetSectionMovies

Get movies for a movie library section.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getSectionMovies" method="get" path="/library/sections/{sectionId}/movies" -->
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

GetSectionMoviesRequest req = new GetSectionMoviesRequest() {
    SectionId = 530892,
};

var res = await sdk.Library.GetSectionMoviesAsync(req);

// handle response
```

### Parameters

| Parameter                                                                   | Type                                                                        | Required                                                                    | Description                                                                 |
| --------------------------------------------------------------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------------------------- |
| `request`                                                                   | [GetSectionMoviesRequest](../../Models/Requests/GetSectionMoviesRequest.md) | :heavy_check_mark:                                                          | The request object to use for the request.                                  |

### Response

**[GetSectionMoviesResponse](../../Models/Requests/GetSectionMoviesResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetNewestForSection

Get the newest additions for a specific library section.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getNewestForSection" method="get" path="/library/sections/{sectionId}/newest" -->
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

GetNewestForSectionRequest req = new GetNewestForSectionRequest() {
    SectionId = 73900,
};

var res = await sdk.Library.GetNewestForSectionAsync(req);

// handle response
```

### Parameters

| Parameter                                                                         | Type                                                                              | Required                                                                          | Description                                                                       |
| --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- |
| `request`                                                                         | [GetNewestForSectionRequest](../../Models/Requests/GetNewestForSectionRequest.md) | :heavy_check_mark:                                                                | The request object to use for the request.                                        |

### Response

**[GetNewestForSectionResponse](../../Models/Requests/GetNewestForSectionResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetOnDeckForSection

Get the On Deck items for a specific library section.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getOnDeckForSection" method="get" path="/library/sections/{sectionId}/onDeck" -->
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

GetOnDeckForSectionRequest req = new GetOnDeckForSectionRequest() {
    SectionId = 331089,
};

var res = await sdk.Library.GetOnDeckForSectionAsync(req);

// handle response
```

### Parameters

| Parameter                                                                         | Type                                                                              | Required                                                                          | Description                                                                       |
| --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- |
| `request`                                                                         | [GetOnDeckForSectionRequest](../../Models/Requests/GetOnDeckForSectionRequest.md) | :heavy_check_mark:                                                                | The request object to use for the request.                                        |

### Response

**[GetOnDeckForSectionResponse](../../Models/Requests/GetOnDeckForSectionResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## OptimizeSection

Optimize the database for a specific library section.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="optimizeSection" method="get" path="/library/sections/{sectionId}/optimize" -->
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

OptimizeSectionRequest req = new OptimizeSectionRequest() {
    SectionId = 721290,
};

var res = await sdk.Library.OptimizeSectionAsync(req);

// handle response
```

### Parameters

| Parameter                                                                 | Type                                                                      | Required                                                                  | Description                                                               |
| ------------------------------------------------------------------------- | ------------------------------------------------------------------------- | ------------------------------------------------------------------------- | ------------------------------------------------------------------------- |
| `request`                                                                 | [OptimizeSectionRequest](../../Models/Requests/OptimizeSectionRequest.md) | :heavy_check_mark:                                                        | The request object to use for the request.                                |

### Response

**[OptimizeSectionResponse](../../Models/Requests/OptimizeSectionResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## OptimizeSectionPost

Optimize the database for a specific library section.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="optimizeSectionPost" method="post" path="/library/sections/{sectionId}/optimize" -->
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

OptimizeSectionPostRequest req = new OptimizeSectionPostRequest() {
    SectionId = 876391,
};

var res = await sdk.Library.OptimizeSectionPostAsync(req);

// handle response
```

### Parameters

| Parameter                                                                         | Type                                                                              | Required                                                                          | Description                                                                       |
| --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- |
| `request`                                                                         | [OptimizeSectionPostRequest](../../Models/Requests/OptimizeSectionPostRequest.md) | :heavy_check_mark:                                                                | The request object to use for the request.                                        |

### Response

**[OptimizeSectionPostResponse](../../Models/Requests/OptimizeSectionPostResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetSectionPhotos

Get photos for a photo library section.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getSectionPhotos" method="get" path="/library/sections/{sectionId}/photos" -->
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

GetSectionPhotosRequest req = new GetSectionPhotosRequest() {
    SectionId = 622466,
};

var res = await sdk.Library.GetSectionPhotosAsync(req);

// handle response
```

### Parameters

| Parameter                                                                   | Type                                                                        | Required                                                                    | Description                                                                 |
| --------------------------------------------------------------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------------------------- |
| `request`                                                                   | [GetSectionPhotosRequest](../../Models/Requests/GetSectionPhotosRequest.md) | :heavy_check_mark:                                                          | The request object to use for the request.                                  |

### Response

**[GetSectionPhotosResponse](../../Models/Requests/GetSectionPhotosResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetSectionPlaylists

Get playlists belonging to a library section.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getSectionPlaylists" method="get" path="/library/sections/{sectionId}/playlists" -->
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

GetSectionPlaylistsRequest req = new GetSectionPlaylistsRequest() {
    SectionId = 826184,
};

var res = await sdk.Library.GetSectionPlaylistsAsync(req);

// handle response
```

### Parameters

| Parameter                                                                         | Type                                                                              | Required                                                                          | Description                                                                       |
| --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- |
| `request`                                                                         | [GetSectionPlaylistsRequest](../../Models/Requests/GetSectionPlaylistsRequest.md) | :heavy_check_mark:                                                                | The request object to use for the request.                                        |

### Response

**[GetSectionPlaylistsResponse](../../Models/Requests/GetSectionPlaylistsResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetSectionPreferences

Get the prefs for a section by id and potentially overriding the agent

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getSectionPreferences" method="get" path="/library/sections/{sectionId}/prefs" -->
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

GetSectionPreferencesRequest req = new GetSectionPreferencesRequest() {
    SectionId = 754869,
};

var res = await sdk.Library.GetSectionPreferencesAsync(req);

// handle response
```

### Parameters

| Parameter                                                                             | Type                                                                                  | Required                                                                              | Description                                                                           |
| ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- |
| `request`                                                                             | [GetSectionPreferencesRequest](../../Models/Requests/GetSectionPreferencesRequest.md) | :heavy_check_mark:                                                                    | The request object to use for the request.                                            |

### Response

**[GetSectionPreferencesResponse](../../Models/Requests/GetSectionPreferencesResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## SetSectionPreferences

Set the prefs for a section by id

### Example Usage

<!-- UsageSnippet language="csharp" operationID="setSectionPreferences" method="put" path="/library/sections/{sectionId}/prefs" -->
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

SetSectionPreferencesRequest req = new SetSectionPreferencesRequest() {
    SectionId = 349936,
    Prefs = new SetSectionPreferencesQueryParamPrefs() {},
};

var res = await sdk.Library.SetSectionPreferencesAsync(req);

// handle response
```

### Parameters

| Parameter                                                                             | Type                                                                                  | Required                                                                              | Description                                                                           |
| ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- |
| `request`                                                                             | [SetSectionPreferencesRequest](../../Models/Requests/SetSectionPreferencesRequest.md) | :heavy_check_mark:                                                                    | The request object to use for the request.                                            |

### Response

**[SetSectionPreferencesResponse](../../Models/Requests/SetSectionPreferencesResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetRecentlyAddedForSection

Get recently added items for a specific library section.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getRecentlyAddedForSection" method="get" path="/library/sections/{sectionId}/recentlyAdded" -->
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

GetRecentlyAddedForSectionRequest req = new GetRecentlyAddedForSectionRequest() {
    SectionId = 46283,
};

var res = await sdk.Library.GetRecentlyAddedForSectionAsync(req);

// handle response
```

### Parameters

| Parameter                                                                                       | Type                                                                                            | Required                                                                                        | Description                                                                                     |
| ----------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- |
| `request`                                                                                       | [GetRecentlyAddedForSectionRequest](../../Models/Requests/GetRecentlyAddedForSectionRequest.md) | :heavy_check_mark:                                                                              | The request object to use for the request.                                                      |

### Response

**[GetRecentlyAddedForSectionResponse](../../Models/Requests/GetRecentlyAddedForSectionResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## CancelRefresh

Cancel the refresh of a section

### Example Usage

<!-- UsageSnippet language="csharp" operationID="cancelRefresh" method="delete" path="/library/sections/{sectionId}/refresh" -->
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

CancelRefreshRequest req = new CancelRefreshRequest() {
    SectionId = 326852,
};

var res = await sdk.Library.CancelRefreshAsync(req);

// handle response
```

### Parameters

| Parameter                                                             | Type                                                                  | Required                                                              | Description                                                           |
| --------------------------------------------------------------------- | --------------------------------------------------------------------- | --------------------------------------------------------------------- | --------------------------------------------------------------------- |
| `request`                                                             | [CancelRefreshRequest](../../Models/Requests/CancelRefreshRequest.md) | :heavy_check_mark:                                                    | The request object to use for the request.                            |

### Response

**[CancelRefreshResponse](../../Models/Requests/CancelRefreshResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## RefreshSection

Trigger a metadata refresh for a library section.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="refreshSection" method="get" path="/library/sections/{sectionId}/refresh" -->
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

RefreshSectionRequest req = new RefreshSectionRequest() {
    SectionId = 450300,
};

var res = await sdk.Library.RefreshSectionAsync(req);

// handle response
```

### Parameters

| Parameter                                                               | Type                                                                    | Required                                                                | Description                                                             |
| ----------------------------------------------------------------------- | ----------------------------------------------------------------------- | ----------------------------------------------------------------------- | ----------------------------------------------------------------------- |
| `request`                                                               | [RefreshSectionRequest](../../Models/Requests/RefreshSectionRequest.md) | :heavy_check_mark:                                                      | The request object to use for the request.                              |

### Response

**[RefreshSectionResponse](../../Models/Requests/RefreshSectionResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## RefreshSectionPost

Trigger a metadata refresh for a library section.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="refreshSectionPost" method="post" path="/library/sections/{sectionId}/refresh" -->
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

RefreshSectionPostRequest req = new RefreshSectionPostRequest() {
    SectionId = 848668,
    Force = BoolInt.True,
};

var res = await sdk.Library.RefreshSectionPostAsync(req);

// handle response
```

### Parameters

| Parameter                                                                       | Type                                                                            | Required                                                                        | Description                                                                     |
| ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| `request`                                                                       | [RefreshSectionPostRequest](../../Models/Requests/RefreshSectionPostRequest.md) | :heavy_check_mark:                                                              | The request object to use for the request.                                      |

### Response

**[RefreshSectionPostResponse](../../Models/Requests/RefreshSectionPostResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## SearchSection

Search within a specific library section.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="searchSection" method="get" path="/library/sections/{sectionId}/search" -->
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

SearchSectionRequest req = new SearchSectionRequest() {
    SectionId = 925380,
};

var res = await sdk.Library.SearchSectionAsync(req);

// handle response
```

### Parameters

| Parameter                                                             | Type                                                                  | Required                                                              | Description                                                           |
| --------------------------------------------------------------------- | --------------------------------------------------------------------- | --------------------------------------------------------------------- | --------------------------------------------------------------------- |
| `request`                                                             | [SearchSectionRequest](../../Models/Requests/SearchSectionRequest.md) | :heavy_check_mark:                                                    | The request object to use for the request.                            |

### Response

**[SearchSectionResponse](../../Models/Requests/SearchSectionResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetSectionSettings

Get section-specific settings.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getSectionSettings" method="get" path="/library/sections/{sectionId}/settings" -->
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

GetSectionSettingsRequest req = new GetSectionSettingsRequest() {
    SectionId = 100390,
};

var res = await sdk.Library.GetSectionSettingsAsync(req);

// handle response
```

### Parameters

| Parameter                                                                       | Type                                                                            | Required                                                                        | Description                                                                     |
| ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| `request`                                                                       | [GetSectionSettingsRequest](../../Models/Requests/GetSectionSettingsRequest.md) | :heavy_check_mark:                                                              | The request object to use for the request.                                      |

### Response

**[GetSectionSettingsResponse](../../Models/Requests/GetSectionSettingsResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetSectionShows

Get shows for a TV library section.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getSectionShows" method="get" path="/library/sections/{sectionId}/shows" -->
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

GetSectionShowsRequest req = new GetSectionShowsRequest() {
    SectionId = 9583,
};

var res = await sdk.Library.GetSectionShowsAsync(req);

// handle response
```

### Parameters

| Parameter                                                                 | Type                                                                      | Required                                                                  | Description                                                               |
| ------------------------------------------------------------------------- | ------------------------------------------------------------------------- | ------------------------------------------------------------------------- | ------------------------------------------------------------------------- |
| `request`                                                                 | [GetSectionShowsRequest](../../Models/Requests/GetSectionShowsRequest.md) | :heavy_check_mark:                                                        | The request object to use for the request.                                |

### Response

**[GetSectionShowsResponse](../../Models/Requests/GetSectionShowsResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetAvailableSorts

Get the sort mechanisms available in a section

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getAvailableSorts" method="get" path="/library/sections/{sectionId}/sorts" -->
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

GetAvailableSortsRequest req = new GetAvailableSortsRequest() {
    SectionId = 212498,
};

var res = await sdk.Library.GetAvailableSortsAsync(req);

// handle response
```

### Parameters

| Parameter                                                                     | Type                                                                          | Required                                                                      | Description                                                                   |
| ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- |
| `request`                                                                     | [GetAvailableSortsRequest](../../Models/Requests/GetAvailableSortsRequest.md) | :heavy_check_mark:                                                            | The request object to use for the request.                                    |

### Response

**[GetAvailableSortsResponse](../../Models/Requests/GetAvailableSortsResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetSectionTags

Get tags in a library section.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getSectionTags" method="get" path="/library/sections/{sectionId}/tags" -->
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

GetSectionTagsRequest req = new GetSectionTagsRequest() {
    SectionId = 787543,
};

var res = await sdk.Library.GetSectionTagsAsync(req);

// handle response
```

### Parameters

| Parameter                                                               | Type                                                                    | Required                                                                | Description                                                             |
| ----------------------------------------------------------------------- | ----------------------------------------------------------------------- | ----------------------------------------------------------------------- | ----------------------------------------------------------------------- |
| `request`                                                               | [GetSectionTagsRequest](../../Models/Requests/GetSectionTagsRequest.md) | :heavy_check_mark:                                                      | The request object to use for the request.                              |

### Response

**[GetSectionTagsResponse](../../Models/Requests/GetSectionTagsResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetSectionTimeline

Get section timeline data.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getSectionTimeline" method="get" path="/library/sections/{sectionId}/timeline" -->
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

GetSectionTimelineRequest req = new GetSectionTimelineRequest() {
    SectionId = 670370,
};

var res = await sdk.Library.GetSectionTimelineAsync(req);

// handle response
```

### Parameters

| Parameter                                                                       | Type                                                                            | Required                                                                        | Description                                                                     |
| ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| `request`                                                                       | [GetSectionTimelineRequest](../../Models/Requests/GetSectionTimelineRequest.md) | :heavy_check_mark:                                                              | The request object to use for the request.                                      |

### Response

**[GetSectionTimelineResponse](../../Models/Requests/GetSectionTimelineResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## UnmatchSectionItems

Unmatch items in a library section from metadata providers.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="unmatchSectionItems" method="get" path="/library/sections/{sectionId}/unmatch" -->
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

UnmatchSectionItemsRequest req = new UnmatchSectionItemsRequest() {
    SectionId = 209342,
};

var res = await sdk.Library.UnmatchSectionItemsAsync(req);

// handle response
```

### Parameters

| Parameter                                                                         | Type                                                                              | Required                                                                          | Description                                                                       |
| --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- |
| `request`                                                                         | [UnmatchSectionItemsRequest](../../Models/Requests/UnmatchSectionItemsRequest.md) | :heavy_check_mark:                                                                | The request object to use for the request.                                        |

### Response

**[UnmatchSectionItemsResponse](../../Models/Requests/UnmatchSectionItemsResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetUnwatchedForSection

Get unwatched items for a specific library section.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getUnwatchedForSection" method="get" path="/library/sections/{sectionId}/unwatched" -->
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

GetUnwatchedForSectionRequest req = new GetUnwatchedForSectionRequest() {
    SectionId = 483590,
};

var res = await sdk.Library.GetUnwatchedForSectionAsync(req);

// handle response
```

### Parameters

| Parameter                                                                               | Type                                                                                    | Required                                                                                | Description                                                                             |
| --------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- |
| `request`                                                                               | [GetUnwatchedForSectionRequest](../../Models/Requests/GetUnwatchedForSectionRequest.md) | :heavy_check_mark:                                                                      | The request object to use for the request.                                              |

### Response

**[GetUnwatchedForSectionResponse](../../Models/Requests/GetUnwatchedForSectionResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetStreamLevels

The the loudness of a stream in db, one entry per 100ms

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getStreamLevels" method="get" path="/library/streams/{streamId}/levels" -->
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

GetStreamLevelsRequest req = new GetStreamLevelsRequest() {
    StreamId = 447611,
};

var res = await sdk.Library.GetStreamLevelsAsync(req);

// handle response
```

### Parameters

| Parameter                                                                 | Type                                                                      | Required                                                                  | Description                                                               |
| ------------------------------------------------------------------------- | ------------------------------------------------------------------------- | ------------------------------------------------------------------------- | ------------------------------------------------------------------------- |
| `request`                                                                 | [GetStreamLevelsRequest](../../Models/Requests/GetStreamLevelsRequest.md) | :heavy_check_mark:                                                        | The request object to use for the request.                                |

### Response

**[GetStreamLevelsResponse](../../Models/Requests/GetStreamLevelsResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetStreamLoudness

The the loudness of a stream in db, one number per line, one entry per 100ms

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getStreamLoudness" method="get" path="/library/streams/{streamId}/loudness" -->
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

GetStreamLoudnessRequest req = new GetStreamLoudnessRequest() {
    StreamId = 277271,
};

var res = await sdk.Library.GetStreamLoudnessAsync(req);

// handle response
```

### Parameters

| Parameter                                                                     | Type                                                                          | Required                                                                      | Description                                                                   |
| ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- |
| `request`                                                                     | [GetStreamLoudnessRequest](../../Models/Requests/GetStreamLoudnessRequest.md) | :heavy_check_mark:                                                            | The request object to use for the request.                                    |

### Response

**[GetStreamLoudnessResponse](../../Models/Requests/GetStreamLoudnessResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetChapterImage

Get a single chapter image for a piece of media

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getChapterImage" method="get" path="/library/media/{mediaId}/chapterImages/{chapter}" -->
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

GetChapterImageRequest req = new GetChapterImageRequest() {
    MediaId = 892563,
    Chapter = 48348,
};

var res = await sdk.Library.GetChapterImageAsync(req);

// handle response
```

### Parameters

| Parameter                                                                 | Type                                                                      | Required                                                                  | Description                                                               |
| ------------------------------------------------------------------------- | ------------------------------------------------------------------------- | ------------------------------------------------------------------------- | ------------------------------------------------------------------------- |
| `request`                                                                 | [GetChapterImageRequest](../../Models/Requests/GetChapterImageRequest.md) | :heavy_check_mark:                                                        | The request object to use for the request.                                |

### Response

**[GetChapterImageResponse](../../Models/Requests/GetChapterImageResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## SetItemArtwork

Set the artwork, thumb, element for a metadata item
Generally only the admin can perform this action.  The exception is if the metadata is a playlist created by the user

### Example Usage

<!-- UsageSnippet language="csharp" operationID="setItemArtwork" method="post" path="/library/metadata/{ids}/{element}" -->
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

SetItemArtworkRequest req = new SetItemArtworkRequest() {
    Ids = "<value>",
    Element = Element.Banner,
};

var res = await sdk.Library.SetItemArtworkAsync(req);

// handle response
```

### Parameters

| Parameter                                                               | Type                                                                    | Required                                                                | Description                                                             |
| ----------------------------------------------------------------------- | ----------------------------------------------------------------------- | ----------------------------------------------------------------------- | ----------------------------------------------------------------------- |
| `request`                                                               | [SetItemArtworkRequest](../../Models/Requests/SetItemArtworkRequest.md) | :heavy_check_mark:                                                      | The request object to use for the request.                              |

### Response

**[SetItemArtworkResponse](../../Models/Requests/SetItemArtworkResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## UpdateItemArtwork

Set the artwork, thumb, element for a metadata item
Generally only the admin can perform this action.  The exception is if the metadata is a playlist created by the user

### Example Usage

<!-- UsageSnippet language="csharp" operationID="updateItemArtwork" method="put" path="/library/metadata/{ids}/{element}" -->
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

UpdateItemArtworkRequest req = new UpdateItemArtworkRequest() {
    Ids = "<value>",
    Element = PathParamElement.ClearLogo,
};

var res = await sdk.Library.UpdateItemArtworkAsync(req);

// handle response
```

### Parameters

| Parameter                                                                     | Type                                                                          | Required                                                                      | Description                                                                   |
| ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- |
| `request`                                                                     | [UpdateItemArtworkRequest](../../Models/Requests/UpdateItemArtworkRequest.md) | :heavy_check_mark:                                                            | The request object to use for the request.                                    |

### Response

**[UpdateItemArtworkResponse](../../Models/Requests/UpdateItemArtworkResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## DeleteMarker

Delete a marker for this user on the metadata item

### Example Usage

<!-- UsageSnippet language="csharp" operationID="deleteMarker" method="delete" path="/library/metadata/{ids}/marker/{marker}" -->
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

DeleteMarkerRequest req = new DeleteMarkerRequest() {
    Ids = "<value>",
    Marker = "<value>",
};

var res = await sdk.Library.DeleteMarkerAsync(req);

// handle response
```

### Parameters

| Parameter                                                           | Type                                                                | Required                                                            | Description                                                         |
| ------------------------------------------------------------------- | ------------------------------------------------------------------- | ------------------------------------------------------------------- | ------------------------------------------------------------------- |
| `request`                                                           | [DeleteMarkerRequest](../../Models/Requests/DeleteMarkerRequest.md) | :heavy_check_mark:                                                  | The request object to use for the request.                          |

### Response

**[DeleteMarkerResponse](../../Models/Requests/DeleteMarkerResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## EditMarker

Edit a marker for this user on the metadata item

### Example Usage

<!-- UsageSnippet language="csharp" operationID="editMarker" method="put" path="/library/metadata/{ids}/marker/{marker}" -->
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

EditMarkerRequest req = new EditMarkerRequest() {
    Ids = "<value>",
    Marker = "<value>",
    MediaType = 884347,
    StartTimeOffset = 517251,
    Attributes = new QueryParamAttributes() {},
};

var res = await sdk.Library.EditMarkerAsync(req);

// handle response
```

### Parameters

| Parameter                                                       | Type                                                            | Required                                                        | Description                                                     |
| --------------------------------------------------------------- | --------------------------------------------------------------- | --------------------------------------------------------------- | --------------------------------------------------------------- |
| `request`                                                       | [EditMarkerRequest](../../Models/Requests/EditMarkerRequest.md) | :heavy_check_mark:                                              | The request object to use for the request.                      |

### Response

**[EditMarkerResponse](../../Models/Requests/EditMarkerResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## DeleteMediaItem

Delete a single media from a metadata item in the library

### Example Usage

<!-- UsageSnippet language="csharp" operationID="deleteMediaItem" method="delete" path="/library/metadata/{ids}/media/{mediaItem}" -->
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

DeleteMediaItemRequest req = new DeleteMediaItemRequest() {
    Ids = "<value>",
    MediaItem = "<value>",
    Proxy = BoolInt.True,
};

var res = await sdk.Library.DeleteMediaItemAsync(req);

// handle response
```

### Parameters

| Parameter                                                                 | Type                                                                      | Required                                                                  | Description                                                               |
| ------------------------------------------------------------------------- | ------------------------------------------------------------------------- | ------------------------------------------------------------------------- | ------------------------------------------------------------------------- |
| `request`                                                                 | [DeleteMediaItemRequest](../../Models/Requests/DeleteMediaItemRequest.md) | :heavy_check_mark:                                                        | The request object to use for the request.                                |

### Response

**[DeleteMediaItemResponse](../../Models/Requests/DeleteMediaItemResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetPartIndex

Get BIF index for a part by index type

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getPartIndex" method="get" path="/library/parts/{partId}/indexes/{index}" -->
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

GetPartIndexRequest req = new GetPartIndexRequest() {
    PartId = 724750,
    Index = Index.Sd,
};

var res = await sdk.Library.GetPartIndexAsync(req);

// handle response
```

### Parameters

| Parameter                                                           | Type                                                                | Required                                                            | Description                                                         |
| ------------------------------------------------------------------- | ------------------------------------------------------------------- | ------------------------------------------------------------------- | ------------------------------------------------------------------- |
| `request`                                                           | [GetPartIndexRequest](../../Models/Requests/GetPartIndexRequest.md) | :heavy_check_mark:                                                  | The request object to use for the request.                          |

### Response

**[GetPartIndexResponse](../../Models/Requests/GetPartIndexResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## DeleteCollection

Delete a library collection from the PMS

### Example Usage

<!-- UsageSnippet language="csharp" operationID="deleteCollection" method="delete" path="/library/sections/{sectionId}/collection/{collectionId}" -->
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

DeleteCollectionRequest req = new DeleteCollectionRequest() {
    SectionId = 283619,
    CollectionId = 680895,
};

var res = await sdk.Library.DeleteCollectionAsync(req);

// handle response
```

### Parameters

| Parameter                                                                   | Type                                                                        | Required                                                                    | Description                                                                 |
| --------------------------------------------------------------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------------------------- |
| `request`                                                                   | [DeleteCollectionRequest](../../Models/Requests/DeleteCollectionRequest.md) | :heavy_check_mark:                                                          | The request object to use for the request.                                  |

### Response

**[DeleteCollectionResponse](../../Models/Requests/DeleteCollectionResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetSectionImage

Get a composite image of images in this section

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getSectionImage" method="get" path="/library/sections/{sectionId}/composite/{updatedAt}" -->
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

GetSectionImageRequest req = new GetSectionImageRequest() {
    MediaQuery = new MediaQuery() {
        Type = MediaType.Episode,
        Sort = "duration:desc,index",
        SourceType = 2,
    },
    SectionId = 925611,
    UpdatedAt = 117413,
};

var res = await sdk.Library.GetSectionImageAsync(req);

// handle response
```

### Parameters

| Parameter                                                                 | Type                                                                      | Required                                                                  | Description                                                               |
| ------------------------------------------------------------------------- | ------------------------------------------------------------------------- | ------------------------------------------------------------------------- | ------------------------------------------------------------------------- |
| `request`                                                                 | [GetSectionImageRequest](../../Models/Requests/GetSectionImageRequest.md) | :heavy_check_mark:                                                        | The request object to use for the request.                                |

### Response

**[GetSectionImageResponse](../../Models/Requests/GetSectionImageResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## DeleteStream

Delete a stream.  Only applies to downloaded subtitle streams or a sidecar subtitle when media deletion is enabled.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="deleteStream" method="delete" path="/library/streams/{streamId}.{ext}" -->
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

DeleteStreamRequest req = new DeleteStreamRequest() {
    StreamId = 841510,
    Ext = "<value>",
};

var res = await sdk.Library.DeleteStreamAsync(req);

// handle response
```

### Parameters

| Parameter                                                           | Type                                                                | Required                                                            | Description                                                         |
| ------------------------------------------------------------------- | ------------------------------------------------------------------- | ------------------------------------------------------------------- | ------------------------------------------------------------------- |
| `request`                                                           | [DeleteStreamRequest](../../Models/Requests/DeleteStreamRequest.md) | :heavy_check_mark:                                                  | The request object to use for the request.                          |

### Response

**[DeleteStreamResponse](../../Models/Requests/DeleteStreamResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetStream

Get a stream (such as a sidecar subtitle stream)

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getStream" method="get" path="/library/streams/{streamId}.{ext}" -->
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

GetStreamRequest req = new GetStreamRequest() {
    StreamId = 314506,
    Ext = "<value>",
    AutoAdjustSubtitle = BoolInt.True,
};

var res = await sdk.Library.GetStreamAsync(req);

// handle response
```

### Parameters

| Parameter                                                     | Type                                                          | Required                                                      | Description                                                   |
| ------------------------------------------------------------- | ------------------------------------------------------------- | ------------------------------------------------------------- | ------------------------------------------------------------- |
| `request`                                                     | [GetStreamRequest](../../Models/Requests/GetStreamRequest.md) | :heavy_check_mark:                                            | The request object to use for the request.                    |

### Response

**[GetStreamResponse](../../Models/Requests/GetStreamResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## SetStreamOffset

Set a stream offset in ms.  This may not be respected by all clients

### Example Usage

<!-- UsageSnippet language="csharp" operationID="setStreamOffset" method="put" path="/library/streams/{streamId}.{ext}" -->
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

SetStreamOffsetRequest req = new SetStreamOffsetRequest() {
    StreamId = 606295,
    Ext = "<value>",
};

var res = await sdk.Library.SetStreamOffsetAsync(req);

// handle response
```

### Parameters

| Parameter                                                                 | Type                                                                      | Required                                                                  | Description                                                               |
| ------------------------------------------------------------------------- | ------------------------------------------------------------------------- | ------------------------------------------------------------------------- | ------------------------------------------------------------------------- |
| `request`                                                                 | [SetStreamOffsetRequest](../../Models/Requests/SetStreamOffsetRequest.md) | :heavy_check_mark:                                                        | The request object to use for the request.                                |

### Response

**[SetStreamOffsetResponse](../../Models/Requests/SetStreamOffsetResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetItemArtwork

Get the artwork, thumb, element for a metadata item

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getItemArtwork" method="get" path="/library/metadata/{ids}/{element}/{timestamp}" -->
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

GetItemArtworkRequest req = new GetItemArtworkRequest() {
    Ids = "<value>",
    Element = GetItemArtworkPathParamElement.Poster,
    Timestamp = 999555,
};

var res = await sdk.Library.GetItemArtworkAsync(req);

// handle response
```

### Parameters

| Parameter                                                               | Type                                                                    | Required                                                                | Description                                                             |
| ----------------------------------------------------------------------- | ----------------------------------------------------------------------- | ----------------------------------------------------------------------- | ----------------------------------------------------------------------- |
| `request`                                                               | [GetItemArtworkRequest](../../Models/Requests/GetItemArtworkRequest.md) | :heavy_check_mark:                                                      | The request object to use for the request.                              |

### Response

**[GetItemArtworkResponse](../../Models/Requests/GetItemArtworkResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.Error        | 401                                              | application/json                                 |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetMediaPart

Get a media part for streaming or download.
  - streaming: This is the default scenario.  Bandwidth usage on this endpoint will be guaranteed (on the server's end) to be at least the bandwidth reservation given in the decision.  If no decision exists, an ad-hoc decision will be created if sufficient bandwidth exists.  Clients should not rely on ad-hoc decisions being made as this may be removed in the future.
  - download: Indicated if the query parameter indicates this is a download.  Bandwidth will be prioritized behind playbacks and will get a fair share of what remains.

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getMediaPart" method="get" path="/library/parts/{partId}/{changestamp}/{filename}" -->
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

GetMediaPartRequest req = new GetMediaPartRequest() {
    PartId = 877105,
    Changestamp = 970622,
    Filename = "example.file",
    Download = BoolInt.True,
};

var res = await sdk.Library.GetMediaPartAsync(req);

// handle response
```

### Parameters

| Parameter                                                           | Type                                                                | Required                                                            | Description                                                         |
| ------------------------------------------------------------------- | ------------------------------------------------------------------- | ------------------------------------------------------------------- | ------------------------------------------------------------------- |
| `request`                                                           | [GetMediaPartRequest](../../Models/Requests/GetMediaPartRequest.md) | :heavy_check_mark:                                                  | The request object to use for the request.                          |

### Response

**[GetMediaPartResponse](../../Models/Requests/GetMediaPartResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |

## GetImageFromBif

Extract an image from the BIF for a part at a particular offset

### Example Usage

<!-- UsageSnippet language="csharp" operationID="getImageFromBif" method="get" path="/library/parts/{partId}/indexes/{index}/{offset}" -->
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

GetImageFromBifRequest req = new GetImageFromBifRequest() {
    PartId = 304273,
    Index = PathParamIndex.Sd,
    Offset = 939569,
};

var res = await sdk.Library.GetImageFromBifAsync(req);

// handle response
```

### Parameters

| Parameter                                                                 | Type                                                                      | Required                                                                  | Description                                                               |
| ------------------------------------------------------------------------- | ------------------------------------------------------------------------- | ------------------------------------------------------------------------- | ------------------------------------------------------------------------- |
| `request`                                                                 | [GetImageFromBifRequest](../../Models/Requests/GetImageFromBifRequest.md) | :heavy_check_mark:                                                        | The request object to use for the request.                                |

### Response

**[GetImageFromBifResponse](../../Models/Requests/GetImageFromBifResponse.md)**

### Errors

| Error Type                                       | Status Code                                      | Content Type                                     |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| LukeHagar.PlexAPI.SDK.Models.Errors.SDKException | 4XX, 5XX                                         | \*/\*                                            |