# FreelanceJobsApi

All URIs are relative to *https://esi.evetech.net*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**getCharactersFreelanceJobsListing**](#getcharactersfreelancejobslisting) | **GET** /characters/{character_id}/freelance-jobs | List character freelance jobs|
|[**getCharactersFreelanceJobsParticipation**](#getcharactersfreelancejobsparticipation) | **GET** /characters/{character_id}/freelance-jobs/{job_id}/participation | Get character freelance job participation|
|[**getCorporationsFreelanceJobsListing**](#getcorporationsfreelancejobslisting) | **GET** /corporations/{corporation_id}/freelance-jobs | List corporation freelance jobs|
|[**getCorporationsFreelanceJobsParticipants**](#getcorporationsfreelancejobsparticipants) | **GET** /corporations/{corporation_id}/freelance-jobs/{job_id}/participants | List participants of a freelance job|
|[**getFreelanceJobsDetail**](#getfreelancejobsdetail) | **GET** /freelance-jobs/{job_id} | Get freelance job details|
|[**getFreelanceJobsListing**](#getfreelancejobslisting) | **GET** /freelance-jobs | List freelance jobs|

# **getCharactersFreelanceJobsListing**
> CharactersFreelanceJobsListing getCharactersFreelanceJobsListing()

Listing of all freelance jobs you are actively participating in.

### Example

```typescript
import {
    FreelanceJobsApi,
    Configuration
} from 'eve-esi-client-ts';

const configuration = new Configuration();
const apiInstance = new FreelanceJobsApi(configuration);

let characterId: number; //The ID of the character (default to undefined)
let xCompatibilityDate: '2025-12-16'; //The compatibility date for the request. (default to undefined)
let acceptLanguage: 'en' | 'de' | 'fr' | 'ja' | 'ru' | 'zh' | 'ko' | 'es'; //The language to use for the response. (optional) (default to 'en')
let ifNoneMatch: string; //The ETag of the previous request. A 304 will be returned if this matches the current ETag. (optional) (default to undefined)
let xTenant: string; //The tenant ID for the request. (optional) (default to 'tranquility')
let ifModifiedSince: string; //The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. (optional) (default to undefined)

const { status, data } = await apiInstance.getCharactersFreelanceJobsListing(
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
| **characterId** | **number** | The ID of the character | defaults to undefined|
| **xCompatibilityDate** | [**&#39;2025-12-16&#39;**]**Array<&#39;2025-12-16&#39;>** | The compatibility date for the request. | defaults to undefined|
| **acceptLanguage** | [**&#39;en&#39; | &#39;de&#39; | &#39;fr&#39; | &#39;ja&#39; | &#39;ru&#39; | &#39;zh&#39; | &#39;ko&#39; | &#39;es&#39;**]**Array<&#39;en&#39; &#124; &#39;de&#39; &#124; &#39;fr&#39; &#124; &#39;ja&#39; &#124; &#39;ru&#39; &#124; &#39;zh&#39; &#124; &#39;ko&#39; &#124; &#39;es&#39;>** | The language to use for the response. | (optional) defaults to 'en'|
| **ifNoneMatch** | [**string**] | The ETag of the previous request. A 304 will be returned if this matches the current ETag. | (optional) defaults to undefined|
| **xTenant** | [**string**] | The tenant ID for the request. | (optional) defaults to 'tranquility'|
| **ifModifiedSince** | [**string**] | The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. | (optional) defaults to undefined|


### Return type

**CharactersFreelanceJobsListing**

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

# **getCharactersFreelanceJobsParticipation**
> CharactersFreelanceJobsParticipation getCharactersFreelanceJobsParticipation()

Show your participation in a freelance job.

### Example

```typescript
import {
    FreelanceJobsApi,
    Configuration
} from 'eve-esi-client-ts';

const configuration = new Configuration();
const apiInstance = new FreelanceJobsApi(configuration);

let characterId: number; //The ID of the character (default to undefined)
let jobId: string; //The ID of the freelance job (default to undefined)
let xCompatibilityDate: '2025-12-16'; //The compatibility date for the request. (default to undefined)
let acceptLanguage: 'en' | 'de' | 'fr' | 'ja' | 'ru' | 'zh' | 'ko' | 'es'; //The language to use for the response. (optional) (default to 'en')
let ifNoneMatch: string; //The ETag of the previous request. A 304 will be returned if this matches the current ETag. (optional) (default to undefined)
let xTenant: string; //The tenant ID for the request. (optional) (default to 'tranquility')
let ifModifiedSince: string; //The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. (optional) (default to undefined)

const { status, data } = await apiInstance.getCharactersFreelanceJobsParticipation(
    characterId,
    jobId,
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
| **jobId** | **string** | The ID of the freelance job | defaults to undefined|
| **xCompatibilityDate** | [**&#39;2025-12-16&#39;**]**Array<&#39;2025-12-16&#39;>** | The compatibility date for the request. | defaults to undefined|
| **acceptLanguage** | [**&#39;en&#39; | &#39;de&#39; | &#39;fr&#39; | &#39;ja&#39; | &#39;ru&#39; | &#39;zh&#39; | &#39;ko&#39; | &#39;es&#39;**]**Array<&#39;en&#39; &#124; &#39;de&#39; &#124; &#39;fr&#39; &#124; &#39;ja&#39; &#124; &#39;ru&#39; &#124; &#39;zh&#39; &#124; &#39;ko&#39; &#124; &#39;es&#39;>** | The language to use for the response. | (optional) defaults to 'en'|
| **ifNoneMatch** | [**string**] | The ETag of the previous request. A 304 will be returned if this matches the current ETag. | (optional) defaults to undefined|
| **xTenant** | [**string**] | The tenant ID for the request. | (optional) defaults to 'tranquility'|
| **ifModifiedSince** | [**string**] | The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. | (optional) defaults to undefined|


### Return type

**CharactersFreelanceJobsParticipation**

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

# **getCorporationsFreelanceJobsListing**
> CorporationsFreelanceJobsListing getCorporationsFreelanceJobsListing()

Listing of all freelance jobs for your corporation.

### Example

```typescript
import {
    FreelanceJobsApi,
    Configuration
} from 'eve-esi-client-ts';

const configuration = new Configuration();
const apiInstance = new FreelanceJobsApi(configuration);

let corporationId: number; //The ID of the corporation (default to undefined)
let xCompatibilityDate: '2025-12-16'; //The compatibility date for the request. (default to undefined)
let after: string; //Return records from after this cursor (mutual exclusive with \'before\'). \'0\' to start from the beginning. (optional) (default to undefined)
let before: string; //Return records from before this cursor (mutual exclusive with \'after\'). \'0\' to start from the end. (optional) (default to undefined)
let limit: number; //The amount of records to retrieve per request. (optional) (default to 10)
let acceptLanguage: 'en' | 'de' | 'fr' | 'ja' | 'ru' | 'zh' | 'ko' | 'es'; //The language to use for the response. (optional) (default to 'en')
let ifNoneMatch: string; //The ETag of the previous request. A 304 will be returned if this matches the current ETag. (optional) (default to undefined)
let xTenant: string; //The tenant ID for the request. (optional) (default to 'tranquility')
let ifModifiedSince: string; //The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. (optional) (default to undefined)

const { status, data } = await apiInstance.getCorporationsFreelanceJobsListing(
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
| **corporationId** | **number** | The ID of the corporation | defaults to undefined|
| **xCompatibilityDate** | [**&#39;2025-12-16&#39;**]**Array<&#39;2025-12-16&#39;>** | The compatibility date for the request. | defaults to undefined|
| **after** | [**string**] | Return records from after this cursor (mutual exclusive with \&#39;before\&#39;). \&#39;0\&#39; to start from the beginning. | (optional) defaults to undefined|
| **before** | [**string**] | Return records from before this cursor (mutual exclusive with \&#39;after\&#39;). \&#39;0\&#39; to start from the end. | (optional) defaults to undefined|
| **limit** | [**number**] | The amount of records to retrieve per request. | (optional) defaults to 10|
| **acceptLanguage** | [**&#39;en&#39; | &#39;de&#39; | &#39;fr&#39; | &#39;ja&#39; | &#39;ru&#39; | &#39;zh&#39; | &#39;ko&#39; | &#39;es&#39;**]**Array<&#39;en&#39; &#124; &#39;de&#39; &#124; &#39;fr&#39; &#124; &#39;ja&#39; &#124; &#39;ru&#39; &#124; &#39;zh&#39; &#124; &#39;ko&#39; &#124; &#39;es&#39;>** | The language to use for the response. | (optional) defaults to 'en'|
| **ifNoneMatch** | [**string**] | The ETag of the previous request. A 304 will be returned if this matches the current ETag. | (optional) defaults to undefined|
| **xTenant** | [**string**] | The tenant ID for the request. | (optional) defaults to 'tranquility'|
| **ifModifiedSince** | [**string**] | The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. | (optional) defaults to undefined|


### Return type

**CorporationsFreelanceJobsListing**

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

# **getCorporationsFreelanceJobsParticipants**
> CorporationsFreelanceJobsParticipants getCorporationsFreelanceJobsParticipants()

Listing of all participants of a freelance job.

### Example

```typescript
import {
    FreelanceJobsApi,
    Configuration
} from 'eve-esi-client-ts';

const configuration = new Configuration();
const apiInstance = new FreelanceJobsApi(configuration);

let corporationId: number; //The ID of the corporation (default to undefined)
let jobId: string; //The ID of the job (default to undefined)
let xCompatibilityDate: '2025-12-16'; //The compatibility date for the request. (default to undefined)
let after: string; //Return records from after this cursor (mutual exclusive with \'before\'). \'0\' to start from the beginning. (optional) (default to undefined)
let before: string; //Return records from before this cursor (mutual exclusive with \'after\'). \'0\' to start from the end. (optional) (default to undefined)
let limit: number; //The amount of records to retrieve per request. (optional) (default to 10)
let acceptLanguage: 'en' | 'de' | 'fr' | 'ja' | 'ru' | 'zh' | 'ko' | 'es'; //The language to use for the response. (optional) (default to 'en')
let ifNoneMatch: string; //The ETag of the previous request. A 304 will be returned if this matches the current ETag. (optional) (default to undefined)
let xTenant: string; //The tenant ID for the request. (optional) (default to 'tranquility')
let ifModifiedSince: string; //The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. (optional) (default to undefined)

const { status, data } = await apiInstance.getCorporationsFreelanceJobsParticipants(
    corporationId,
    jobId,
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
| **jobId** | **string** | The ID of the job | defaults to undefined|
| **xCompatibilityDate** | [**&#39;2025-12-16&#39;**]**Array<&#39;2025-12-16&#39;>** | The compatibility date for the request. | defaults to undefined|
| **after** | [**string**] | Return records from after this cursor (mutual exclusive with \&#39;before\&#39;). \&#39;0\&#39; to start from the beginning. | (optional) defaults to undefined|
| **before** | [**string**] | Return records from before this cursor (mutual exclusive with \&#39;after\&#39;). \&#39;0\&#39; to start from the end. | (optional) defaults to undefined|
| **limit** | [**number**] | The amount of records to retrieve per request. | (optional) defaults to 10|
| **acceptLanguage** | [**&#39;en&#39; | &#39;de&#39; | &#39;fr&#39; | &#39;ja&#39; | &#39;ru&#39; | &#39;zh&#39; | &#39;ko&#39; | &#39;es&#39;**]**Array<&#39;en&#39; &#124; &#39;de&#39; &#124; &#39;fr&#39; &#124; &#39;ja&#39; &#124; &#39;ru&#39; &#124; &#39;zh&#39; &#124; &#39;ko&#39; &#124; &#39;es&#39;>** | The language to use for the response. | (optional) defaults to 'en'|
| **ifNoneMatch** | [**string**] | The ETag of the previous request. A 304 will be returned if this matches the current ETag. | (optional) defaults to undefined|
| **xTenant** | [**string**] | The tenant ID for the request. | (optional) defaults to 'tranquility'|
| **ifModifiedSince** | [**string**] | The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. | (optional) defaults to undefined|


### Return type

**CorporationsFreelanceJobsParticipants**

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

# **getFreelanceJobsDetail**
> FreelanceJobsDetail getFreelanceJobsDetail()

Get the details of a freelance job.  Jobs without an ACL (public jobs) does not require authentication.  Jobs with an ACL requires authentication, and requires that the character is: - An active participant of the job, or - A freelance job manager for the corporation that owns the job.

### Example

```typescript
import {
    FreelanceJobsApi,
    Configuration
} from 'eve-esi-client-ts';

const configuration = new Configuration();
const apiInstance = new FreelanceJobsApi(configuration);

let jobId: string; //The ID of the freelance job (default to undefined)
let xCompatibilityDate: '2025-12-16'; //The compatibility date for the request. (default to undefined)
let acceptLanguage: 'en' | 'de' | 'fr' | 'ja' | 'ru' | 'zh' | 'ko' | 'es'; //The language to use for the response. (optional) (default to 'en')
let ifNoneMatch: string; //The ETag of the previous request. A 304 will be returned if this matches the current ETag. (optional) (default to undefined)
let xTenant: string; //The tenant ID for the request. (optional) (default to 'tranquility')
let ifModifiedSince: string; //The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. (optional) (default to undefined)

const { status, data } = await apiInstance.getFreelanceJobsDetail(
    jobId,
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
| **jobId** | **string** | The ID of the freelance job | defaults to undefined|
| **xCompatibilityDate** | [**&#39;2025-12-16&#39;**]**Array<&#39;2025-12-16&#39;>** | The compatibility date for the request. | defaults to undefined|
| **acceptLanguage** | [**&#39;en&#39; | &#39;de&#39; | &#39;fr&#39; | &#39;ja&#39; | &#39;ru&#39; | &#39;zh&#39; | &#39;ko&#39; | &#39;es&#39;**]**Array<&#39;en&#39; &#124; &#39;de&#39; &#124; &#39;fr&#39; &#124; &#39;ja&#39; &#124; &#39;ru&#39; &#124; &#39;zh&#39; &#124; &#39;ko&#39; &#124; &#39;es&#39;>** | The language to use for the response. | (optional) defaults to 'en'|
| **ifNoneMatch** | [**string**] | The ETag of the previous request. A 304 will be returned if this matches the current ETag. | (optional) defaults to undefined|
| **xTenant** | [**string**] | The tenant ID for the request. | (optional) defaults to 'tranquility'|
| **ifModifiedSince** | [**string**] | The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. | (optional) defaults to undefined|


### Return type

**FreelanceJobsDetail**

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

# **getFreelanceJobsListing**
> FreelanceJobsListing getFreelanceJobsListing()

Listing of all public freelance jobs.

### Example

```typescript
import {
    FreelanceJobsApi,
    Configuration
} from 'eve-esi-client-ts';

const configuration = new Configuration();
const apiInstance = new FreelanceJobsApi(configuration);

let xCompatibilityDate: '2025-12-16'; //The compatibility date for the request. (default to undefined)
let after: string; //Return records from after this cursor (mutual exclusive with \'before\'). \'0\' to start from the beginning. (optional) (default to undefined)
let before: string; //Return records from before this cursor (mutual exclusive with \'after\'). \'0\' to start from the end. (optional) (default to undefined)
let limit: number; //The amount of records to retrieve per request. (optional) (default to 10)
let corporationId: number; //Filter on corporation ID (optional) (default to undefined)
let acceptLanguage: 'en' | 'de' | 'fr' | 'ja' | 'ru' | 'zh' | 'ko' | 'es'; //The language to use for the response. (optional) (default to 'en')
let ifNoneMatch: string; //The ETag of the previous request. A 304 will be returned if this matches the current ETag. (optional) (default to undefined)
let xTenant: string; //The tenant ID for the request. (optional) (default to 'tranquility')
let ifModifiedSince: string; //The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. (optional) (default to undefined)

const { status, data } = await apiInstance.getFreelanceJobsListing(
    xCompatibilityDate,
    after,
    before,
    limit,
    corporationId,
    acceptLanguage,
    ifNoneMatch,
    xTenant,
    ifModifiedSince
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **xCompatibilityDate** | [**&#39;2025-12-16&#39;**]**Array<&#39;2025-12-16&#39;>** | The compatibility date for the request. | defaults to undefined|
| **after** | [**string**] | Return records from after this cursor (mutual exclusive with \&#39;before\&#39;). \&#39;0\&#39; to start from the beginning. | (optional) defaults to undefined|
| **before** | [**string**] | Return records from before this cursor (mutual exclusive with \&#39;after\&#39;). \&#39;0\&#39; to start from the end. | (optional) defaults to undefined|
| **limit** | [**number**] | The amount of records to retrieve per request. | (optional) defaults to 10|
| **corporationId** | **number** | Filter on corporation ID | (optional) defaults to undefined|
| **acceptLanguage** | [**&#39;en&#39; | &#39;de&#39; | &#39;fr&#39; | &#39;ja&#39; | &#39;ru&#39; | &#39;zh&#39; | &#39;ko&#39; | &#39;es&#39;**]**Array<&#39;en&#39; &#124; &#39;de&#39; &#124; &#39;fr&#39; &#124; &#39;ja&#39; &#124; &#39;ru&#39; &#124; &#39;zh&#39; &#124; &#39;ko&#39; &#124; &#39;es&#39;>** | The language to use for the response. | (optional) defaults to 'en'|
| **ifNoneMatch** | [**string**] | The ETag of the previous request. A 304 will be returned if this matches the current ETag. | (optional) defaults to undefined|
| **xTenant** | [**string**] | The tenant ID for the request. | (optional) defaults to 'tranquility'|
| **ifModifiedSince** | [**string**] | The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. | (optional) defaults to undefined|


### Return type

**FreelanceJobsListing**

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

