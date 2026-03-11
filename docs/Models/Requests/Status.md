# Status

## Example Usage

```csharp
using LukeHagar.PlexAPI.SDK.Models.Requests;

var value = Status.Online;

// Open enum: use .Of() to create instances from custom string values
var custom = Status.Of("custom_value");
```


## Values

| Name      | Value     |
| --------- | --------- |
| `Online`  | online    |
| `Offline` | offline   |