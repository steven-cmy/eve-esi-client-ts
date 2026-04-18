# CharactersCharacterIdContactsGetInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**contact_id** | **number** |  | [default to undefined]
**contact_type** | **string** |  | [default to undefined]
**is_blocked** | **boolean** | Whether this contact is in the blocked list. Note a missing value denotes unknown, not true or false | [optional] [default to undefined]
**is_watched** | **boolean** | Whether this contact is being watched | [optional] [default to undefined]
**label_ids** | **Array&lt;number&gt;** |  | [optional] [default to undefined]
**standing** | **number** | Standing of the contact | [default to undefined]

## Example

```typescript
import { CharactersCharacterIdContactsGetInner } from 'eve-esi-client-ts';

const instance: CharactersCharacterIdContactsGetInner = {
    contact_id,
    contact_type,
    is_blocked,
    is_watched,
    label_ids,
    standing,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
