# ProcessingState

The state of processing if this generator is part of an optimizer playlist

## Example Usage

```csharp
using LukeHagar.PlexAPI.SDK.Models.Requests;

var value = ProcessingState.Processed;
```


## Values

| Name         | Value        |
| ------------ | ------------ |
| `Processed`  | processed    |
| `Completed`  | completed    |
| `Tombstoned` | tombstoned   |
| `Disabled`   | disabled     |
| `Error`      | error        |
| `Pending`    | pending      |