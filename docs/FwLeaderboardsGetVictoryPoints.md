# FwLeaderboardsGetVictoryPoints

Top 4 rankings of factions by victory points from yesterday, last week and in total

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**active_total** | [**Array&lt;FwLeaderboardsGetVictoryPointsActiveTotalInner&gt;**](FwLeaderboardsGetVictoryPointsActiveTotalInner.md) | Top 4 ranking of factions active in faction warfare by total victory points. A faction is considered \&quot;active\&quot; if they have participated in faction warfare in the past 14 days | [default to undefined]
**last_week** | [**Array&lt;FwLeaderboardsGetVictoryPointsLastWeekInner&gt;**](FwLeaderboardsGetVictoryPointsLastWeekInner.md) | Top 4 ranking of factions by victory points in the past week | [default to undefined]
**yesterday** | [**Array&lt;FwLeaderboardsGetVictoryPointsYesterdayInner&gt;**](FwLeaderboardsGetVictoryPointsYesterdayInner.md) | Top 4 ranking of factions by victory points in the past day | [default to undefined]

## Example

```typescript
import { FwLeaderboardsGetVictoryPoints } from 'eve-esi-client-ts';

const instance: FwLeaderboardsGetVictoryPoints = {
    active_total,
    last_week,
    yesterday,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
