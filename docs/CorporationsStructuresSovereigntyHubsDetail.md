# CorporationsStructuresSovereigntyHubsDetail


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**fuel_access_list_id** | **number** | Access List with who can manage Sovereignty Hub\&#39;s fuel | [optional] [default to undefined]
**id** | **number** | Sovereignty Hub\&#39;s ID | [default to undefined]
**reagent_bay** | [**CorporationsStructuresSovereigntyHubsDetailReagentbay**](CorporationsStructuresSovereigntyHubsDetailReagentbay.md) | Sovereignty Hub\&#39;s reagent bay | [default to undefined]
**resources** | [**CorporationsStructuresSovereigntyHubsDetailResources**](CorporationsStructuresSovereigntyHubsDetailResources.md) | Sovereignty Hub\&#39;s resources | [default to undefined]
**solar_system_id** | **number** | Sovereignty Hub\&#39;s solar system ID | [default to undefined]
**upgrades** | [**Array&lt;CorporationsStructuresSovereigntyHubsDetailUpgrade&gt;**](CorporationsStructuresSovereigntyHubsDetailUpgrade.md) | Sovereignty Hub\&#39;s installed upgrades | [default to undefined]
**vulnerability_window** | [**CorporationsStructuresSovereigntyHubsDetailVulnerabilitywindow**](CorporationsStructuresSovereigntyHubsDetailVulnerabilitywindow.md) | Sovereignty Hub\&#39;s vulnerability window; if omitted, this Sovereignty Hub is part of an active campaign | [optional] [default to undefined]
**workforce_transport** | [**CorporationsStructuresSovereigntyHubsDetailTransport**](CorporationsStructuresSovereigntyHubsDetailTransport.md) | Sovereignty Hub\&#39;s workforce transport settings | [default to undefined]

## Example

```typescript
import { CorporationsStructuresSovereigntyHubsDetail } from 'eve-esi-client-ts';

const instance: CorporationsStructuresSovereigntyHubsDetail = {
    fuel_access_list_id,
    id,
    reagent_bay,
    resources,
    solar_system_id,
    upgrades,
    vulnerability_window,
    workforce_transport,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
