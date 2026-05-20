# SovereigntySystemsSolarsystemClaim

Claim on this solar system

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**faction** | [**SovereigntySystemsFaction**](SovereigntySystemsFaction.md) | Solar system is claimed by a faction | [optional] [default to undefined]
**alliance** | [**SovereigntySystemsAlliance**](SovereigntySystemsAlliance.md) | Solar system is claimed by an alliance | [optional] [default to undefined]
**unclaimed** | **boolean** | Solar system is unclaimed | [optional] [default to undefined]

## Example

```typescript
import { SovereigntySystemsSolarsystemClaim } from 'eve-esi-client-ts';

const instance: SovereigntySystemsSolarsystemClaim = {
    faction,
    alliance,
    unclaimed,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
