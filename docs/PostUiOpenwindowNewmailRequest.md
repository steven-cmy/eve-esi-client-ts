# PostUiOpenwindowNewmailRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**body** | **string** |  | [default to undefined]
**recipients** | **Array&lt;number&gt;** |  | [default to undefined]
**subject** | **string** |  | [default to undefined]
**to_corp_or_alliance_id** | **number** |  | [optional] [default to undefined]
**to_mailing_list_id** | **number** | Corporations, alliances and mailing lists are all types of mailing groups. You may only send to one mailing group, at a time, so you may fill out either this field or the to_corp_or_alliance_ids field | [optional] [default to undefined]

## Example

```typescript
import { PostUiOpenwindowNewmailRequest } from 'eve-esi-client-ts';

const instance: PostUiOpenwindowNewmailRequest = {
    body,
    recipients,
    subject,
    to_corp_or_alliance_id,
    to_mailing_list_id,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
