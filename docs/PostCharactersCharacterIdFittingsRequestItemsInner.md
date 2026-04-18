# PostCharactersCharacterIdFittingsRequestItemsInner

item object

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**flag** | **string** | Fitting location for the item. Entries placed in \&#39;Invalid\&#39; will be discarded. If this leaves the fitting with nothing, it will cause an error. | [default to undefined]
**quantity** | **number** |  | [default to undefined]
**type_id** | **number** |  | [default to undefined]

## Example

```typescript
import { PostCharactersCharacterIdFittingsRequestItemsInner } from 'eve-esi-client-ts';

const instance: PostCharactersCharacterIdFittingsRequestItemsInner = {
    flag,
    quantity,
    type_id,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
