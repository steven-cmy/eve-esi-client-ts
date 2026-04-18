# CharactersSkillqueueSkill


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**finish_date** | **string** | The date the skill training will finish | [optional] [default to undefined]
**finished_level** | **number** | The level the skill is training for | [default to undefined]
**level_end_sp** | **number** | The Skill Points at the end of the level | [optional] [default to undefined]
**level_start_sp** | **number** | The Skill Points at the start of the level | [optional] [default to undefined]
**queue_position** | **number** | The position of the skill in the queue | [default to undefined]
**skill_id** | **number** | The TypeID of the skill | [default to undefined]
**start_date** | **string** | The date the skill training will start/continue | [optional] [default to undefined]
**training_start_sp** | **number** | The Skill Points at the start of training | [optional] [default to undefined]

## Example

```typescript
import { CharactersSkillqueueSkill } from 'eve-esi-client-ts';

const instance: CharactersSkillqueueSkill = {
    finish_date,
    finished_level,
    level_end_sp,
    level_start_sp,
    queue_position,
    skill_id,
    start_date,
    training_start_sp,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
