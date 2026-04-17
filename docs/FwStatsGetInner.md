# FwStatsGetInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**faction_id** | **number** |  | [default to undefined]
**kills** | [**FwStatsGetInnerKills**](FwStatsGetInnerKills.md) |  | [default to undefined]
**pilots** | **number** | How many pilots fight for the given faction | [default to undefined]
**systems_controlled** | **number** | The number of solar systems controlled by the given faction | [default to undefined]
**victory_points** | [**FwStatsGetInnerVictoryPoints**](FwStatsGetInnerVictoryPoints.md) |  | [default to undefined]

## Example

```typescript
import { FwStatsGetInner } from 'eve-esi-client-ts';

const instance: FwStatsGetInner = {
    faction_id,
    kills,
    pilots,
    systems_controlled,
    victory_points,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
