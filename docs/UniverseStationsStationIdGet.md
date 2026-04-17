# UniverseStationsStationIdGet


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**max_dockable_ship_volume** | **number** |  | [default to undefined]
**name** | **string** |  | [default to undefined]
**office_rental_cost** | **number** |  | [default to undefined]
**owner** | **number** | ID of the corporation that controls this station | [optional] [default to undefined]
**position** | [**CharactersCharacterIdAssetsLocationsPostInnerPosition**](CharactersCharacterIdAssetsLocationsPostInnerPosition.md) |  | [default to undefined]
**race_id** | **number** |  | [optional] [default to undefined]
**reprocessing_efficiency** | **number** |  | [default to undefined]
**reprocessing_stations_take** | **number** |  | [default to undefined]
**services** | **Array&lt;string&gt;** |  | [default to undefined]
**station_id** | **number** |  | [default to undefined]
**system_id** | **number** | The solar system this station is in | [default to undefined]
**type_id** | **number** |  | [default to undefined]

## Example

```typescript
import { UniverseStationsStationIdGet } from 'eve-esi-client-ts';

const instance: UniverseStationsStationIdGet = {
    max_dockable_ship_volume,
    name,
    office_rental_cost,
    owner,
    position,
    race_id,
    reprocessing_efficiency,
    reprocessing_stations_take,
    services,
    station_id,
    system_id,
    type_id,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
