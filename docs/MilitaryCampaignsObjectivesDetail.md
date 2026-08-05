# MilitaryCampaignsObjectivesDetail


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**finished** | **string** | Moment the objective transitioned to a non-active state | [optional] [default to undefined]
**id** | **string** | Objective\&#39;s ID | [default to undefined]
**last_modified** | **string** | Objective\&#39;s last modified | [default to undefined]
**participants** | [**MilitaryCampaignsObjectivesDetailParticipants**](MilitaryCampaignsObjectivesDetailParticipants.md) | Objective\&#39;s participants | [default to undefined]
**progress** | **number** | Objective\&#39;s progress | [default to undefined]
**started** | **string** | Moment the objective started | [optional] [default to undefined]
**state** | **string** | Objective\&#39;s state | [default to undefined]

## Example

```typescript
import { MilitaryCampaignsObjectivesDetail } from 'eve-esi-client-ts';

const instance: MilitaryCampaignsObjectivesDetail = {
    finished,
    id,
    last_modified,
    participants,
    progress,
    started,
    state,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
