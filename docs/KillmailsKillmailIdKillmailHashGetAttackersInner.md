# KillmailsKillmailIdKillmailHashGetAttackersInner

attacker object

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**alliance_id** | **number** |  | [optional] [default to undefined]
**character_id** | **number** |  | [optional] [default to undefined]
**corporation_id** | **number** |  | [optional] [default to undefined]
**damage_done** | **number** |  | [default to undefined]
**faction_id** | **number** |  | [optional] [default to undefined]
**final_blow** | **boolean** | Was the attacker the one to achieve the final blow  | [default to undefined]
**security_status** | **number** | Security status for the attacker  | [default to undefined]
**ship_type_id** | **number** | What ship was the attacker flying  | [optional] [default to undefined]
**weapon_type_id** | **number** | What weapon was used by the attacker for the kill  | [optional] [default to undefined]

## Example

```typescript
import { KillmailsKillmailIdKillmailHashGetAttackersInner } from 'eve-esi-client-ts';

const instance: KillmailsKillmailIdKillmailHashGetAttackersInner = {
    alliance_id,
    character_id,
    corporation_id,
    damage_done,
    faction_id,
    final_blow,
    security_status,
    ship_type_id,
    weapon_type_id,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
