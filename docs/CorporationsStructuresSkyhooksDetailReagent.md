# CorporationsStructuresSkyhooksDetailReagent


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**last_cycle** | **string** | Moment the \&#39;SecureStock\&#39;/\&#39;UnsecuredStock\&#39; value had its last cycle; use SDE to calculate the current values | [default to undefined]
**secured_stock** | **number** | Secured stock of the reagent at the time of \&#39;last_cycle\&#39; | [default to undefined]
**type_id** | **number** | Reagent\&#39;s type ID | [default to undefined]
**unsecured_stock** | **number** | Unsecured stock of the reagent at the time of \&#39;last_cycle\&#39; | [default to undefined]

## Example

```typescript
import { CorporationsStructuresSkyhooksDetailReagent } from 'eve-esi-client-ts';

const instance: CorporationsStructuresSkyhooksDetailReagent = {
    last_cycle,
    secured_stock,
    type_id,
    unsecured_stock,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
