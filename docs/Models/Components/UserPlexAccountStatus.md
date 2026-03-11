# UserPlexAccountStatus

## Example Usage

```csharp
using LukeHagar.PlexAPI.SDK.Models.Components;

var value = UserPlexAccountStatus.Online;

// Open enum: use .Of() to create instances from custom string values
var custom = UserPlexAccountStatus.Of("custom_value");
```


## Values

| Name      | Value     |
| --------- | --------- |
| `Online`  | online    |
| `Offline` | offline   |