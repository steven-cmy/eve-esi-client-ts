# CharactersCharacterIdAttributesGet


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**accrued_remap_cooldown_date** | **string** | Neural remapping cooldown after a character uses remap accrued over time | [optional] [default to undefined]
**bonus_remaps** | **number** | Number of available bonus character neural remaps | [optional] [default to undefined]
**charisma** | **number** |  | [default to undefined]
**intelligence** | **number** |  | [default to undefined]
**last_remap_date** | **string** | Datetime of last neural remap, including usage of bonus remaps | [optional] [default to undefined]
**memory** | **number** |  | [default to undefined]
**perception** | **number** |  | [default to undefined]
**willpower** | **number** |  | [default to undefined]

## Example

```typescript
import { CharactersCharacterIdAttributesGet } from 'eve-esi-client-ts';

const instance: CharactersCharacterIdAttributesGet = {
    accrued_remap_cooldown_date,
    bonus_remaps,
    charisma,
    intelligence,
    last_remap_date,
    memory,
    perception,
    willpower,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
