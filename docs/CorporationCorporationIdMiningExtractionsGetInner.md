# CorporationCorporationIdMiningExtractionsGetInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**chunk_arrival_time** | **string** | The time at which the chunk being extracted will arrive and can be fractured by the moon mining drill.  | [default to undefined]
**extraction_start_time** | **string** | The time at which the current extraction was initiated.  | [default to undefined]
**moon_id** | **number** |  | [default to undefined]
**natural_decay_time** | **string** | The time at which the chunk being extracted will naturally fracture if it is not first fractured by the moon mining drill.  | [default to undefined]
**structure_id** | **number** |  | [default to undefined]

## Example

```typescript
import { CorporationCorporationIdMiningExtractionsGetInner } from 'eve-esi-client-ts';

const instance: CorporationCorporationIdMiningExtractionsGetInner = {
    chunk_arrival_time,
    extraction_start_time,
    moon_id,
    natural_decay_time,
    structure_id,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
