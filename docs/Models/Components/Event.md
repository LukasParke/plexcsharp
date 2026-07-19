# Event

Event type that triggered the webhook.

## Example Usage

```csharp
using LukeHagar.PlexAPI.SDK.Models.Components;

var value = Event.MediaPlay;
```


## Values

| Name            | Value           |
| --------------- | --------------- |
| `MediaPlay`     | media.play      |
| `MediaPause`    | media.pause     |
| `MediaResume`   | media.resume    |
| `MediaStop`     | media.stop      |
| `MediaScrobble` | media.scrobble  |
| `MediaRate`     | media.rate      |
| `LibraryNew`    | library.new     |
| `LibraryOnDeck` | library.on.deck |