# CorporationProjectsApi

All URIs are relative to *https://esi.evetech.net*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**getCorporationsProjectsContribution**](#getcorporationsprojectscontribution) | **GET** /corporations/{corporation_id}/projects/{project_id}/contribution/{character_id} | Get your project contribution|
|[**getCorporationsProjectsContributors**](#getcorporationsprojectscontributors) | **GET** /corporations/{corporation_id}/projects/{project_id}/contributors | List project contributors|
|[**getCorporationsProjectsDetail**](#getcorporationsprojectsdetail) | **GET** /corporations/{corporation_id}/projects/{project_id} | Get project details|
|[**getCorporationsProjectsListing**](#getcorporationsprojectslisting) | **GET** /corporations/{corporation_id}/projects | List corporation projects|

# **getCorporationsProjectsContribution**
> CorporationsProjectsContribution getCorporationsProjectsContribution()

Show your contribution to a corporation project.

### Example

```typescript
import {
    CorporationProjectsApi,
    Configuration
} from 'eve-esi-client-ts';

const configuration = new Configuration();
const apiInstance = new CorporationProjectsApi(configuration);

let corporationId: number; //The ID of the corporation (default to undefined)
let projectId: string; //The ID of the project (default to undefined)
let characterId: number; //The ID of the character (default to undefined)
let xCompatibilityDate: '2025-12-16'; //The compatibility date for the request. (default to undefined)
let acceptLanguage: 'en' | 'de' | 'fr' | 'ja' | 'ru' | 'zh' | 'ko' | 'es'; //The language to use for the response. (optional) (default to 'en')
let ifNoneMatch: string; //The ETag of the previous request. A 304 will be returned if this matches the current ETag. (optional) (default to undefined)
let xTenant: string; //The tenant ID for the request. (optional) (default to 'tranquility')
let ifModifiedSince: string; //The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. (optional) (default to undefined)

const { status, data } = await apiInstance.getCorporationsProjectsContribution(
    corporationId,
    projectId,
    characterId,
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
| **corporationId** | **number** | The ID of the corporation | defaults to undefined|
| **projectId** | **string** | The ID of the project | defaults to undefined|
| **characterId** | **number** | The ID of the character | defaults to undefined|
| **xCompatibilityDate** | [**&#39;2025-12-16&#39;**]**Array<&#39;2025-12-16&#39;>** | The compatibility date for the request. | defaults to undefined|
| **acceptLanguage** | [**&#39;en&#39; | &#39;de&#39; | &#39;fr&#39; | &#39;ja&#39; | &#39;ru&#39; | &#39;zh&#39; | &#39;ko&#39; | &#39;es&#39;**]**Array<&#39;en&#39; &#124; &#39;de&#39; &#124; &#39;fr&#39; &#124; &#39;ja&#39; &#124; &#39;ru&#39; &#124; &#39;zh&#39; &#124; &#39;ko&#39; &#124; &#39;es&#39;>** | The language to use for the response. | (optional) defaults to 'en'|
| **ifNoneMatch** | [**string**] | The ETag of the previous request. A 304 will be returned if this matches the current ETag. | (optional) defaults to undefined|
| **xTenant** | [**string**] | The tenant ID for the request. | (optional) defaults to 'tranquility'|
| **ifModifiedSince** | [**string**] | The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. | (optional) defaults to undefined|


### Return type

**CorporationsProjectsContribution**

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

# **getCorporationsProjectsContributors**
> CorporationsProjectsContributors getCorporationsProjectsContributors()

Listing of all contributors to a corporation project.

### Example

```typescript
import {
    CorporationProjectsApi,
    Configuration
} from 'eve-esi-client-ts';

const configuration = new Configuration();
const apiInstance = new CorporationProjectsApi(configuration);

let corporationId: number; //The ID of the corporation (default to undefined)
let projectId: string; //The ID of the project (default to undefined)
let xCompatibilityDate: '2025-12-16'; //The compatibility date for the request. (default to undefined)
let after: string; //Return records from after this cursor (mutual exclusive with \'before\'). \'0\' to start from the beginning. (optional) (default to undefined)
let before: string; //Return records from before this cursor (mutual exclusive with \'after\'). \'0\' to start from the end. (optional) (default to undefined)
let limit: number; //The amount of records to retrieve per request. (optional) (default to 10)
let acceptLanguage: 'en' | 'de' | 'fr' | 'ja' | 'ru' | 'zh' | 'ko' | 'es'; //The language to use for the response. (optional) (default to 'en')
let ifNoneMatch: string; //The ETag of the previous request. A 304 will be returned if this matches the current ETag. (optional) (default to undefined)
let xTenant: string; //The tenant ID for the request. (optional) (default to 'tranquility')
let ifModifiedSince: string; //The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. (optional) (default to undefined)

const { status, data } = await apiInstance.getCorporationsProjectsContributors(
    corporationId,
    projectId,
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
| **corporationId** | **number** | The ID of the corporation | defaults to undefined|
| **projectId** | **string** | The ID of the project | defaults to undefined|
| **xCompatibilityDate** | [**&#39;2025-12-16&#39;**]**Array<&#39;2025-12-16&#39;>** | The compatibility date for the request. | defaults to undefined|
| **after** | [**string**] | Return records from after this cursor (mutual exclusive with \&#39;before\&#39;). \&#39;0\&#39; to start from the beginning. | (optional) defaults to undefined|
| **before** | [**string**] | Return records from before this cursor (mutual exclusive with \&#39;after\&#39;). \&#39;0\&#39; to start from the end. | (optional) defaults to undefined|
| **limit** | [**number**] | The amount of records to retrieve per request. | (optional) defaults to 10|
| **acceptLanguage** | [**&#39;en&#39; | &#39;de&#39; | &#39;fr&#39; | &#39;ja&#39; | &#39;ru&#39; | &#39;zh&#39; | &#39;ko&#39; | &#39;es&#39;**]**Array<&#39;en&#39; &#124; &#39;de&#39; &#124; &#39;fr&#39; &#124; &#39;ja&#39; &#124; &#39;ru&#39; &#124; &#39;zh&#39; &#124; &#39;ko&#39; &#124; &#39;es&#39;>** | The language to use for the response. | (optional) defaults to 'en'|
| **ifNoneMatch** | [**string**] | The ETag of the previous request. A 304 will be returned if this matches the current ETag. | (optional) defaults to undefined|
| **xTenant** | [**string**] | The tenant ID for the request. | (optional) defaults to 'tranquility'|
| **ifModifiedSince** | [**string**] | The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. | (optional) defaults to undefined|


### Return type

**CorporationsProjectsContributors**

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

# **getCorporationsProjectsDetail**
> CorporationsProjectsDetail getCorporationsProjectsDetail()

Get the details of a corporation project.

### Example

```typescript
import {
    CorporationProjectsApi,
    Configuration
} from 'eve-esi-client-ts';

const configuration = new Configuration();
const apiInstance = new CorporationProjectsApi(configuration);

let corporationId: number; //The ID of the corporation (default to undefined)
let projectId: string; //The ID of the project (default to undefined)
let xCompatibilityDate: '2025-12-16'; //The compatibility date for the request. (default to undefined)
let acceptLanguage: 'en' | 'de' | 'fr' | 'ja' | 'ru' | 'zh' | 'ko' | 'es'; //The language to use for the response. (optional) (default to 'en')
let ifNoneMatch: string; //The ETag of the previous request. A 304 will be returned if this matches the current ETag. (optional) (default to undefined)
let xTenant: string; //The tenant ID for the request. (optional) (default to 'tranquility')
let ifModifiedSince: string; //The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. (optional) (default to undefined)

const { status, data } = await apiInstance.getCorporationsProjectsDetail(
    corporationId,
    projectId,
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
| **corporationId** | **number** | The ID of the corporation | defaults to undefined|
| **projectId** | **string** | The ID of the project | defaults to undefined|
| **xCompatibilityDate** | [**&#39;2025-12-16&#39;**]**Array<&#39;2025-12-16&#39;>** | The compatibility date for the request. | defaults to undefined|
| **acceptLanguage** | [**&#39;en&#39; | &#39;de&#39; | &#39;fr&#39; | &#39;ja&#39; | &#39;ru&#39; | &#39;zh&#39; | &#39;ko&#39; | &#39;es&#39;**]**Array<&#39;en&#39; &#124; &#39;de&#39; &#124; &#39;fr&#39; &#124; &#39;ja&#39; &#124; &#39;ru&#39; &#124; &#39;zh&#39; &#124; &#39;ko&#39; &#124; &#39;es&#39;>** | The language to use for the response. | (optional) defaults to 'en'|
| **ifNoneMatch** | [**string**] | The ETag of the previous request. A 304 will be returned if this matches the current ETag. | (optional) defaults to undefined|
| **xTenant** | [**string**] | The tenant ID for the request. | (optional) defaults to 'tranquility'|
| **ifModifiedSince** | [**string**] | The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. | (optional) defaults to undefined|


### Return type

**CorporationsProjectsDetail**

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

# **getCorporationsProjectsListing**
> CorporationsProjectsListing getCorporationsProjectsListing()

Listing of all (active) corporation projects.

### Example

```typescript
import {
    CorporationProjectsApi,
    Configuration
} from 'eve-esi-client-ts';

const configuration = new Configuration();
const apiInstance = new CorporationProjectsApi(configuration);

let corporationId: number; //The ID of the corporation (default to undefined)
let xCompatibilityDate: '2025-12-16'; //The compatibility date for the request. (default to undefined)
let after: string; //Return records from after this cursor (mutual exclusive with \'before\'). \'0\' to start from the beginning. (optional) (default to undefined)
let before: string; //Return records from before this cursor (mutual exclusive with \'after\'). \'0\' to start from the end. (optional) (default to undefined)
let limit: number; //The amount of records to retrieve per request. (optional) (default to 10)
let state: 'All' | 'Active'; //Filter by state (optional) (default to 'Active')
let acceptLanguage: 'en' | 'de' | 'fr' | 'ja' | 'ru' | 'zh' | 'ko' | 'es'; //The language to use for the response. (optional) (default to 'en')
let ifNoneMatch: string; //The ETag of the previous request. A 304 will be returned if this matches the current ETag. (optional) (default to undefined)
let xTenant: string; //The tenant ID for the request. (optional) (default to 'tranquility')
let ifModifiedSince: string; //The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. (optional) (default to undefined)

const { status, data } = await apiInstance.getCorporationsProjectsListing(
    corporationId,
    xCompatibilityDate,
    after,
    before,
    limit,
    state,
    acceptLanguage,
    ifNoneMatch,
    xTenant,
    ifModifiedSince
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **corporationId** | **number** | The ID of the corporation | defaults to undefined|
| **xCompatibilityDate** | [**&#39;2025-12-16&#39;**]**Array<&#39;2025-12-16&#39;>** | The compatibility date for the request. | defaults to undefined|
| **after** | [**string**] | Return records from after this cursor (mutual exclusive with \&#39;before\&#39;). \&#39;0\&#39; to start from the beginning. | (optional) defaults to undefined|
| **before** | [**string**] | Return records from before this cursor (mutual exclusive with \&#39;after\&#39;). \&#39;0\&#39; to start from the end. | (optional) defaults to undefined|
| **limit** | [**number**] | The amount of records to retrieve per request. | (optional) defaults to 10|
| **state** | [**&#39;All&#39; | &#39;Active&#39;**]**Array<&#39;All&#39; &#124; &#39;Active&#39;>** | Filter by state | (optional) defaults to 'Active'|
| **acceptLanguage** | [**&#39;en&#39; | &#39;de&#39; | &#39;fr&#39; | &#39;ja&#39; | &#39;ru&#39; | &#39;zh&#39; | &#39;ko&#39; | &#39;es&#39;**]**Array<&#39;en&#39; &#124; &#39;de&#39; &#124; &#39;fr&#39; &#124; &#39;ja&#39; &#124; &#39;ru&#39; &#124; &#39;zh&#39; &#124; &#39;ko&#39; &#124; &#39;es&#39;>** | The language to use for the response. | (optional) defaults to 'en'|
| **ifNoneMatch** | [**string**] | The ETag of the previous request. A 304 will be returned if this matches the current ETag. | (optional) defaults to undefined|
| **xTenant** | [**string**] | The tenant ID for the request. | (optional) defaults to 'tranquility'|
| **ifModifiedSince** | [**string**] | The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. | (optional) defaults to undefined|


### Return type

**CorporationsProjectsListing**

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

