# KillmailsKillmailIdKillmailHashGetVictim


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**alliance_id** | **number** |  | [optional] [default to undefined]
**character_id** | **number** |  | [optional] [default to undefined]
**corporation_id** | **number** |  | [optional] [default to undefined]
**damage_taken** | **number** | How much total damage was taken by the victim  | [default to undefined]
**faction_id** | **number** |  | [optional] [default to undefined]
**items** | [**Array&lt;KillmailsKillmailIdKillmailHashGetVictimItemsInner&gt;**](KillmailsKillmailIdKillmailHashGetVictimItemsInner.md) |  | [optional] [default to undefined]
**position** | [**KillmailsKillmailIdKillmailHashGetVictimPosition**](KillmailsKillmailIdKillmailHashGetVictimPosition.md) |  | [optional] [default to undefined]
**ship_type_id** | **number** | The ship that the victim was piloting and was destroyed  | [default to undefined]

## Example

```typescript
import { KillmailsKillmailIdKillmailHashGetVictim } from 'eve-esi-client-ts';

const instance: KillmailsKillmailIdKillmailHashGetVictim = {
    alliance_id,
    character_id,
    corporation_id,
    damage_taken,
    faction_id,
    items,
    position,
    ship_type_id,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
