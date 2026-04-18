# CorporationsCorporationIdRolesHistoryGetInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**changed_at** | **string** |  | [default to undefined]
**character_id** | **number** | The character whose roles are changed | [default to undefined]
**issuer_id** | **number** | ID of the character who issued this change | [default to undefined]
**new_roles** | **Set&lt;string&gt;** |  | [default to undefined]
**old_roles** | **Set&lt;string&gt;** |  | [default to undefined]
**role_type** | **string** |  | [default to undefined]

## Example

```typescript
import { CorporationsCorporationIdRolesHistoryGetInner } from 'eve-esi-client-ts';

const instance: CorporationsCorporationIdRolesHistoryGetInner = {
    changed_at,
    character_id,
    issuer_id,
    new_roles,
    old_roles,
    role_type,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
