# FwLeaderboardsCharactersGetVictoryPoints

Top 100 rankings of pilots by victory points from yesterday, last week and in total

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**active_total** | [**Array&lt;FwLeaderboardsCharactersGetVictoryPointsActiveTotalInner&gt;**](FwLeaderboardsCharactersGetVictoryPointsActiveTotalInner.md) | Top 100 ranking of pilots active in faction warfare by total victory points. A pilot is considered \&quot;active\&quot; if they have participated in faction warfare in the past 14 days | [default to undefined]
**last_week** | [**Array&lt;FwLeaderboardsCharactersGetVictoryPointsLastWeekInner&gt;**](FwLeaderboardsCharactersGetVictoryPointsLastWeekInner.md) | Top 100 ranking of pilots by victory points in the past week | [default to undefined]
**yesterday** | [**Array&lt;FwLeaderboardsCharactersGetVictoryPointsYesterdayInner&gt;**](FwLeaderboardsCharactersGetVictoryPointsYesterdayInner.md) | Top 100 ranking of pilots by victory points in the past day | [default to undefined]

## Example

```typescript
import { FwLeaderboardsCharactersGetVictoryPoints } from 'eve-esi-client-ts';

const instance: FwLeaderboardsCharactersGetVictoryPoints = {
    active_total,
    last_week,
    yesterday,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
