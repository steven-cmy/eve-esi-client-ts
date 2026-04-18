# FreelanceJobsDetailConfigurationParametersValue


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**matcher** | [**FreelanceJobsDetailParametermatcher**](FreelanceJobsDetailParametermatcher.md) | Parameter that matches a type | [optional] [default to undefined]
**_options** | [**FreelanceJobsDetailParameteroptions**](FreelanceJobsDetailParameteroptions.md) | Parameter that has one or more selected values | [optional] [default to undefined]
**_boolean** | [**FreelanceJobsDetailParameterboolean**](FreelanceJobsDetailParameterboolean.md) | Parameter that can be toggled | [optional] [default to undefined]
**corporation_item_delivery** | [**FreelanceJobsDetailParametercorporationitemdelivery**](FreelanceJobsDetailParametercorporationitemdelivery.md) | Parameter for delivering items to a corporation | [optional] [default to undefined]

## Example

```typescript
import { FreelanceJobsDetailConfigurationParametersValue } from 'eve-esi-client-ts';

const instance: FreelanceJobsDetailConfigurationParametersValue = {
    matcher,
    _options,
    _boolean,
    corporation_item_delivery,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
