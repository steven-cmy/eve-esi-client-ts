# SearchApi

All URIs are relative to *https://esi.evetech.net*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**getCharactersCharacterIdSearch**](#getcharacterscharacteridsearch) | **GET** /characters/{character_id}/search | Search on a string|

# **getCharactersCharacterIdSearch**
> CharactersCharacterIdSearchGet getCharactersCharacterIdSearch()

Search for entities that match a given sub-string.

### Example

```typescript
import {
    SearchApi,
    Configuration
} from 'eve-esi-client-ts';

const configuration = new Configuration();
const apiInstance = new SearchApi(configuration);

let categories: Set<'agent' | 'alliance' | 'character' | 'constellation' | 'corporation' | 'faction' | 'inventory_type' | 'region' | 'solar_system' | 'station' | 'structure'>; // (default to undefined)
let characterId: number; //The ID of the character (default to undefined)
let search: string; // (default to undefined)
let xCompatibilityDate: '2020-01-01'; //The compatibility date for the request. (default to undefined)
let strict: boolean; // (optional) (default to false)
let acceptLanguage: 'en' | 'de' | 'fr' | 'ja' | 'ru' | 'zh' | 'ko' | 'es'; //The language to use for the response. (optional) (default to 'en')
let ifNoneMatch: string; //The ETag of the previous request. A 304 will be returned if this matches the current ETag. (optional) (default to undefined)
let xTenant: string; //The tenant ID for the request. (optional) (default to 'tranquility')
let ifModifiedSince: string; //The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. (optional) (default to undefined)

const { status, data } = await apiInstance.getCharactersCharacterIdSearch(
    categories,
    characterId,
    search,
    xCompatibilityDate,
    strict,
    acceptLanguage,
    ifNoneMatch,
    xTenant,
    ifModifiedSince
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **categories** | **Array<&#39;agent&#39; &#124; &#39;alliance&#39; &#124; &#39;character&#39; &#124; &#39;constellation&#39; &#124; &#39;corporation&#39; &#124; &#39;faction&#39; &#124; &#39;inventory_type&#39; &#124; &#39;region&#39; &#124; &#39;solar_system&#39; &#124; &#39;station&#39; &#124; &#39;structure&#39;>** |  | defaults to undefined|
| **characterId** | [**number**] | The ID of the character | defaults to undefined|
| **search** | [**string**] |  | defaults to undefined|
| **xCompatibilityDate** | [**&#39;2020-01-01&#39;**]**Array<&#39;2020-01-01&#39;>** | The compatibility date for the request. | defaults to undefined|
| **strict** | [**boolean**] |  | (optional) defaults to false|
| **acceptLanguage** | [**&#39;en&#39; | &#39;de&#39; | &#39;fr&#39; | &#39;ja&#39; | &#39;ru&#39; | &#39;zh&#39; | &#39;ko&#39; | &#39;es&#39;**]**Array<&#39;en&#39; &#124; &#39;de&#39; &#124; &#39;fr&#39; &#124; &#39;ja&#39; &#124; &#39;ru&#39; &#124; &#39;zh&#39; &#124; &#39;ko&#39; &#124; &#39;es&#39;>** | The language to use for the response. | (optional) defaults to 'en'|
| **ifNoneMatch** | [**string**] | The ETag of the previous request. A 304 will be returned if this matches the current ETag. | (optional) defaults to undefined|
| **xTenant** | [**string**] | The tenant ID for the request. | (optional) defaults to 'tranquility'|
| **ifModifiedSince** | [**string**] | The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. | (optional) defaults to undefined|


### Return type

**CharactersCharacterIdSearchGet**

### Authorization

[OAuth2](../README.md#OAuth2)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | OK |  * Cache-Control -  <br>  * Content-Language -  <br>  * ETag -  <br>  * Last-Modified -  <br>  |
|**0** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

