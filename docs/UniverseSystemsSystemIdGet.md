# UniverseSystemsSystemIdGet


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**constellation_id** | **number** | The constellation this solar system is in | [default to undefined]
**name** | **string** |  | [default to undefined]
**planets** | [**Array&lt;UniverseSystemsSystemIdGetPlanetsInner&gt;**](UniverseSystemsSystemIdGetPlanetsInner.md) |  | [optional] [default to undefined]
**position** | [**CharactersCharacterIdAssetsLocationsPostInnerPosition**](CharactersCharacterIdAssetsLocationsPostInnerPosition.md) |  | [default to undefined]
**security_class** | **string** |  | [optional] [default to undefined]
**security_status** | **number** |  | [default to undefined]
**star_id** | **number** |  | [optional] [default to undefined]
**stargates** | **Array&lt;number&gt;** |  | [optional] [default to undefined]
**stations** | **Array&lt;number&gt;** |  | [optional] [default to undefined]
**system_id** | **number** |  | [default to undefined]

## Example

```typescript
import { UniverseSystemsSystemIdGet } from 'eve-esi-client-ts';

const instance: UniverseSystemsSystemIdGet = {
    constellation_id,
    name,
    planets,
    position,
    security_class,
    security_status,
    star_id,
    stargates,
    stations,
    system_id,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
