# CorporationsProjectsDetail


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**configuration** | [**CorporationsProjectsDetailConfiguration**](CorporationsProjectsDetailConfiguration.md) |  | [default to undefined]
**contribution** | [**CorporationsProjectsDetailContribution**](CorporationsProjectsDetailContribution.md) | Project\&#39;s contribution settings | [optional] [default to undefined]
**creator** | [**CorporationsProjectsDetailCreator**](CorporationsProjectsDetailCreator.md) | Project\&#39;s creator | [default to undefined]
**details** | [**CorporationsProjectsDetailDetails**](CorporationsProjectsDetailDetails.md) | Project\&#39;s details | [default to undefined]
**id** | **string** | Project\&#39;s ID | [default to undefined]
**last_modified** | **string** | Moment this project was last modified. Project contributions also count as a modification | [default to undefined]
**name** | **string** | Project\&#39;s name | [default to undefined]
**progress** | [**CorporationsProjectsDetailProgress**](CorporationsProjectsDetailProgress.md) | Project\&#39;s progress | [default to undefined]
**reward** | [**CorporationsProjectsDetailReward**](CorporationsProjectsDetailReward.md) | Project\&#39;s reward | [optional] [default to undefined]
**state** | **string** | Project\&#39;s current state | [default to undefined]

## Example

```typescript
import { CorporationsProjectsDetail } from 'eve-esi-client-ts';

const instance: CorporationsProjectsDetail = {
    configuration,
    contribution,
    creator,
    details,
    id,
    last_modified,
    name,
    progress,
    reward,
    state,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
