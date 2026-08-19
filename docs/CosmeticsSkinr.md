# CosmeticsSkinr


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**creator_id** | **number** | SKINR creator character ID | [default to undefined]
**id** | **string** | SKINR ID | [default to undefined]
**layout** | [**CosmeticsSkinrLayout**](CosmeticsSkinrLayout.md) | SKINR layout | [default to undefined]
**line** | **string** | SKINR line name | [optional] [default to undefined]
**name** | **string** | SKINR name | [default to undefined]
**ship_type_id** | **number** | ID of the ship hull | [default to undefined]
**tier** | [**CosmeticsSkinrTier**](CosmeticsSkinrTier.md) | SKINR tier | [default to undefined]

## Example

```typescript
import { CosmeticsSkinr } from 'eve-esi-client-ts';

const instance: CosmeticsSkinr = {
    creator_id,
    id,
    layout,
    line,
    name,
    ship_type_id,
    tier,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
