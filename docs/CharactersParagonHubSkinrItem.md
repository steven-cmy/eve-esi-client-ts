# CharactersParagonHubSkinrItem


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**created** | **string** | When the listing was created | [default to undefined]
**expires** | **string** | When the listing expires | [default to undefined]
**id** | **string** | Unique identifier of the listing | [default to undefined]
**last_modified** | **string** | When this listing was last retrieved from the game | [default to undefined]
**price** | [**CharactersParagonHubSkinrItemPrice**](CharactersParagonHubSkinrItemPrice.md) |  | [default to undefined]
**quantity** | **number** | How many licenses remain in this listing | [default to undefined]
**seller_id** | **number** | Character that posted the listing | [default to undefined]
**skinr_id** | **string** | SKINR license identifier | [default to undefined]
**state** | **string** | Lifecycle state of the listing | [default to undefined]
**target** | [**CharactersParagonHubSkinrItemTarget**](CharactersParagonHubSkinrItemTarget.md) |  | [default to undefined]

## Example

```typescript
import { CharactersParagonHubSkinrItem } from 'eve-esi-client-ts';

const instance: CharactersParagonHubSkinrItem = {
    created,
    expires,
    id,
    last_modified,
    price,
    quantity,
    seller_id,
    skinr_id,
    state,
    target,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
