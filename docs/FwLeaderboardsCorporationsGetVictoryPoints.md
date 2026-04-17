# FwLeaderboardsCorporationsGetVictoryPoints

Top 10 rankings of corporations by victory points from yesterday, last week and in total

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**active_total** | [**Array&lt;FwLeaderboardsCorporationsGetVictoryPointsActiveTotalInner&gt;**](FwLeaderboardsCorporationsGetVictoryPointsActiveTotalInner.md) | Top 10 ranking of corporations active in faction warfare by total victory points. A corporation is considered \&quot;active\&quot; if they have participated in faction warfare in the past 14 days | [default to undefined]
**last_week** | [**Array&lt;FwLeaderboardsCorporationsGetVictoryPointsLastWeekInner&gt;**](FwLeaderboardsCorporationsGetVictoryPointsLastWeekInner.md) | Top 10 ranking of corporations by victory points in the past week | [default to undefined]
**yesterday** | [**Array&lt;FwLeaderboardsCorporationsGetVictoryPointsYesterdayInner&gt;**](FwLeaderboardsCorporationsGetVictoryPointsYesterdayInner.md) | Top 10 ranking of corporations by victory points in the past day | [default to undefined]

## Example

```typescript
import { FwLeaderboardsCorporationsGetVictoryPoints } from 'eve-esi-client-ts';

const instance: FwLeaderboardsCorporationsGetVictoryPoints = {
    active_total,
    last_week,
    yesterday,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
