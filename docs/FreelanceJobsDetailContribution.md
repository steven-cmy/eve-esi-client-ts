# FreelanceJobsDetailContribution


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**contribution_per_participant_limit** | **number** | Limit on the contribution of the individual participant | [optional] [default to undefined]
**max_committed_participants** | **number** | Maximum number of participants that can commit to this job | [default to undefined]
**reward_per_contribution** | **number** | ISK reward per contribution | [optional] [default to undefined]
**submission_limit** | **number** | Limit on amount of contribution per submission | [optional] [default to undefined]
**submission_multiplier** | **number** | Multiplier towards progress per contribution | [optional] [default to undefined]

## Example

```typescript
import { FreelanceJobsDetailContribution } from 'eve-esi-client-ts';

const instance: FreelanceJobsDetailContribution = {
    contribution_per_participant_limit,
    max_committed_participants,
    reward_per_contribution,
    submission_limit,
    submission_multiplier,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
