# SovereigntySystemsAlliance


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**alliance_id** | **number** | Alliance that claimed this solar system | [default to undefined]
**claimed_since** | **string** | Time the claim was made | [default to undefined]
**corporation_id** | **number** | Corporation that claimed this solar system | [default to undefined]
**development** | [**SovereigntySystemsDevelopment**](SovereigntySystemsDevelopment.md) | Solar system\&#39;s development | [default to undefined]
**is_capital_system** | **boolean** | Whether the system is the capital system of the alliance | [default to undefined]
**sovereignty_hub** | [**SovereigntySystemsSovereigntyhub**](SovereigntySystemsSovereigntyhub.md) | Sovereignty Hub holding the claim | [default to undefined]

## Example

```typescript
import { SovereigntySystemsAlliance } from 'eve-esi-client-ts';

const instance: SovereigntySystemsAlliance = {
    alliance_id,
    claimed_since,
    corporation_id,
    development,
    is_capital_system,
    sovereignty_hub,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
