# FreelanceJobsDetailDetails


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**career** | **string** | Assigned career path | [default to undefined]
**created** | **string** | Moment this freelance job was created | [default to undefined]
**creator** | [**FreelanceJobsDetailCreator**](FreelanceJobsDetailCreator.md) | Creator | [default to undefined]
**description** | **string** | Description | [default to undefined]
**expires** | **string** | Moment this freelance job expires | [optional] [default to undefined]
**finished** | **string** | Moment this freelance job transitioned to a non-active state | [optional] [default to undefined]

## Example

```typescript
import { FreelanceJobsDetailDetails } from 'eve-esi-client-ts';

const instance: FreelanceJobsDetailDetails = {
    career,
    created,
    creator,
    description,
    expires,
    finished,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
