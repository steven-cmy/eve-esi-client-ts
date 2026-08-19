# Status


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**players** | **number** | Number of characters currently logged in | [default to undefined]
**server_version** | **string** | Build number of the cluster | [default to undefined]
**start_time** | **string** | Moment the cluster started accepting connections | [default to undefined]
**vip** | **boolean** | Whether the cluster only accepts VIP logins | [default to undefined]

## Example

```typescript
import { Status } from 'eve-esi-client-ts';

const instance: Status = {
    players,
    server_version,
    start_time,
    vip,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
