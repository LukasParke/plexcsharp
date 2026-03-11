# DefaultSubtitleAccessibility

The subtitles for the deaf or hard-of-hearing (SDH) searches mode (0 = Prefer non-SDH subtitles, 1 = Prefer SDH subtitles, 2 = Only show SDH subtitles, 3 = Only show non-SDH subtitles)

## Example Usage

```csharp
using LukeHagar.PlexAPI.SDK.Models.Components;

var value = DefaultSubtitleAccessibility.PreferNonSdh;
```


## Values

| Name           | Value          |
| -------------- | -------------- |
| `PreferNonSdh` | 0              |
| `PreferSdh`    | 1              |
| `OnlySdh`      | 2              |
| `OnlyNonSdh`   | 3              |