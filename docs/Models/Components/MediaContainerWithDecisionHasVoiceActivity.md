# MediaContainerWithDecisionHasVoiceActivity

Voice activity detection availability flag returned by PMS.
PMS returns this as string values (`"0"` or `"1"`) instead of a JSON boolean.


## Example Usage

```csharp
using LukeHagar.PlexAPI.SDK.Models.Components;

var value = MediaContainerWithDecisionHasVoiceActivity.Zero;
```


## Values

| Name   | Value  |
| ------ | ------ |
| `Zero` | 0      |
| `One`  | 1      |