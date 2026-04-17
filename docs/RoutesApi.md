# RoutesApi

All URIs are relative to *https://esi.evetech.net*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**getRouteOriginDestination**](#getrouteorigindestination) | **GET** /route/{origin}/{destination} | Get route|

# **getRouteOriginDestination**
> Array<number> getRouteOriginDestination()

Get the systems between origin and destination

### Example

```typescript
import {
    RoutesApi,
    Configuration
} from 'eve-esi-client-ts';

const configuration = new Configuration();
const apiInstance = new RoutesApi(configuration);

let destination: number; // (default to undefined)
let origin: number; // (default to undefined)
let xCompatibilityDate: '2020-01-01'; //The compatibility date for the request. (default to undefined)
let avoid: Set<number>; // (optional) (default to undefined)
let connections: Set<Array<number>>; // (optional) (default to undefined)
let flag: 'shortest' | 'secure' | 'insecure'; // (optional) (default to 'shortest')
let acceptLanguage: 'en' | 'de' | 'fr' | 'ja' | 'ru' | 'zh' | 'ko' | 'es'; //The language to use for the response. (optional) (default to 'en')
let ifNoneMatch: string; //The ETag of the previous request. A 304 will be returned if this matches the current ETag. (optional) (default to undefined)
let xTenant: string; //The tenant ID for the request. (optional) (default to 'tranquility')
let ifModifiedSince: string; //The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. (optional) (default to undefined)

const { status, data } = await apiInstance.getRouteOriginDestination(
    destination,
    origin,
    xCompatibilityDate,
    avoid,
    connections,
    flag,
    acceptLanguage,
    ifNoneMatch,
    xTenant,
    ifModifiedSince
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **destination** | [**number**] |  | defaults to undefined|
| **origin** | [**number**] |  | defaults to undefined|
| **xCompatibilityDate** | [**&#39;2020-01-01&#39;**]**Array<&#39;2020-01-01&#39;>** | The compatibility date for the request. | defaults to undefined|
| **avoid** | **Set&lt;number&gt;** |  | (optional) defaults to undefined|
| **connections** | **Set&lt;Array&lt;number&gt;&gt;** |  | (optional) defaults to undefined|
| **flag** | [**&#39;shortest&#39; | &#39;secure&#39; | &#39;insecure&#39;**]**Array<&#39;shortest&#39; &#124; &#39;secure&#39; &#124; &#39;insecure&#39;>** |  | (optional) defaults to 'shortest'|
| **acceptLanguage** | [**&#39;en&#39; | &#39;de&#39; | &#39;fr&#39; | &#39;ja&#39; | &#39;ru&#39; | &#39;zh&#39; | &#39;ko&#39; | &#39;es&#39;**]**Array<&#39;en&#39; &#124; &#39;de&#39; &#124; &#39;fr&#39; &#124; &#39;ja&#39; &#124; &#39;ru&#39; &#124; &#39;zh&#39; &#124; &#39;ko&#39; &#124; &#39;es&#39;>** | The language to use for the response. | (optional) defaults to 'en'|
| **ifNoneMatch** | [**string**] | The ETag of the previous request. A 304 will be returned if this matches the current ETag. | (optional) defaults to undefined|
| **xTenant** | [**string**] | The tenant ID for the request. | (optional) defaults to 'tranquility'|
| **ifModifiedSince** | [**string**] | The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. | (optional) defaults to undefined|


### Return type

**Array<number>**

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

