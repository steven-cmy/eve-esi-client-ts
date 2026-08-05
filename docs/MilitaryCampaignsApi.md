# MilitaryCampaignsApi

All URIs are relative to *https://esi.evetech.net*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**getCharactersMilitaryCampaignsObjectivesListing**](#getcharactersmilitarycampaignsobjectiveslisting) | **GET** /characters/{character_id}/military-campaigns/objectives | List character participation in military campaigns|
|[**getCharactersMilitaryCampaignsObjectivesParticipation**](#getcharactersmilitarycampaignsobjectivesparticipation) | **GET** /characters/{character_id}/military-campaigns/objectives/{objective_id} | Get character military campaign objective participation|
|[**getMilitaryCampaignsDetail**](#getmilitarycampaignsdetail) | **GET** /military-campaigns/{campaign_id} | Get military campaign details|
|[**getMilitaryCampaignsListing**](#getmilitarycampaignslisting) | **GET** /military-campaigns | List military campaigns|
|[**getMilitaryCampaignsObjectivesDetail**](#getmilitarycampaignsobjectivesdetail) | **GET** /military-campaigns/{campaign_id}/objectives/{objective_id} | Get military campaign objective details|
|[**getMilitaryCampaignsObjectivesListing**](#getmilitarycampaignsobjectiveslisting) | **GET** /military-campaigns/{campaign_id}/objectives | List military campaign objectives|

# **getCharactersMilitaryCampaignsObjectivesListing**
> CharactersMilitaryCampaignsObjectivesListing getCharactersMilitaryCampaignsObjectivesListing()

Listing of the military campaign objectives the character has participated in.

### Example

```typescript
import {
    MilitaryCampaignsApi,
    Configuration
} from 'eve-esi-client-ts';

const configuration = new Configuration();
const apiInstance = new MilitaryCampaignsApi(configuration);

let characterId: number; //The ID of the character (default to undefined)
let xCompatibilityDate: '2026-08-04'; //The compatibility date for the request. (default to undefined)
let after: string; //Return records from after this cursor (mutual exclusive with \'before\'). \'0\' to start from the beginning. (optional) (default to undefined)
let before: string; //Return records from before this cursor (mutual exclusive with \'after\'). \'0\' to start from the end. (optional) (default to undefined)
let limit: number; //The amount of records to retrieve per request. (optional) (default to 10)
let acceptLanguage: 'en' | 'de' | 'fr' | 'ja' | 'ru' | 'zh' | 'ko' | 'es'; //The language to use for the response. (optional) (default to 'en')
let ifNoneMatch: string; //The ETag of the previous request. A 304 will be returned if this matches the current ETag. (optional) (default to undefined)
let xTenant: string; //The tenant ID for the request. (optional) (default to 'tranquility')
let ifModifiedSince: string; //The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. (optional) (default to undefined)

const { status, data } = await apiInstance.getCharactersMilitaryCampaignsObjectivesListing(
    characterId,
    xCompatibilityDate,
    after,
    before,
    limit,
    acceptLanguage,
    ifNoneMatch,
    xTenant,
    ifModifiedSince
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **characterId** | **number** | The ID of the character | defaults to undefined|
| **xCompatibilityDate** | [**&#39;2026-08-04&#39;**]**Array<&#39;2026-08-04&#39;>** | The compatibility date for the request. | defaults to undefined|
| **after** | [**string**] | Return records from after this cursor (mutual exclusive with \&#39;before\&#39;). \&#39;0\&#39; to start from the beginning. | (optional) defaults to undefined|
| **before** | [**string**] | Return records from before this cursor (mutual exclusive with \&#39;after\&#39;). \&#39;0\&#39; to start from the end. | (optional) defaults to undefined|
| **limit** | [**number**] | The amount of records to retrieve per request. | (optional) defaults to 10|
| **acceptLanguage** | [**&#39;en&#39; | &#39;de&#39; | &#39;fr&#39; | &#39;ja&#39; | &#39;ru&#39; | &#39;zh&#39; | &#39;ko&#39; | &#39;es&#39;**]**Array<&#39;en&#39; &#124; &#39;de&#39; &#124; &#39;fr&#39; &#124; &#39;ja&#39; &#124; &#39;ru&#39; &#124; &#39;zh&#39; &#124; &#39;ko&#39; &#124; &#39;es&#39;>** | The language to use for the response. | (optional) defaults to 'en'|
| **ifNoneMatch** | [**string**] | The ETag of the previous request. A 304 will be returned if this matches the current ETag. | (optional) defaults to undefined|
| **xTenant** | [**string**] | The tenant ID for the request. | (optional) defaults to 'tranquility'|
| **ifModifiedSince** | [**string**] | The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. | (optional) defaults to undefined|


### Return type

**CharactersMilitaryCampaignsObjectivesListing**

### Authorization

[OAuth2](../README.md#OAuth2)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | OK |  * Cache-Control -  <br>  * ETag -  <br>  * Last-Modified -  <br>  |
|**0** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getCharactersMilitaryCampaignsObjectivesParticipation**
> CharactersMilitaryCampaignsObjectivesParticipation getCharactersMilitaryCampaignsObjectivesParticipation()

Show your participation in a military campaign objective.

### Example

```typescript
import {
    MilitaryCampaignsApi,
    Configuration
} from 'eve-esi-client-ts';

const configuration = new Configuration();
const apiInstance = new MilitaryCampaignsApi(configuration);

let characterId: number; //The ID of the character (default to undefined)
let objectiveId: string; //The ID of the objective (default to undefined)
let xCompatibilityDate: '2026-08-04'; //The compatibility date for the request. (default to undefined)
let acceptLanguage: 'en' | 'de' | 'fr' | 'ja' | 'ru' | 'zh' | 'ko' | 'es'; //The language to use for the response. (optional) (default to 'en')
let ifNoneMatch: string; //The ETag of the previous request. A 304 will be returned if this matches the current ETag. (optional) (default to undefined)
let xTenant: string; //The tenant ID for the request. (optional) (default to 'tranquility')
let ifModifiedSince: string; //The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. (optional) (default to undefined)

const { status, data } = await apiInstance.getCharactersMilitaryCampaignsObjectivesParticipation(
    characterId,
    objectiveId,
    xCompatibilityDate,
    acceptLanguage,
    ifNoneMatch,
    xTenant,
    ifModifiedSince
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **characterId** | **number** | The ID of the character | defaults to undefined|
| **objectiveId** | **string** | The ID of the objective | defaults to undefined|
| **xCompatibilityDate** | [**&#39;2026-08-04&#39;**]**Array<&#39;2026-08-04&#39;>** | The compatibility date for the request. | defaults to undefined|
| **acceptLanguage** | [**&#39;en&#39; | &#39;de&#39; | &#39;fr&#39; | &#39;ja&#39; | &#39;ru&#39; | &#39;zh&#39; | &#39;ko&#39; | &#39;es&#39;**]**Array<&#39;en&#39; &#124; &#39;de&#39; &#124; &#39;fr&#39; &#124; &#39;ja&#39; &#124; &#39;ru&#39; &#124; &#39;zh&#39; &#124; &#39;ko&#39; &#124; &#39;es&#39;>** | The language to use for the response. | (optional) defaults to 'en'|
| **ifNoneMatch** | [**string**] | The ETag of the previous request. A 304 will be returned if this matches the current ETag. | (optional) defaults to undefined|
| **xTenant** | [**string**] | The tenant ID for the request. | (optional) defaults to 'tranquility'|
| **ifModifiedSince** | [**string**] | The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. | (optional) defaults to undefined|


### Return type

**CharactersMilitaryCampaignsObjectivesParticipation**

### Authorization

[OAuth2](../README.md#OAuth2)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | OK |  * Cache-Control -  <br>  * ETag -  <br>  * Last-Modified -  <br>  |
|**0** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getMilitaryCampaignsDetail**
> MilitaryCampaignsDetail getMilitaryCampaignsDetail()

Get the details of a military campaign.

### Example

```typescript
import {
    MilitaryCampaignsApi,
    Configuration
} from 'eve-esi-client-ts';

const configuration = new Configuration();
const apiInstance = new MilitaryCampaignsApi(configuration);

let campaignId: string; //The ID of the military campaign (default to undefined)
let xCompatibilityDate: '2026-08-04'; //The compatibility date for the request. (default to undefined)
let acceptLanguage: 'en' | 'de' | 'fr' | 'ja' | 'ru' | 'zh' | 'ko' | 'es'; //The language to use for the response. (optional) (default to 'en')
let ifNoneMatch: string; //The ETag of the previous request. A 304 will be returned if this matches the current ETag. (optional) (default to undefined)
let xTenant: string; //The tenant ID for the request. (optional) (default to 'tranquility')
let ifModifiedSince: string; //The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. (optional) (default to undefined)

const { status, data } = await apiInstance.getMilitaryCampaignsDetail(
    campaignId,
    xCompatibilityDate,
    acceptLanguage,
    ifNoneMatch,
    xTenant,
    ifModifiedSince
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **campaignId** | **string** | The ID of the military campaign | defaults to undefined|
| **xCompatibilityDate** | [**&#39;2026-08-04&#39;**]**Array<&#39;2026-08-04&#39;>** | The compatibility date for the request. | defaults to undefined|
| **acceptLanguage** | [**&#39;en&#39; | &#39;de&#39; | &#39;fr&#39; | &#39;ja&#39; | &#39;ru&#39; | &#39;zh&#39; | &#39;ko&#39; | &#39;es&#39;**]**Array<&#39;en&#39; &#124; &#39;de&#39; &#124; &#39;fr&#39; &#124; &#39;ja&#39; &#124; &#39;ru&#39; &#124; &#39;zh&#39; &#124; &#39;ko&#39; &#124; &#39;es&#39;>** | The language to use for the response. | (optional) defaults to 'en'|
| **ifNoneMatch** | [**string**] | The ETag of the previous request. A 304 will be returned if this matches the current ETag. | (optional) defaults to undefined|
| **xTenant** | [**string**] | The tenant ID for the request. | (optional) defaults to 'tranquility'|
| **ifModifiedSince** | [**string**] | The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. | (optional) defaults to undefined|


### Return type

**MilitaryCampaignsDetail**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | OK |  * Cache-Control -  <br>  * ETag -  <br>  * Last-Modified -  <br>  |
|**0** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getMilitaryCampaignsListing**
> MilitaryCampaignsListing getMilitaryCampaignsListing()

Listing of all active military campaigns.

### Example

```typescript
import {
    MilitaryCampaignsApi,
    Configuration
} from 'eve-esi-client-ts';

const configuration = new Configuration();
const apiInstance = new MilitaryCampaignsApi(configuration);

let xCompatibilityDate: '2026-08-04'; //The compatibility date for the request. (default to undefined)
let acceptLanguage: 'en' | 'de' | 'fr' | 'ja' | 'ru' | 'zh' | 'ko' | 'es'; //The language to use for the response. (optional) (default to 'en')
let ifNoneMatch: string; //The ETag of the previous request. A 304 will be returned if this matches the current ETag. (optional) (default to undefined)
let xTenant: string; //The tenant ID for the request. (optional) (default to 'tranquility')
let ifModifiedSince: string; //The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. (optional) (default to undefined)

const { status, data } = await apiInstance.getMilitaryCampaignsListing(
    xCompatibilityDate,
    acceptLanguage,
    ifNoneMatch,
    xTenant,
    ifModifiedSince
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **xCompatibilityDate** | [**&#39;2026-08-04&#39;**]**Array<&#39;2026-08-04&#39;>** | The compatibility date for the request. | defaults to undefined|
| **acceptLanguage** | [**&#39;en&#39; | &#39;de&#39; | &#39;fr&#39; | &#39;ja&#39; | &#39;ru&#39; | &#39;zh&#39; | &#39;ko&#39; | &#39;es&#39;**]**Array<&#39;en&#39; &#124; &#39;de&#39; &#124; &#39;fr&#39; &#124; &#39;ja&#39; &#124; &#39;ru&#39; &#124; &#39;zh&#39; &#124; &#39;ko&#39; &#124; &#39;es&#39;>** | The language to use for the response. | (optional) defaults to 'en'|
| **ifNoneMatch** | [**string**] | The ETag of the previous request. A 304 will be returned if this matches the current ETag. | (optional) defaults to undefined|
| **xTenant** | [**string**] | The tenant ID for the request. | (optional) defaults to 'tranquility'|
| **ifModifiedSince** | [**string**] | The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. | (optional) defaults to undefined|


### Return type

**MilitaryCampaignsListing**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | OK |  * Cache-Control -  <br>  * ETag -  <br>  * Last-Modified -  <br>  |
|**0** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getMilitaryCampaignsObjectivesDetail**
> MilitaryCampaignsObjectivesDetail getMilitaryCampaignsObjectivesDetail()

Get the details of an objective of a military campaign.

### Example

```typescript
import {
    MilitaryCampaignsApi,
    Configuration
} from 'eve-esi-client-ts';

const configuration = new Configuration();
const apiInstance = new MilitaryCampaignsApi(configuration);

let campaignId: string; //The ID of the military campaign (default to undefined)
let objectiveId: string; //The ID of the objective (default to undefined)
let xCompatibilityDate: '2026-08-04'; //The compatibility date for the request. (default to undefined)
let acceptLanguage: 'en' | 'de' | 'fr' | 'ja' | 'ru' | 'zh' | 'ko' | 'es'; //The language to use for the response. (optional) (default to 'en')
let ifNoneMatch: string; //The ETag of the previous request. A 304 will be returned if this matches the current ETag. (optional) (default to undefined)
let xTenant: string; //The tenant ID for the request. (optional) (default to 'tranquility')
let ifModifiedSince: string; //The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. (optional) (default to undefined)

const { status, data } = await apiInstance.getMilitaryCampaignsObjectivesDetail(
    campaignId,
    objectiveId,
    xCompatibilityDate,
    acceptLanguage,
    ifNoneMatch,
    xTenant,
    ifModifiedSince
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **campaignId** | **string** | The ID of the military campaign | defaults to undefined|
| **objectiveId** | **string** | The ID of the objective | defaults to undefined|
| **xCompatibilityDate** | [**&#39;2026-08-04&#39;**]**Array<&#39;2026-08-04&#39;>** | The compatibility date for the request. | defaults to undefined|
| **acceptLanguage** | [**&#39;en&#39; | &#39;de&#39; | &#39;fr&#39; | &#39;ja&#39; | &#39;ru&#39; | &#39;zh&#39; | &#39;ko&#39; | &#39;es&#39;**]**Array<&#39;en&#39; &#124; &#39;de&#39; &#124; &#39;fr&#39; &#124; &#39;ja&#39; &#124; &#39;ru&#39; &#124; &#39;zh&#39; &#124; &#39;ko&#39; &#124; &#39;es&#39;>** | The language to use for the response. | (optional) defaults to 'en'|
| **ifNoneMatch** | [**string**] | The ETag of the previous request. A 304 will be returned if this matches the current ETag. | (optional) defaults to undefined|
| **xTenant** | [**string**] | The tenant ID for the request. | (optional) defaults to 'tranquility'|
| **ifModifiedSince** | [**string**] | The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. | (optional) defaults to undefined|


### Return type

**MilitaryCampaignsObjectivesDetail**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | OK |  * Cache-Control -  <br>  * ETag -  <br>  * Last-Modified -  <br>  |
|**0** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getMilitaryCampaignsObjectivesListing**
> MilitaryCampaignsObjectivesListing getMilitaryCampaignsObjectivesListing()

Listing of all active, completed or expired objectives of a military campaign.

### Example

```typescript
import {
    MilitaryCampaignsApi,
    Configuration
} from 'eve-esi-client-ts';

const configuration = new Configuration();
const apiInstance = new MilitaryCampaignsApi(configuration);

let campaignId: string; //The ID of the military campaign (default to undefined)
let xCompatibilityDate: '2026-08-04'; //The compatibility date for the request. (default to undefined)
let after: string; //Return records from after this cursor (mutual exclusive with \'before\'). \'0\' to start from the beginning. (optional) (default to undefined)
let before: string; //Return records from before this cursor (mutual exclusive with \'after\'). \'0\' to start from the end. (optional) (default to undefined)
let limit: number; //The amount of records to retrieve per request. (optional) (default to 10)
let acceptLanguage: 'en' | 'de' | 'fr' | 'ja' | 'ru' | 'zh' | 'ko' | 'es'; //The language to use for the response. (optional) (default to 'en')
let ifNoneMatch: string; //The ETag of the previous request. A 304 will be returned if this matches the current ETag. (optional) (default to undefined)
let xTenant: string; //The tenant ID for the request. (optional) (default to 'tranquility')
let ifModifiedSince: string; //The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. (optional) (default to undefined)

const { status, data } = await apiInstance.getMilitaryCampaignsObjectivesListing(
    campaignId,
    xCompatibilityDate,
    after,
    before,
    limit,
    acceptLanguage,
    ifNoneMatch,
    xTenant,
    ifModifiedSince
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **campaignId** | **string** | The ID of the military campaign | defaults to undefined|
| **xCompatibilityDate** | [**&#39;2026-08-04&#39;**]**Array<&#39;2026-08-04&#39;>** | The compatibility date for the request. | defaults to undefined|
| **after** | [**string**] | Return records from after this cursor (mutual exclusive with \&#39;before\&#39;). \&#39;0\&#39; to start from the beginning. | (optional) defaults to undefined|
| **before** | [**string**] | Return records from before this cursor (mutual exclusive with \&#39;after\&#39;). \&#39;0\&#39; to start from the end. | (optional) defaults to undefined|
| **limit** | [**number**] | The amount of records to retrieve per request. | (optional) defaults to 10|
| **acceptLanguage** | [**&#39;en&#39; | &#39;de&#39; | &#39;fr&#39; | &#39;ja&#39; | &#39;ru&#39; | &#39;zh&#39; | &#39;ko&#39; | &#39;es&#39;**]**Array<&#39;en&#39; &#124; &#39;de&#39; &#124; &#39;fr&#39; &#124; &#39;ja&#39; &#124; &#39;ru&#39; &#124; &#39;zh&#39; &#124; &#39;ko&#39; &#124; &#39;es&#39;>** | The language to use for the response. | (optional) defaults to 'en'|
| **ifNoneMatch** | [**string**] | The ETag of the previous request. A 304 will be returned if this matches the current ETag. | (optional) defaults to undefined|
| **xTenant** | [**string**] | The tenant ID for the request. | (optional) defaults to 'tranquility'|
| **ifModifiedSince** | [**string**] | The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. | (optional) defaults to undefined|


### Return type

**MilitaryCampaignsObjectivesListing**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | OK |  * Cache-Control -  <br>  * ETag -  <br>  * Last-Modified -  <br>  |
|**0** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

