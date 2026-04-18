# DogmaDynamicItemsTypeIdItemIdGet


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**created_by** | **number** | The ID of the character who created the item | [default to undefined]
**dogma_attributes** | [**Array&lt;DogmaDynamicItemsTypeIdItemIdGetDogmaAttributesInner&gt;**](DogmaDynamicItemsTypeIdItemIdGetDogmaAttributesInner.md) |  | [default to undefined]
**dogma_effects** | [**Array&lt;DogmaDynamicItemsTypeIdItemIdGetDogmaEffectsInner&gt;**](DogmaDynamicItemsTypeIdItemIdGetDogmaEffectsInner.md) |  | [default to undefined]
**mutator_type_id** | **number** | The type ID of the mutator used to generate the dynamic item. | [default to undefined]
**source_type_id** | **number** | The type ID of the source item the mutator was applied to create the dynamic item. | [default to undefined]

## Example

```typescript
import { DogmaDynamicItemsTypeIdItemIdGet } from 'eve-esi-client-ts';

const instance: DogmaDynamicItemsTypeIdItemIdGet = {
    created_by,
    dogma_attributes,
    dogma_effects,
    mutator_type_id,
    source_type_id,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
