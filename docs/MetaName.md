# MetaName


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**current** | **string** | The name ESI is going by today. It was almost certainly something else last time you looked. | [default to undefined]
**history** | [**Array&lt;MetaNameEntry&gt;**](MetaNameEntry.md) | Every name ESI has ever gone by, newest first. It has never once been the same twice. | [default to undefined]

## Example

```typescript
import { MetaName } from 'eve-esi-client-ts';

const instance: MetaName = {
    current,
    history,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
