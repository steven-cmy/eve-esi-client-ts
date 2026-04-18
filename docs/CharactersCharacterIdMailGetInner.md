# CharactersCharacterIdMailGetInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**from** | **number** | From whom the mail was sent | [optional] [default to undefined]
**is_read** | **boolean** |  | [optional] [default to undefined]
**labels** | **Set&lt;number&gt;** |  | [optional] [default to undefined]
**mail_id** | **number** |  | [optional] [default to undefined]
**recipients** | [**Set&lt;PostCharactersCharacterIdMailRequestRecipientsInner&gt;**](PostCharactersCharacterIdMailRequestRecipientsInner.md) | Recipients of the mail | [optional] [default to undefined]
**subject** | **string** | Mail subject | [optional] [default to undefined]
**timestamp** | **string** | When the mail was sent | [optional] [default to undefined]

## Example

```typescript
import { CharactersCharacterIdMailGetInner } from 'eve-esi-client-ts';

const instance: CharactersCharacterIdMailGetInner = {
    from,
    is_read,
    labels,
    mail_id,
    recipients,
    subject,
    timestamp,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
