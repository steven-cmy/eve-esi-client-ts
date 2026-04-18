# RouteRequestBody


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**avoid_systems** | **Set&lt;number&gt;** | Systems to avoid | [optional] [default to undefined]
**connections** | [**Array&lt;RouteConnection&gt;**](RouteConnection.md) | Additional one-way connections (like Jump Bridges) between systems | [optional] [default to undefined]
**preference** | **string** | Preference for the route | [optional] [default to PreferenceEnum_Shorter]
**security_penalty** | **number** | Strictness of the path preference | [optional] [default to 50]

## Example

```typescript
import { RouteRequestBody } from 'eve-esi-client-ts';

const instance: RouteRequestBody = {
    avoid_systems,
    connections,
    preference,
    security_penalty,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
