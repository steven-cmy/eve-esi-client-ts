# UniverseStructuresStructureIdGet


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **string** | The full name of the structure | [default to undefined]
**owner_id** | **number** | The ID of the corporation who owns this particular structure | [default to undefined]
**position** | [**UniverseStructuresStructureIdGetPosition**](UniverseStructuresStructureIdGetPosition.md) |  | [optional] [default to undefined]
**solar_system_id** | **number** |  | [default to undefined]
**type_id** | **number** |  | [optional] [default to undefined]

## Example

```typescript
import { UniverseStructuresStructureIdGet } from 'eve-esi-client-ts';

const instance: UniverseStructuresStructureIdGet = {
    name,
    owner_id,
    position,
    solar_system_id,
    type_id,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
