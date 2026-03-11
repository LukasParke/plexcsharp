# ProcessingStateContext

The error which could have occurred (or `good`)

## Example Usage

```csharp
using LukeHagar.PlexAPI.SDK.Models.Requests;

var value = ProcessingStateContext.Good;
```


## Values

| Name                      | Value                     |
| ------------------------- | ------------------------- |
| `Good`                    | good                      |
| `SourceFileUnavailable`   | sourceFileUnavailable     |
| `SourceFileMetadataError` | sourceFileMetadataError   |
| `ClientProfileError`      | clientProfileError        |
| `IoError`                 | ioError                   |
| `TranscoderError`         | transcoderError           |
| `UnknownError`            | unknownError              |
| `MediaAnalysisError`      | mediaAnalysisError        |
| `DownloadFailed`          | downloadFailed            |
| `AccessDenied`            | accessDenied              |
| `CannotTranscode`         | cannotTranscode           |
| `CodecInstallError`       | codecInstallError         |