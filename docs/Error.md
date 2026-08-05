# ModelError


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**details** | [**Array&lt;ErrorDetail&gt;**](ErrorDetail.md) | List of individual issues. | [optional] [default to undefined]
**error** | **string** | Error message. | [default to undefined]
**status** | **number** | HTTP status code. | [optional] [default to undefined]

## Example

```typescript
import { ModelError } from 'eve-esi-client-ts';

const instance: ModelError = {
    details,
    error,
    status,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
