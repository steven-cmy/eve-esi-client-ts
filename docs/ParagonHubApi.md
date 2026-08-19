# ParagonHubApi

All URIs are relative to *https://esi.evetech.net*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**getCharactersParagonHubSkinr**](#getcharactersparagonhubskinr) | **GET** /characters/{character_id}/paragon-hub/skinr | List a character\&#39;s Paragon Hub SKINR listings|
|[**getParagonHubSkinr**](#getparagonhubskinr) | **GET** /paragon-hub/skinr | List public Paragon Hub SKINR listings|
|[**getParagonHubSkinrAlliances**](#getparagonhubskinralliances) | **GET** /paragon-hub/skinr/alliances/{alliance_id} | List Paragon Hub SKINR listings targeted at an alliance|
|[**getParagonHubSkinrCharacters**](#getparagonhubskinrcharacters) | **GET** /paragon-hub/skinr/characters/{character_id} | List Paragon Hub SKINR listings targeted at a character|
|[**getParagonHubSkinrCorporations**](#getparagonhubskinrcorporations) | **GET** /paragon-hub/skinr/corporations/{corporation_id} | List Paragon Hub SKINR listings targeted at a corporation|

# **getCharactersParagonHubSkinr**
> CharactersParagonHubSkinr getCharactersParagonHubSkinr()

List the SKINR listings a character has posted on the Paragon Hub.

### Example

```typescript
import {
    ParagonHubApi,
    Configuration
} from 'eve-esi-client-ts';

const configuration = new Configuration();
const apiInstance = new ParagonHubApi(configuration);

let characterId: number; //The ID of the character whose listings to return (default to undefined)
let xCompatibilityDate: '2026-08-18'; //The compatibility date for the request. (default to undefined)
let after: string; //Return records from after this cursor (mutual exclusive with \'before\'). \'0\' to start from the beginning. (optional) (default to undefined)
let before: string; //Return records from before this cursor (mutual exclusive with \'after\'). \'0\' to start from the end. (optional) (default to undefined)
let limit: number; //The amount of records to retrieve per request. (optional) (default to 10)
let acceptLanguage: 'en' | 'de' | 'fr' | 'ja' | 'ru' | 'zh' | 'ko' | 'es'; //The language to use for the response. (optional) (default to 'en')
let ifNoneMatch: string; //The ETag of the previous request. A 304 will be returned if this matches the current ETag. (optional) (default to undefined)
let xTenant: string; //The tenant ID for the request. (optional) (default to 'tranquility')
let ifModifiedSince: string; //The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. (optional) (default to undefined)

const { status, data } = await apiInstance.getCharactersParagonHubSkinr(
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
| **characterId** | **number** | The ID of the character whose listings to return | defaults to undefined|
| **xCompatibilityDate** | [**&#39;2026-08-18&#39;**]**Array<&#39;2026-08-18&#39;>** | The compatibility date for the request. | defaults to undefined|
| **after** | [**string**] | Return records from after this cursor (mutual exclusive with \&#39;before\&#39;). \&#39;0\&#39; to start from the beginning. | (optional) defaults to undefined|
| **before** | [**string**] | Return records from before this cursor (mutual exclusive with \&#39;after\&#39;). \&#39;0\&#39; to start from the end. | (optional) defaults to undefined|
| **limit** | [**number**] | The amount of records to retrieve per request. | (optional) defaults to 10|
| **acceptLanguage** | [**&#39;en&#39; | &#39;de&#39; | &#39;fr&#39; | &#39;ja&#39; | &#39;ru&#39; | &#39;zh&#39; | &#39;ko&#39; | &#39;es&#39;**]**Array<&#39;en&#39; &#124; &#39;de&#39; &#124; &#39;fr&#39; &#124; &#39;ja&#39; &#124; &#39;ru&#39; &#124; &#39;zh&#39; &#124; &#39;ko&#39; &#124; &#39;es&#39;>** | The language to use for the response. | (optional) defaults to 'en'|
| **ifNoneMatch** | [**string**] | The ETag of the previous request. A 304 will be returned if this matches the current ETag. | (optional) defaults to undefined|
| **xTenant** | [**string**] | The tenant ID for the request. | (optional) defaults to 'tranquility'|
| **ifModifiedSince** | [**string**] | The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. | (optional) defaults to undefined|


### Return type

**CharactersParagonHubSkinr**

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

# **getParagonHubSkinr**
> ParagonHubSkinr getParagonHubSkinr()

Browse the SKINR listings publicly available on the Paragon Hub.

### Example

```typescript
import {
    ParagonHubApi,
    Configuration
} from 'eve-esi-client-ts';

const configuration = new Configuration();
const apiInstance = new ParagonHubApi(configuration);

let xCompatibilityDate: '2026-08-18'; //The compatibility date for the request. (default to undefined)
let after: string; //Return records from after this cursor (mutual exclusive with \'before\'). \'0\' to start from the beginning. (optional) (default to undefined)
let before: string; //Return records from before this cursor (mutual exclusive with \'after\'). \'0\' to start from the end. (optional) (default to undefined)
let limit: number; //The amount of records to retrieve per request. (optional) (default to 10)
let acceptLanguage: 'en' | 'de' | 'fr' | 'ja' | 'ru' | 'zh' | 'ko' | 'es'; //The language to use for the response. (optional) (default to 'en')
let ifNoneMatch: string; //The ETag of the previous request. A 304 will be returned if this matches the current ETag. (optional) (default to undefined)
let xTenant: string; //The tenant ID for the request. (optional) (default to 'tranquility')
let ifModifiedSince: string; //The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. (optional) (default to undefined)

const { status, data } = await apiInstance.getParagonHubSkinr(
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
| **xCompatibilityDate** | [**&#39;2026-08-18&#39;**]**Array<&#39;2026-08-18&#39;>** | The compatibility date for the request. | defaults to undefined|
| **after** | [**string**] | Return records from after this cursor (mutual exclusive with \&#39;before\&#39;). \&#39;0\&#39; to start from the beginning. | (optional) defaults to undefined|
| **before** | [**string**] | Return records from before this cursor (mutual exclusive with \&#39;after\&#39;). \&#39;0\&#39; to start from the end. | (optional) defaults to undefined|
| **limit** | [**number**] | The amount of records to retrieve per request. | (optional) defaults to 10|
| **acceptLanguage** | [**&#39;en&#39; | &#39;de&#39; | &#39;fr&#39; | &#39;ja&#39; | &#39;ru&#39; | &#39;zh&#39; | &#39;ko&#39; | &#39;es&#39;**]**Array<&#39;en&#39; &#124; &#39;de&#39; &#124; &#39;fr&#39; &#124; &#39;ja&#39; &#124; &#39;ru&#39; &#124; &#39;zh&#39; &#124; &#39;ko&#39; &#124; &#39;es&#39;>** | The language to use for the response. | (optional) defaults to 'en'|
| **ifNoneMatch** | [**string**] | The ETag of the previous request. A 304 will be returned if this matches the current ETag. | (optional) defaults to undefined|
| **xTenant** | [**string**] | The tenant ID for the request. | (optional) defaults to 'tranquility'|
| **ifModifiedSince** | [**string**] | The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. | (optional) defaults to undefined|


### Return type

**ParagonHubSkinr**

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

# **getParagonHubSkinrAlliances**
> ParagonHubSkinrAlliances getParagonHubSkinrAlliances()

Browse the SKINR listings on the Paragon Hub that are visible to the given alliance.

### Example

```typescript
import {
    ParagonHubApi,
    Configuration
} from 'eve-esi-client-ts';

const configuration = new Configuration();
const apiInstance = new ParagonHubApi(configuration);

let allianceId: number; //The ID of the alliance the listings are targeted at (default to undefined)
let xCompatibilityDate: '2026-08-18'; //The compatibility date for the request. (default to undefined)
let after: string; //Return records from after this cursor (mutual exclusive with \'before\'). \'0\' to start from the beginning. (optional) (default to undefined)
let before: string; //Return records from before this cursor (mutual exclusive with \'after\'). \'0\' to start from the end. (optional) (default to undefined)
let limit: number; //The amount of records to retrieve per request. (optional) (default to 10)
let acceptLanguage: 'en' | 'de' | 'fr' | 'ja' | 'ru' | 'zh' | 'ko' | 'es'; //The language to use for the response. (optional) (default to 'en')
let ifNoneMatch: string; //The ETag of the previous request. A 304 will be returned if this matches the current ETag. (optional) (default to undefined)
let xTenant: string; //The tenant ID for the request. (optional) (default to 'tranquility')
let ifModifiedSince: string; //The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. (optional) (default to undefined)

const { status, data } = await apiInstance.getParagonHubSkinrAlliances(
    allianceId,
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
| **allianceId** | **number** | The ID of the alliance the listings are targeted at | defaults to undefined|
| **xCompatibilityDate** | [**&#39;2026-08-18&#39;**]**Array<&#39;2026-08-18&#39;>** | The compatibility date for the request. | defaults to undefined|
| **after** | [**string**] | Return records from after this cursor (mutual exclusive with \&#39;before\&#39;). \&#39;0\&#39; to start from the beginning. | (optional) defaults to undefined|
| **before** | [**string**] | Return records from before this cursor (mutual exclusive with \&#39;after\&#39;). \&#39;0\&#39; to start from the end. | (optional) defaults to undefined|
| **limit** | [**number**] | The amount of records to retrieve per request. | (optional) defaults to 10|
| **acceptLanguage** | [**&#39;en&#39; | &#39;de&#39; | &#39;fr&#39; | &#39;ja&#39; | &#39;ru&#39; | &#39;zh&#39; | &#39;ko&#39; | &#39;es&#39;**]**Array<&#39;en&#39; &#124; &#39;de&#39; &#124; &#39;fr&#39; &#124; &#39;ja&#39; &#124; &#39;ru&#39; &#124; &#39;zh&#39; &#124; &#39;ko&#39; &#124; &#39;es&#39;>** | The language to use for the response. | (optional) defaults to 'en'|
| **ifNoneMatch** | [**string**] | The ETag of the previous request. A 304 will be returned if this matches the current ETag. | (optional) defaults to undefined|
| **xTenant** | [**string**] | The tenant ID for the request. | (optional) defaults to 'tranquility'|
| **ifModifiedSince** | [**string**] | The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. | (optional) defaults to undefined|


### Return type

**ParagonHubSkinrAlliances**

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

# **getParagonHubSkinrCharacters**
> ParagonHubSkinrCharacters getParagonHubSkinrCharacters()

Browse the SKINR listings on the Paragon Hub that are visible to the given character.

### Example

```typescript
import {
    ParagonHubApi,
    Configuration
} from 'eve-esi-client-ts';

const configuration = new Configuration();
const apiInstance = new ParagonHubApi(configuration);

let characterId: number; //The ID of the character the listings are targeted at (default to undefined)
let xCompatibilityDate: '2026-08-18'; //The compatibility date for the request. (default to undefined)
let after: string; //Return records from after this cursor (mutual exclusive with \'before\'). \'0\' to start from the beginning. (optional) (default to undefined)
let before: string; //Return records from before this cursor (mutual exclusive with \'after\'). \'0\' to start from the end. (optional) (default to undefined)
let limit: number; //The amount of records to retrieve per request. (optional) (default to 10)
let acceptLanguage: 'en' | 'de' | 'fr' | 'ja' | 'ru' | 'zh' | 'ko' | 'es'; //The language to use for the response. (optional) (default to 'en')
let ifNoneMatch: string; //The ETag of the previous request. A 304 will be returned if this matches the current ETag. (optional) (default to undefined)
let xTenant: string; //The tenant ID for the request. (optional) (default to 'tranquility')
let ifModifiedSince: string; //The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. (optional) (default to undefined)

const { status, data } = await apiInstance.getParagonHubSkinrCharacters(
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
| **characterId** | **number** | The ID of the character the listings are targeted at | defaults to undefined|
| **xCompatibilityDate** | [**&#39;2026-08-18&#39;**]**Array<&#39;2026-08-18&#39;>** | The compatibility date for the request. | defaults to undefined|
| **after** | [**string**] | Return records from after this cursor (mutual exclusive with \&#39;before\&#39;). \&#39;0\&#39; to start from the beginning. | (optional) defaults to undefined|
| **before** | [**string**] | Return records from before this cursor (mutual exclusive with \&#39;after\&#39;). \&#39;0\&#39; to start from the end. | (optional) defaults to undefined|
| **limit** | [**number**] | The amount of records to retrieve per request. | (optional) defaults to 10|
| **acceptLanguage** | [**&#39;en&#39; | &#39;de&#39; | &#39;fr&#39; | &#39;ja&#39; | &#39;ru&#39; | &#39;zh&#39; | &#39;ko&#39; | &#39;es&#39;**]**Array<&#39;en&#39; &#124; &#39;de&#39; &#124; &#39;fr&#39; &#124; &#39;ja&#39; &#124; &#39;ru&#39; &#124; &#39;zh&#39; &#124; &#39;ko&#39; &#124; &#39;es&#39;>** | The language to use for the response. | (optional) defaults to 'en'|
| **ifNoneMatch** | [**string**] | The ETag of the previous request. A 304 will be returned if this matches the current ETag. | (optional) defaults to undefined|
| **xTenant** | [**string**] | The tenant ID for the request. | (optional) defaults to 'tranquility'|
| **ifModifiedSince** | [**string**] | The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. | (optional) defaults to undefined|


### Return type

**ParagonHubSkinrCharacters**

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

# **getParagonHubSkinrCorporations**
> ParagonHubSkinrCorporations getParagonHubSkinrCorporations()

Browse the SKINR listings on the Paragon Hub that are visible to the given corporation.

### Example

```typescript
import {
    ParagonHubApi,
    Configuration
} from 'eve-esi-client-ts';

const configuration = new Configuration();
const apiInstance = new ParagonHubApi(configuration);

let corporationId: number; //The ID of the corporation the listings are targeted at (default to undefined)
let xCompatibilityDate: '2026-08-18'; //The compatibility date for the request. (default to undefined)
let after: string; //Return records from after this cursor (mutual exclusive with \'before\'). \'0\' to start from the beginning. (optional) (default to undefined)
let before: string; //Return records from before this cursor (mutual exclusive with \'after\'). \'0\' to start from the end. (optional) (default to undefined)
let limit: number; //The amount of records to retrieve per request. (optional) (default to 10)
let acceptLanguage: 'en' | 'de' | 'fr' | 'ja' | 'ru' | 'zh' | 'ko' | 'es'; //The language to use for the response. (optional) (default to 'en')
let ifNoneMatch: string; //The ETag of the previous request. A 304 will be returned if this matches the current ETag. (optional) (default to undefined)
let xTenant: string; //The tenant ID for the request. (optional) (default to 'tranquility')
let ifModifiedSince: string; //The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. (optional) (default to undefined)

const { status, data } = await apiInstance.getParagonHubSkinrCorporations(
    corporationId,
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
| **corporationId** | **number** | The ID of the corporation the listings are targeted at | defaults to undefined|
| **xCompatibilityDate** | [**&#39;2026-08-18&#39;**]**Array<&#39;2026-08-18&#39;>** | The compatibility date for the request. | defaults to undefined|
| **after** | [**string**] | Return records from after this cursor (mutual exclusive with \&#39;before\&#39;). \&#39;0\&#39; to start from the beginning. | (optional) defaults to undefined|
| **before** | [**string**] | Return records from before this cursor (mutual exclusive with \&#39;after\&#39;). \&#39;0\&#39; to start from the end. | (optional) defaults to undefined|
| **limit** | [**number**] | The amount of records to retrieve per request. | (optional) defaults to 10|
| **acceptLanguage** | [**&#39;en&#39; | &#39;de&#39; | &#39;fr&#39; | &#39;ja&#39; | &#39;ru&#39; | &#39;zh&#39; | &#39;ko&#39; | &#39;es&#39;**]**Array<&#39;en&#39; &#124; &#39;de&#39; &#124; &#39;fr&#39; &#124; &#39;ja&#39; &#124; &#39;ru&#39; &#124; &#39;zh&#39; &#124; &#39;ko&#39; &#124; &#39;es&#39;>** | The language to use for the response. | (optional) defaults to 'en'|
| **ifNoneMatch** | [**string**] | The ETag of the previous request. A 304 will be returned if this matches the current ETag. | (optional) defaults to undefined|
| **xTenant** | [**string**] | The tenant ID for the request. | (optional) defaults to 'tranquility'|
| **ifModifiedSince** | [**string**] | The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. | (optional) defaults to undefined|


### Return type

**ParagonHubSkinrCorporations**

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

