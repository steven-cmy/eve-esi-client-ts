# CorporationsStructuresSkyhooksDetail


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**effective_workforce** | **number** | Skyhook\&#39;s effective workforce; this can differ from the Skyhook\&#39;s normal workforce due to the influence of an attached Mercenary Den | [optional] [default to undefined]
**id** | **number** | Skyhook\&#39;s ID | [default to undefined]
**is_active** | **boolean** | Whether the Skyhook is active and producing workforce/power/reagents | [default to undefined]
**planet_id** | **number** | ID of the planet the Skyhook is anchored on | [default to undefined]
**reagents** | [**Array&lt;CorporationsStructuresSkyhooksDetailReagent&gt;**](CorporationsStructuresSkyhooksDetailReagent.md) | Skyhook\&#39;s reagents | [optional] [default to undefined]
**reinforcement_timer** | [**CorporationsStructuresSkyhooksDetailReinforcementtimer**](CorporationsStructuresSkyhooksDetailReinforcementtimer.md) | Skyhook\&#39;s reinforcement timer (if the structure is reinforced) | [optional] [default to undefined]
**state** | **string** | Skyhook\&#39;s state | [default to undefined]
**theft_vulnerability** | [**CorporationsStructuresSkyhooksDetailTheftvulnerability**](CorporationsStructuresSkyhooksDetailTheftvulnerability.md) | Skyhook\&#39;s theft vulnerability | [optional] [default to undefined]

## Example

```typescript
import { CorporationsStructuresSkyhooksDetail } from 'eve-esi-client-ts';

const instance: CorporationsStructuresSkyhooksDetail = {
    effective_workforce,
    id,
    is_active,
    planet_id,
    reagents,
    reinforcement_timer,
    state,
    theft_vulnerability,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
