# FreelanceJobsDetailAccessandvisibility


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**acl_protected** | **boolean** | Whether the job is protected by an ACL | [default to undefined]
**broadcast_locations** | [**Array&lt;FreelanceJobsDetailBroadcastlocations&gt;**](FreelanceJobsDetailBroadcastlocations.md) | Solar systems where the job is broadcast | [optional] [default to undefined]
**restrictions** | [**FreelanceJobsDetailRestrictions**](FreelanceJobsDetailRestrictions.md) | Restrictions on who can participate | [optional] [default to undefined]

## Example

```typescript
import { FreelanceJobsDetailAccessandvisibility } from 'eve-esi-client-ts';

const instance: FreelanceJobsDetailAccessandvisibility = {
    acl_protected,
    broadcast_locations,
    restrictions,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
