# KillmailsKillmailIdKillmailHashGetVictimItemsInner

item object

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**flag** | **number** | Flag for the location of the item  | [default to undefined]
**item_type_id** | **number** |  | [default to undefined]
**items** | [**Array&lt;KillmailsKillmailIdKillmailHashGetVictimItemsInnerItemsInner&gt;**](KillmailsKillmailIdKillmailHashGetVictimItemsInnerItemsInner.md) |  | [optional] [default to undefined]
**quantity_destroyed** | **number** | How many of the item were destroyed if any  | [optional] [default to undefined]
**quantity_dropped** | **number** | How many of the item were dropped if any  | [optional] [default to undefined]
**singleton** | **number** |  | [default to undefined]

## Example

```typescript
import { KillmailsKillmailIdKillmailHashGetVictimItemsInner } from 'eve-esi-client-ts';

const instance: KillmailsKillmailIdKillmailHashGetVictimItemsInner = {
    flag,
    item_type_id,
    items,
    quantity_destroyed,
    quantity_dropped,
    singleton,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
