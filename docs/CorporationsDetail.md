# CorporationsDetail


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**alliance_id** | **number** | Alliance the corporation is a member of (Player-owned corporation only) | [optional] [default to undefined]
**ceo_id** | **number** | Corporation\&#39;s CEO ID | [optional] [default to undefined]
**creator_id** | **number** | Corporation\&#39;s creator ID | [optional] [default to undefined]
**date_founded** | **string** | Corporation\&#39;s founding date | [optional] [default to undefined]
**description** | **string** | Corporation\&#39;s description | [default to undefined]
**enlisted_faction_id** | **number** | Faction the corporation is enlisted in (Player-owned corporation only) | [optional] [default to undefined]
**friendly_fire** | **string** | Corporation\&#39;s friendly fire status | [default to undefined]
**home_station_id** | **number** | Corporation\&#39;s home station ID | [default to undefined]
**member_count** | **number** | Corporation\&#39;s member count | [default to undefined]
**name** | **string** | Corporation\&#39;s name | [default to undefined]
**palette** | [**CorporationsDetailPalette**](CorporationsDetailPalette.md) | Corporation\&#39;s palette colors (Player-owned corporation only) | [optional] [default to undefined]
**shares** | **number** | Corporation\&#39;s shares | [default to undefined]
**state** | **string** | Corporation\&#39;s state | [default to undefined]
**tax_rates** | [**CorporationsDetailTaxrates**](CorporationsDetailTaxrates.md) | Corporation\&#39;s tax rates | [default to undefined]
**ticker** | **string** | Corporation\&#39;s short name | [default to undefined]
**type** | **string** | Corporation\&#39;s type | [default to undefined]
**url** | **string** | Corporation\&#39;s URL | [optional] [default to undefined]
**war_eligible** | **boolean** | Corporation\&#39;s war eligible | [default to undefined]

## Example

```typescript
import { CorporationsDetail } from 'eve-esi-client-ts';

const instance: CorporationsDetail = {
    alliance_id,
    ceo_id,
    creator_id,
    date_founded,
    description,
    enlisted_faction_id,
    friendly_fire,
    home_station_id,
    member_count,
    name,
    palette,
    shares,
    state,
    tax_rates,
    ticker,
    type,
    url,
    war_eligible,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
