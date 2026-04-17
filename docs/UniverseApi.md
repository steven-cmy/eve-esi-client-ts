# UniverseApi

All URIs are relative to *https://esi.evetech.net*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**getUniverseAncestries**](#getuniverseancestries) | **GET** /universe/ancestries | Get ancestries|
|[**getUniverseAsteroidBeltsAsteroidBeltId**](#getuniverseasteroidbeltsasteroidbeltid) | **GET** /universe/asteroid_belts/{asteroid_belt_id} | Get asteroid belt information|
|[**getUniverseBloodlines**](#getuniversebloodlines) | **GET** /universe/bloodlines | Get bloodlines|
|[**getUniverseCategories**](#getuniversecategories) | **GET** /universe/categories | Get item categories|
|[**getUniverseCategoriesCategoryId**](#getuniversecategoriescategoryid) | **GET** /universe/categories/{category_id} | Get item category information|
|[**getUniverseConstellations**](#getuniverseconstellations) | **GET** /universe/constellations | Get constellations|
|[**getUniverseConstellationsConstellationId**](#getuniverseconstellationsconstellationid) | **GET** /universe/constellations/{constellation_id} | Get constellation information|
|[**getUniverseFactions**](#getuniversefactions) | **GET** /universe/factions | Get factions|
|[**getUniverseGraphics**](#getuniversegraphics) | **GET** /universe/graphics | Get graphics|
|[**getUniverseGraphicsGraphicId**](#getuniversegraphicsgraphicid) | **GET** /universe/graphics/{graphic_id} | Get graphic information|
|[**getUniverseGroups**](#getuniversegroups) | **GET** /universe/groups | Get item groups|
|[**getUniverseGroupsGroupId**](#getuniversegroupsgroupid) | **GET** /universe/groups/{group_id} | Get item group information|
|[**getUniverseMoonsMoonId**](#getuniversemoonsmoonid) | **GET** /universe/moons/{moon_id} | Get moon information|
|[**getUniversePlanetsPlanetId**](#getuniverseplanetsplanetid) | **GET** /universe/planets/{planet_id} | Get planet information|
|[**getUniverseRaces**](#getuniverseraces) | **GET** /universe/races | Get character races|
|[**getUniverseRegions**](#getuniverseregions) | **GET** /universe/regions | Get regions|
|[**getUniverseRegionsRegionId**](#getuniverseregionsregionid) | **GET** /universe/regions/{region_id} | Get region information|
|[**getUniverseStargatesStargateId**](#getuniversestargatesstargateid) | **GET** /universe/stargates/{stargate_id} | Get stargate information|
|[**getUniverseStarsStarId**](#getuniversestarsstarid) | **GET** /universe/stars/{star_id} | Get star information|
|[**getUniverseStationsStationId**](#getuniversestationsstationid) | **GET** /universe/stations/{station_id} | Get station information|
|[**getUniverseStructures**](#getuniversestructures) | **GET** /universe/structures | List all public structures|
|[**getUniverseStructuresStructureId**](#getuniversestructuresstructureid) | **GET** /universe/structures/{structure_id} | Get structure information|
|[**getUniverseSystemJumps**](#getuniversesystemjumps) | **GET** /universe/system_jumps | Get system jumps|
|[**getUniverseSystemKills**](#getuniversesystemkills) | **GET** /universe/system_kills | Get system kills|
|[**getUniverseSystems**](#getuniversesystems) | **GET** /universe/systems | Get solar systems|
|[**getUniverseSystemsSystemId**](#getuniversesystemssystemid) | **GET** /universe/systems/{system_id} | Get solar system information|
|[**getUniverseTypes**](#getuniversetypes) | **GET** /universe/types | Get types|
|[**getUniverseTypesTypeId**](#getuniversetypestypeid) | **GET** /universe/types/{type_id} | Get type information|
|[**postUniverseIds**](#postuniverseids) | **POST** /universe/ids | Bulk names to IDs|
|[**postUniverseNames**](#postuniversenames) | **POST** /universe/names | Get names and categories for a set of IDs|

# **getUniverseAncestries**
> Array<UniverseAncestriesGetInner> getUniverseAncestries()

Get all character ancestries  This route expires daily at 11:05

### Example

```typescript
import {
    UniverseApi,
    Configuration
} from 'eve-esi-client-ts';

const configuration = new Configuration();
const apiInstance = new UniverseApi(configuration);

let xCompatibilityDate: '2025-12-16'; //The compatibility date for the request. (default to undefined)
let acceptLanguage: 'en' | 'de' | 'fr' | 'ja' | 'ru' | 'zh' | 'ko' | 'es'; //The language to use for the response. (optional) (default to 'en')
let ifNoneMatch: string; //The ETag of the previous request. A 304 will be returned if this matches the current ETag. (optional) (default to undefined)
let xTenant: string; //The tenant ID for the request. (optional) (default to 'tranquility')
let ifModifiedSince: string; //The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. (optional) (default to undefined)

const { status, data } = await apiInstance.getUniverseAncestries(
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
| **xCompatibilityDate** | [**&#39;2025-12-16&#39;**]**Array<&#39;2025-12-16&#39;>** | The compatibility date for the request. | defaults to undefined|
| **acceptLanguage** | [**&#39;en&#39; | &#39;de&#39; | &#39;fr&#39; | &#39;ja&#39; | &#39;ru&#39; | &#39;zh&#39; | &#39;ko&#39; | &#39;es&#39;**]**Array<&#39;en&#39; &#124; &#39;de&#39; &#124; &#39;fr&#39; &#124; &#39;ja&#39; &#124; &#39;ru&#39; &#124; &#39;zh&#39; &#124; &#39;ko&#39; &#124; &#39;es&#39;>** | The language to use for the response. | (optional) defaults to 'en'|
| **ifNoneMatch** | [**string**] | The ETag of the previous request. A 304 will be returned if this matches the current ETag. | (optional) defaults to undefined|
| **xTenant** | [**string**] | The tenant ID for the request. | (optional) defaults to 'tranquility'|
| **ifModifiedSince** | [**string**] | The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. | (optional) defaults to undefined|


### Return type

**Array<UniverseAncestriesGetInner>**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | OK |  * Cache-Control -  <br>  * Content-Language -  <br>  * ETag -  <br>  * Last-Modified -  <br>  |
|**0** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getUniverseAsteroidBeltsAsteroidBeltId**
> UniverseAsteroidBeltsAsteroidBeltIdGet getUniverseAsteroidBeltsAsteroidBeltId()

Get information on an asteroid belt  This route expires daily at 11:05

### Example

```typescript
import {
    UniverseApi,
    Configuration
} from 'eve-esi-client-ts';

const configuration = new Configuration();
const apiInstance = new UniverseApi(configuration);

let asteroidBeltId: number; // (default to undefined)
let xCompatibilityDate: '2025-12-16'; //The compatibility date for the request. (default to undefined)
let acceptLanguage: 'en' | 'de' | 'fr' | 'ja' | 'ru' | 'zh' | 'ko' | 'es'; //The language to use for the response. (optional) (default to 'en')
let ifNoneMatch: string; //The ETag of the previous request. A 304 will be returned if this matches the current ETag. (optional) (default to undefined)
let xTenant: string; //The tenant ID for the request. (optional) (default to 'tranquility')
let ifModifiedSince: string; //The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. (optional) (default to undefined)

const { status, data } = await apiInstance.getUniverseAsteroidBeltsAsteroidBeltId(
    asteroidBeltId,
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
| **asteroidBeltId** | [**number**] |  | defaults to undefined|
| **xCompatibilityDate** | [**&#39;2025-12-16&#39;**]**Array<&#39;2025-12-16&#39;>** | The compatibility date for the request. | defaults to undefined|
| **acceptLanguage** | [**&#39;en&#39; | &#39;de&#39; | &#39;fr&#39; | &#39;ja&#39; | &#39;ru&#39; | &#39;zh&#39; | &#39;ko&#39; | &#39;es&#39;**]**Array<&#39;en&#39; &#124; &#39;de&#39; &#124; &#39;fr&#39; &#124; &#39;ja&#39; &#124; &#39;ru&#39; &#124; &#39;zh&#39; &#124; &#39;ko&#39; &#124; &#39;es&#39;>** | The language to use for the response. | (optional) defaults to 'en'|
| **ifNoneMatch** | [**string**] | The ETag of the previous request. A 304 will be returned if this matches the current ETag. | (optional) defaults to undefined|
| **xTenant** | [**string**] | The tenant ID for the request. | (optional) defaults to 'tranquility'|
| **ifModifiedSince** | [**string**] | The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. | (optional) defaults to undefined|


### Return type

**UniverseAsteroidBeltsAsteroidBeltIdGet**

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

# **getUniverseBloodlines**
> Array<UniverseBloodlinesGetInner> getUniverseBloodlines()

Get a list of bloodlines  This route expires daily at 11:05

### Example

```typescript
import {
    UniverseApi,
    Configuration
} from 'eve-esi-client-ts';

const configuration = new Configuration();
const apiInstance = new UniverseApi(configuration);

let xCompatibilityDate: '2025-12-16'; //The compatibility date for the request. (default to undefined)
let acceptLanguage: 'en' | 'de' | 'fr' | 'ja' | 'ru' | 'zh' | 'ko' | 'es'; //The language to use for the response. (optional) (default to 'en')
let ifNoneMatch: string; //The ETag of the previous request. A 304 will be returned if this matches the current ETag. (optional) (default to undefined)
let xTenant: string; //The tenant ID for the request. (optional) (default to 'tranquility')
let ifModifiedSince: string; //The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. (optional) (default to undefined)

const { status, data } = await apiInstance.getUniverseBloodlines(
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
| **xCompatibilityDate** | [**&#39;2025-12-16&#39;**]**Array<&#39;2025-12-16&#39;>** | The compatibility date for the request. | defaults to undefined|
| **acceptLanguage** | [**&#39;en&#39; | &#39;de&#39; | &#39;fr&#39; | &#39;ja&#39; | &#39;ru&#39; | &#39;zh&#39; | &#39;ko&#39; | &#39;es&#39;**]**Array<&#39;en&#39; &#124; &#39;de&#39; &#124; &#39;fr&#39; &#124; &#39;ja&#39; &#124; &#39;ru&#39; &#124; &#39;zh&#39; &#124; &#39;ko&#39; &#124; &#39;es&#39;>** | The language to use for the response. | (optional) defaults to 'en'|
| **ifNoneMatch** | [**string**] | The ETag of the previous request. A 304 will be returned if this matches the current ETag. | (optional) defaults to undefined|
| **xTenant** | [**string**] | The tenant ID for the request. | (optional) defaults to 'tranquility'|
| **ifModifiedSince** | [**string**] | The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. | (optional) defaults to undefined|


### Return type

**Array<UniverseBloodlinesGetInner>**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | OK |  * Cache-Control -  <br>  * Content-Language -  <br>  * ETag -  <br>  * Last-Modified -  <br>  |
|**0** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getUniverseCategories**
> Array<number> getUniverseCategories()

Get a list of item categories  This route expires daily at 11:05

### Example

```typescript
import {
    UniverseApi,
    Configuration
} from 'eve-esi-client-ts';

const configuration = new Configuration();
const apiInstance = new UniverseApi(configuration);

let xCompatibilityDate: '2025-12-16'; //The compatibility date for the request. (default to undefined)
let acceptLanguage: 'en' | 'de' | 'fr' | 'ja' | 'ru' | 'zh' | 'ko' | 'es'; //The language to use for the response. (optional) (default to 'en')
let ifNoneMatch: string; //The ETag of the previous request. A 304 will be returned if this matches the current ETag. (optional) (default to undefined)
let xTenant: string; //The tenant ID for the request. (optional) (default to 'tranquility')
let ifModifiedSince: string; //The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. (optional) (default to undefined)

const { status, data } = await apiInstance.getUniverseCategories(
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
| **xCompatibilityDate** | [**&#39;2025-12-16&#39;**]**Array<&#39;2025-12-16&#39;>** | The compatibility date for the request. | defaults to undefined|
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

# **getUniverseCategoriesCategoryId**
> UniverseCategoriesCategoryIdGet getUniverseCategoriesCategoryId()

Get information of an item category  This route expires daily at 11:05

### Example

```typescript
import {
    UniverseApi,
    Configuration
} from 'eve-esi-client-ts';

const configuration = new Configuration();
const apiInstance = new UniverseApi(configuration);

let categoryId: number; // (default to undefined)
let xCompatibilityDate: '2025-12-16'; //The compatibility date for the request. (default to undefined)
let acceptLanguage: 'en' | 'de' | 'fr' | 'ja' | 'ru' | 'zh' | 'ko' | 'es'; //The language to use for the response. (optional) (default to 'en')
let ifNoneMatch: string; //The ETag of the previous request. A 304 will be returned if this matches the current ETag. (optional) (default to undefined)
let xTenant: string; //The tenant ID for the request. (optional) (default to 'tranquility')
let ifModifiedSince: string; //The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. (optional) (default to undefined)

const { status, data } = await apiInstance.getUniverseCategoriesCategoryId(
    categoryId,
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
| **categoryId** | [**number**] |  | defaults to undefined|
| **xCompatibilityDate** | [**&#39;2025-12-16&#39;**]**Array<&#39;2025-12-16&#39;>** | The compatibility date for the request. | defaults to undefined|
| **acceptLanguage** | [**&#39;en&#39; | &#39;de&#39; | &#39;fr&#39; | &#39;ja&#39; | &#39;ru&#39; | &#39;zh&#39; | &#39;ko&#39; | &#39;es&#39;**]**Array<&#39;en&#39; &#124; &#39;de&#39; &#124; &#39;fr&#39; &#124; &#39;ja&#39; &#124; &#39;ru&#39; &#124; &#39;zh&#39; &#124; &#39;ko&#39; &#124; &#39;es&#39;>** | The language to use for the response. | (optional) defaults to 'en'|
| **ifNoneMatch** | [**string**] | The ETag of the previous request. A 304 will be returned if this matches the current ETag. | (optional) defaults to undefined|
| **xTenant** | [**string**] | The tenant ID for the request. | (optional) defaults to 'tranquility'|
| **ifModifiedSince** | [**string**] | The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. | (optional) defaults to undefined|


### Return type

**UniverseCategoriesCategoryIdGet**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | OK |  * Cache-Control -  <br>  * Content-Language -  <br>  * ETag -  <br>  * Last-Modified -  <br>  |
|**0** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getUniverseConstellations**
> Array<number> getUniverseConstellations()

Get a list of constellations  This route expires daily at 11:05

### Example

```typescript
import {
    UniverseApi,
    Configuration
} from 'eve-esi-client-ts';

const configuration = new Configuration();
const apiInstance = new UniverseApi(configuration);

let xCompatibilityDate: '2025-12-16'; //The compatibility date for the request. (default to undefined)
let acceptLanguage: 'en' | 'de' | 'fr' | 'ja' | 'ru' | 'zh' | 'ko' | 'es'; //The language to use for the response. (optional) (default to 'en')
let ifNoneMatch: string; //The ETag of the previous request. A 304 will be returned if this matches the current ETag. (optional) (default to undefined)
let xTenant: string; //The tenant ID for the request. (optional) (default to 'tranquility')
let ifModifiedSince: string; //The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. (optional) (default to undefined)

const { status, data } = await apiInstance.getUniverseConstellations(
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
| **xCompatibilityDate** | [**&#39;2025-12-16&#39;**]**Array<&#39;2025-12-16&#39;>** | The compatibility date for the request. | defaults to undefined|
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

# **getUniverseConstellationsConstellationId**
> UniverseConstellationsConstellationIdGet getUniverseConstellationsConstellationId()

Get information on a constellation  This route expires daily at 11:05

### Example

```typescript
import {
    UniverseApi,
    Configuration
} from 'eve-esi-client-ts';

const configuration = new Configuration();
const apiInstance = new UniverseApi(configuration);

let constellationId: number; // (default to undefined)
let xCompatibilityDate: '2025-12-16'; //The compatibility date for the request. (default to undefined)
let acceptLanguage: 'en' | 'de' | 'fr' | 'ja' | 'ru' | 'zh' | 'ko' | 'es'; //The language to use for the response. (optional) (default to 'en')
let ifNoneMatch: string; //The ETag of the previous request. A 304 will be returned if this matches the current ETag. (optional) (default to undefined)
let xTenant: string; //The tenant ID for the request. (optional) (default to 'tranquility')
let ifModifiedSince: string; //The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. (optional) (default to undefined)

const { status, data } = await apiInstance.getUniverseConstellationsConstellationId(
    constellationId,
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
| **constellationId** | [**number**] |  | defaults to undefined|
| **xCompatibilityDate** | [**&#39;2025-12-16&#39;**]**Array<&#39;2025-12-16&#39;>** | The compatibility date for the request. | defaults to undefined|
| **acceptLanguage** | [**&#39;en&#39; | &#39;de&#39; | &#39;fr&#39; | &#39;ja&#39; | &#39;ru&#39; | &#39;zh&#39; | &#39;ko&#39; | &#39;es&#39;**]**Array<&#39;en&#39; &#124; &#39;de&#39; &#124; &#39;fr&#39; &#124; &#39;ja&#39; &#124; &#39;ru&#39; &#124; &#39;zh&#39; &#124; &#39;ko&#39; &#124; &#39;es&#39;>** | The language to use for the response. | (optional) defaults to 'en'|
| **ifNoneMatch** | [**string**] | The ETag of the previous request. A 304 will be returned if this matches the current ETag. | (optional) defaults to undefined|
| **xTenant** | [**string**] | The tenant ID for the request. | (optional) defaults to 'tranquility'|
| **ifModifiedSince** | [**string**] | The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. | (optional) defaults to undefined|


### Return type

**UniverseConstellationsConstellationIdGet**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | OK |  * Cache-Control -  <br>  * Content-Language -  <br>  * ETag -  <br>  * Last-Modified -  <br>  |
|**0** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getUniverseFactions**
> Array<UniverseFactionsGetInner> getUniverseFactions()

Get a list of factions  This route expires daily at 11:05

### Example

```typescript
import {
    UniverseApi,
    Configuration
} from 'eve-esi-client-ts';

const configuration = new Configuration();
const apiInstance = new UniverseApi(configuration);

let xCompatibilityDate: '2025-12-16'; //The compatibility date for the request. (default to undefined)
let acceptLanguage: 'en' | 'de' | 'fr' | 'ja' | 'ru' | 'zh' | 'ko' | 'es'; //The language to use for the response. (optional) (default to 'en')
let ifNoneMatch: string; //The ETag of the previous request. A 304 will be returned if this matches the current ETag. (optional) (default to undefined)
let xTenant: string; //The tenant ID for the request. (optional) (default to 'tranquility')
let ifModifiedSince: string; //The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. (optional) (default to undefined)

const { status, data } = await apiInstance.getUniverseFactions(
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
| **xCompatibilityDate** | [**&#39;2025-12-16&#39;**]**Array<&#39;2025-12-16&#39;>** | The compatibility date for the request. | defaults to undefined|
| **acceptLanguage** | [**&#39;en&#39; | &#39;de&#39; | &#39;fr&#39; | &#39;ja&#39; | &#39;ru&#39; | &#39;zh&#39; | &#39;ko&#39; | &#39;es&#39;**]**Array<&#39;en&#39; &#124; &#39;de&#39; &#124; &#39;fr&#39; &#124; &#39;ja&#39; &#124; &#39;ru&#39; &#124; &#39;zh&#39; &#124; &#39;ko&#39; &#124; &#39;es&#39;>** | The language to use for the response. | (optional) defaults to 'en'|
| **ifNoneMatch** | [**string**] | The ETag of the previous request. A 304 will be returned if this matches the current ETag. | (optional) defaults to undefined|
| **xTenant** | [**string**] | The tenant ID for the request. | (optional) defaults to 'tranquility'|
| **ifModifiedSince** | [**string**] | The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. | (optional) defaults to undefined|


### Return type

**Array<UniverseFactionsGetInner>**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | OK |  * Cache-Control -  <br>  * Content-Language -  <br>  * ETag -  <br>  * Last-Modified -  <br>  |
|**0** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getUniverseGraphics**
> Array<number> getUniverseGraphics()

Get a list of graphics  This route expires daily at 11:05

### Example

```typescript
import {
    UniverseApi,
    Configuration
} from 'eve-esi-client-ts';

const configuration = new Configuration();
const apiInstance = new UniverseApi(configuration);

let xCompatibilityDate: '2025-12-16'; //The compatibility date for the request. (default to undefined)
let acceptLanguage: 'en' | 'de' | 'fr' | 'ja' | 'ru' | 'zh' | 'ko' | 'es'; //The language to use for the response. (optional) (default to 'en')
let ifNoneMatch: string; //The ETag of the previous request. A 304 will be returned if this matches the current ETag. (optional) (default to undefined)
let xTenant: string; //The tenant ID for the request. (optional) (default to 'tranquility')
let ifModifiedSince: string; //The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. (optional) (default to undefined)

const { status, data } = await apiInstance.getUniverseGraphics(
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
| **xCompatibilityDate** | [**&#39;2025-12-16&#39;**]**Array<&#39;2025-12-16&#39;>** | The compatibility date for the request. | defaults to undefined|
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

# **getUniverseGraphicsGraphicId**
> UniverseGraphicsGraphicIdGet getUniverseGraphicsGraphicId()

Get information on a graphic  This route expires daily at 11:05

### Example

```typescript
import {
    UniverseApi,
    Configuration
} from 'eve-esi-client-ts';

const configuration = new Configuration();
const apiInstance = new UniverseApi(configuration);

let graphicId: number; // (default to undefined)
let xCompatibilityDate: '2025-12-16'; //The compatibility date for the request. (default to undefined)
let acceptLanguage: 'en' | 'de' | 'fr' | 'ja' | 'ru' | 'zh' | 'ko' | 'es'; //The language to use for the response. (optional) (default to 'en')
let ifNoneMatch: string; //The ETag of the previous request. A 304 will be returned if this matches the current ETag. (optional) (default to undefined)
let xTenant: string; //The tenant ID for the request. (optional) (default to 'tranquility')
let ifModifiedSince: string; //The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. (optional) (default to undefined)

const { status, data } = await apiInstance.getUniverseGraphicsGraphicId(
    graphicId,
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
| **graphicId** | [**number**] |  | defaults to undefined|
| **xCompatibilityDate** | [**&#39;2025-12-16&#39;**]**Array<&#39;2025-12-16&#39;>** | The compatibility date for the request. | defaults to undefined|
| **acceptLanguage** | [**&#39;en&#39; | &#39;de&#39; | &#39;fr&#39; | &#39;ja&#39; | &#39;ru&#39; | &#39;zh&#39; | &#39;ko&#39; | &#39;es&#39;**]**Array<&#39;en&#39; &#124; &#39;de&#39; &#124; &#39;fr&#39; &#124; &#39;ja&#39; &#124; &#39;ru&#39; &#124; &#39;zh&#39; &#124; &#39;ko&#39; &#124; &#39;es&#39;>** | The language to use for the response. | (optional) defaults to 'en'|
| **ifNoneMatch** | [**string**] | The ETag of the previous request. A 304 will be returned if this matches the current ETag. | (optional) defaults to undefined|
| **xTenant** | [**string**] | The tenant ID for the request. | (optional) defaults to 'tranquility'|
| **ifModifiedSince** | [**string**] | The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. | (optional) defaults to undefined|


### Return type

**UniverseGraphicsGraphicIdGet**

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

# **getUniverseGroups**
> Array<number> getUniverseGroups()

Get a list of item groups  This route expires daily at 11:05

### Example

```typescript
import {
    UniverseApi,
    Configuration
} from 'eve-esi-client-ts';

const configuration = new Configuration();
const apiInstance = new UniverseApi(configuration);

let xCompatibilityDate: '2025-12-16'; //The compatibility date for the request. (default to undefined)
let page: number; // (optional) (default to undefined)
let acceptLanguage: 'en' | 'de' | 'fr' | 'ja' | 'ru' | 'zh' | 'ko' | 'es'; //The language to use for the response. (optional) (default to 'en')
let ifNoneMatch: string; //The ETag of the previous request. A 304 will be returned if this matches the current ETag. (optional) (default to undefined)
let xTenant: string; //The tenant ID for the request. (optional) (default to 'tranquility')
let ifModifiedSince: string; //The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. (optional) (default to undefined)

const { status, data } = await apiInstance.getUniverseGroups(
    xCompatibilityDate,
    page,
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
| **page** | [**number**] |  | (optional) defaults to undefined|
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
|**200** | OK |  * Cache-Control -  <br>  * ETag -  <br>  * Last-Modified -  <br>  * X-Pages - The total number of pages in the result set. <br>  |
|**0** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getUniverseGroupsGroupId**
> UniverseGroupsGroupIdGet getUniverseGroupsGroupId()

Get information on an item group  This route expires daily at 11:05

### Example

```typescript
import {
    UniverseApi,
    Configuration
} from 'eve-esi-client-ts';

const configuration = new Configuration();
const apiInstance = new UniverseApi(configuration);

let groupId: number; // (default to undefined)
let xCompatibilityDate: '2025-12-16'; //The compatibility date for the request. (default to undefined)
let acceptLanguage: 'en' | 'de' | 'fr' | 'ja' | 'ru' | 'zh' | 'ko' | 'es'; //The language to use for the response. (optional) (default to 'en')
let ifNoneMatch: string; //The ETag of the previous request. A 304 will be returned if this matches the current ETag. (optional) (default to undefined)
let xTenant: string; //The tenant ID for the request. (optional) (default to 'tranquility')
let ifModifiedSince: string; //The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. (optional) (default to undefined)

const { status, data } = await apiInstance.getUniverseGroupsGroupId(
    groupId,
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
| **groupId** | [**number**] |  | defaults to undefined|
| **xCompatibilityDate** | [**&#39;2025-12-16&#39;**]**Array<&#39;2025-12-16&#39;>** | The compatibility date for the request. | defaults to undefined|
| **acceptLanguage** | [**&#39;en&#39; | &#39;de&#39; | &#39;fr&#39; | &#39;ja&#39; | &#39;ru&#39; | &#39;zh&#39; | &#39;ko&#39; | &#39;es&#39;**]**Array<&#39;en&#39; &#124; &#39;de&#39; &#124; &#39;fr&#39; &#124; &#39;ja&#39; &#124; &#39;ru&#39; &#124; &#39;zh&#39; &#124; &#39;ko&#39; &#124; &#39;es&#39;>** | The language to use for the response. | (optional) defaults to 'en'|
| **ifNoneMatch** | [**string**] | The ETag of the previous request. A 304 will be returned if this matches the current ETag. | (optional) defaults to undefined|
| **xTenant** | [**string**] | The tenant ID for the request. | (optional) defaults to 'tranquility'|
| **ifModifiedSince** | [**string**] | The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. | (optional) defaults to undefined|


### Return type

**UniverseGroupsGroupIdGet**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | OK |  * Cache-Control -  <br>  * Content-Language -  <br>  * ETag -  <br>  * Last-Modified -  <br>  |
|**0** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getUniverseMoonsMoonId**
> UniverseMoonsMoonIdGet getUniverseMoonsMoonId()

Get information on a moon  This route expires daily at 11:05

### Example

```typescript
import {
    UniverseApi,
    Configuration
} from 'eve-esi-client-ts';

const configuration = new Configuration();
const apiInstance = new UniverseApi(configuration);

let moonId: number; // (default to undefined)
let xCompatibilityDate: '2025-12-16'; //The compatibility date for the request. (default to undefined)
let acceptLanguage: 'en' | 'de' | 'fr' | 'ja' | 'ru' | 'zh' | 'ko' | 'es'; //The language to use for the response. (optional) (default to 'en')
let ifNoneMatch: string; //The ETag of the previous request. A 304 will be returned if this matches the current ETag. (optional) (default to undefined)
let xTenant: string; //The tenant ID for the request. (optional) (default to 'tranquility')
let ifModifiedSince: string; //The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. (optional) (default to undefined)

const { status, data } = await apiInstance.getUniverseMoonsMoonId(
    moonId,
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
| **moonId** | [**number**] |  | defaults to undefined|
| **xCompatibilityDate** | [**&#39;2025-12-16&#39;**]**Array<&#39;2025-12-16&#39;>** | The compatibility date for the request. | defaults to undefined|
| **acceptLanguage** | [**&#39;en&#39; | &#39;de&#39; | &#39;fr&#39; | &#39;ja&#39; | &#39;ru&#39; | &#39;zh&#39; | &#39;ko&#39; | &#39;es&#39;**]**Array<&#39;en&#39; &#124; &#39;de&#39; &#124; &#39;fr&#39; &#124; &#39;ja&#39; &#124; &#39;ru&#39; &#124; &#39;zh&#39; &#124; &#39;ko&#39; &#124; &#39;es&#39;>** | The language to use for the response. | (optional) defaults to 'en'|
| **ifNoneMatch** | [**string**] | The ETag of the previous request. A 304 will be returned if this matches the current ETag. | (optional) defaults to undefined|
| **xTenant** | [**string**] | The tenant ID for the request. | (optional) defaults to 'tranquility'|
| **ifModifiedSince** | [**string**] | The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. | (optional) defaults to undefined|


### Return type

**UniverseMoonsMoonIdGet**

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

# **getUniversePlanetsPlanetId**
> UniversePlanetsPlanetIdGet getUniversePlanetsPlanetId()

Get information on a planet  This route expires daily at 11:05

### Example

```typescript
import {
    UniverseApi,
    Configuration
} from 'eve-esi-client-ts';

const configuration = new Configuration();
const apiInstance = new UniverseApi(configuration);

let planetId: number; // (default to undefined)
let xCompatibilityDate: '2025-12-16'; //The compatibility date for the request. (default to undefined)
let acceptLanguage: 'en' | 'de' | 'fr' | 'ja' | 'ru' | 'zh' | 'ko' | 'es'; //The language to use for the response. (optional) (default to 'en')
let ifNoneMatch: string; //The ETag of the previous request. A 304 will be returned if this matches the current ETag. (optional) (default to undefined)
let xTenant: string; //The tenant ID for the request. (optional) (default to 'tranquility')
let ifModifiedSince: string; //The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. (optional) (default to undefined)

const { status, data } = await apiInstance.getUniversePlanetsPlanetId(
    planetId,
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
| **planetId** | [**number**] |  | defaults to undefined|
| **xCompatibilityDate** | [**&#39;2025-12-16&#39;**]**Array<&#39;2025-12-16&#39;>** | The compatibility date for the request. | defaults to undefined|
| **acceptLanguage** | [**&#39;en&#39; | &#39;de&#39; | &#39;fr&#39; | &#39;ja&#39; | &#39;ru&#39; | &#39;zh&#39; | &#39;ko&#39; | &#39;es&#39;**]**Array<&#39;en&#39; &#124; &#39;de&#39; &#124; &#39;fr&#39; &#124; &#39;ja&#39; &#124; &#39;ru&#39; &#124; &#39;zh&#39; &#124; &#39;ko&#39; &#124; &#39;es&#39;>** | The language to use for the response. | (optional) defaults to 'en'|
| **ifNoneMatch** | [**string**] | The ETag of the previous request. A 304 will be returned if this matches the current ETag. | (optional) defaults to undefined|
| **xTenant** | [**string**] | The tenant ID for the request. | (optional) defaults to 'tranquility'|
| **ifModifiedSince** | [**string**] | The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. | (optional) defaults to undefined|


### Return type

**UniversePlanetsPlanetIdGet**

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

# **getUniverseRaces**
> Array<UniverseRacesGetInner> getUniverseRaces()

Get a list of character races  This route expires daily at 11:05

### Example

```typescript
import {
    UniverseApi,
    Configuration
} from 'eve-esi-client-ts';

const configuration = new Configuration();
const apiInstance = new UniverseApi(configuration);

let xCompatibilityDate: '2025-12-16'; //The compatibility date for the request. (default to undefined)
let acceptLanguage: 'en' | 'de' | 'fr' | 'ja' | 'ru' | 'zh' | 'ko' | 'es'; //The language to use for the response. (optional) (default to 'en')
let ifNoneMatch: string; //The ETag of the previous request. A 304 will be returned if this matches the current ETag. (optional) (default to undefined)
let xTenant: string; //The tenant ID for the request. (optional) (default to 'tranquility')
let ifModifiedSince: string; //The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. (optional) (default to undefined)

const { status, data } = await apiInstance.getUniverseRaces(
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
| **xCompatibilityDate** | [**&#39;2025-12-16&#39;**]**Array<&#39;2025-12-16&#39;>** | The compatibility date for the request. | defaults to undefined|
| **acceptLanguage** | [**&#39;en&#39; | &#39;de&#39; | &#39;fr&#39; | &#39;ja&#39; | &#39;ru&#39; | &#39;zh&#39; | &#39;ko&#39; | &#39;es&#39;**]**Array<&#39;en&#39; &#124; &#39;de&#39; &#124; &#39;fr&#39; &#124; &#39;ja&#39; &#124; &#39;ru&#39; &#124; &#39;zh&#39; &#124; &#39;ko&#39; &#124; &#39;es&#39;>** | The language to use for the response. | (optional) defaults to 'en'|
| **ifNoneMatch** | [**string**] | The ETag of the previous request. A 304 will be returned if this matches the current ETag. | (optional) defaults to undefined|
| **xTenant** | [**string**] | The tenant ID for the request. | (optional) defaults to 'tranquility'|
| **ifModifiedSince** | [**string**] | The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. | (optional) defaults to undefined|


### Return type

**Array<UniverseRacesGetInner>**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | OK |  * Cache-Control -  <br>  * Content-Language -  <br>  * ETag -  <br>  * Last-Modified -  <br>  |
|**0** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getUniverseRegions**
> Array<number> getUniverseRegions()

Get a list of regions  This route expires daily at 11:05

### Example

```typescript
import {
    UniverseApi,
    Configuration
} from 'eve-esi-client-ts';

const configuration = new Configuration();
const apiInstance = new UniverseApi(configuration);

let xCompatibilityDate: '2025-12-16'; //The compatibility date for the request. (default to undefined)
let acceptLanguage: 'en' | 'de' | 'fr' | 'ja' | 'ru' | 'zh' | 'ko' | 'es'; //The language to use for the response. (optional) (default to 'en')
let ifNoneMatch: string; //The ETag of the previous request. A 304 will be returned if this matches the current ETag. (optional) (default to undefined)
let xTenant: string; //The tenant ID for the request. (optional) (default to 'tranquility')
let ifModifiedSince: string; //The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. (optional) (default to undefined)

const { status, data } = await apiInstance.getUniverseRegions(
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
| **xCompatibilityDate** | [**&#39;2025-12-16&#39;**]**Array<&#39;2025-12-16&#39;>** | The compatibility date for the request. | defaults to undefined|
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

# **getUniverseRegionsRegionId**
> UniverseRegionsRegionIdGet getUniverseRegionsRegionId()

Get information on a region  This route expires daily at 11:05

### Example

```typescript
import {
    UniverseApi,
    Configuration
} from 'eve-esi-client-ts';

const configuration = new Configuration();
const apiInstance = new UniverseApi(configuration);

let regionId: number; // (default to undefined)
let xCompatibilityDate: '2025-12-16'; //The compatibility date for the request. (default to undefined)
let acceptLanguage: 'en' | 'de' | 'fr' | 'ja' | 'ru' | 'zh' | 'ko' | 'es'; //The language to use for the response. (optional) (default to 'en')
let ifNoneMatch: string; //The ETag of the previous request. A 304 will be returned if this matches the current ETag. (optional) (default to undefined)
let xTenant: string; //The tenant ID for the request. (optional) (default to 'tranquility')
let ifModifiedSince: string; //The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. (optional) (default to undefined)

const { status, data } = await apiInstance.getUniverseRegionsRegionId(
    regionId,
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
| **regionId** | [**number**] |  | defaults to undefined|
| **xCompatibilityDate** | [**&#39;2025-12-16&#39;**]**Array<&#39;2025-12-16&#39;>** | The compatibility date for the request. | defaults to undefined|
| **acceptLanguage** | [**&#39;en&#39; | &#39;de&#39; | &#39;fr&#39; | &#39;ja&#39; | &#39;ru&#39; | &#39;zh&#39; | &#39;ko&#39; | &#39;es&#39;**]**Array<&#39;en&#39; &#124; &#39;de&#39; &#124; &#39;fr&#39; &#124; &#39;ja&#39; &#124; &#39;ru&#39; &#124; &#39;zh&#39; &#124; &#39;ko&#39; &#124; &#39;es&#39;>** | The language to use for the response. | (optional) defaults to 'en'|
| **ifNoneMatch** | [**string**] | The ETag of the previous request. A 304 will be returned if this matches the current ETag. | (optional) defaults to undefined|
| **xTenant** | [**string**] | The tenant ID for the request. | (optional) defaults to 'tranquility'|
| **ifModifiedSince** | [**string**] | The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. | (optional) defaults to undefined|


### Return type

**UniverseRegionsRegionIdGet**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | OK |  * Cache-Control -  <br>  * Content-Language -  <br>  * ETag -  <br>  * Last-Modified -  <br>  |
|**0** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getUniverseStargatesStargateId**
> UniverseStargatesStargateIdGet getUniverseStargatesStargateId()

Get information on a stargate  This route expires daily at 11:05

### Example

```typescript
import {
    UniverseApi,
    Configuration
} from 'eve-esi-client-ts';

const configuration = new Configuration();
const apiInstance = new UniverseApi(configuration);

let stargateId: number; // (default to undefined)
let xCompatibilityDate: '2025-12-16'; //The compatibility date for the request. (default to undefined)
let acceptLanguage: 'en' | 'de' | 'fr' | 'ja' | 'ru' | 'zh' | 'ko' | 'es'; //The language to use for the response. (optional) (default to 'en')
let ifNoneMatch: string; //The ETag of the previous request. A 304 will be returned if this matches the current ETag. (optional) (default to undefined)
let xTenant: string; //The tenant ID for the request. (optional) (default to 'tranquility')
let ifModifiedSince: string; //The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. (optional) (default to undefined)

const { status, data } = await apiInstance.getUniverseStargatesStargateId(
    stargateId,
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
| **stargateId** | [**number**] |  | defaults to undefined|
| **xCompatibilityDate** | [**&#39;2025-12-16&#39;**]**Array<&#39;2025-12-16&#39;>** | The compatibility date for the request. | defaults to undefined|
| **acceptLanguage** | [**&#39;en&#39; | &#39;de&#39; | &#39;fr&#39; | &#39;ja&#39; | &#39;ru&#39; | &#39;zh&#39; | &#39;ko&#39; | &#39;es&#39;**]**Array<&#39;en&#39; &#124; &#39;de&#39; &#124; &#39;fr&#39; &#124; &#39;ja&#39; &#124; &#39;ru&#39; &#124; &#39;zh&#39; &#124; &#39;ko&#39; &#124; &#39;es&#39;>** | The language to use for the response. | (optional) defaults to 'en'|
| **ifNoneMatch** | [**string**] | The ETag of the previous request. A 304 will be returned if this matches the current ETag. | (optional) defaults to undefined|
| **xTenant** | [**string**] | The tenant ID for the request. | (optional) defaults to 'tranquility'|
| **ifModifiedSince** | [**string**] | The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. | (optional) defaults to undefined|


### Return type

**UniverseStargatesStargateIdGet**

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

# **getUniverseStarsStarId**
> UniverseStarsStarIdGet getUniverseStarsStarId()

Get information on a star  This route expires daily at 11:05

### Example

```typescript
import {
    UniverseApi,
    Configuration
} from 'eve-esi-client-ts';

const configuration = new Configuration();
const apiInstance = new UniverseApi(configuration);

let starId: number; // (default to undefined)
let xCompatibilityDate: '2025-12-16'; //The compatibility date for the request. (default to undefined)
let acceptLanguage: 'en' | 'de' | 'fr' | 'ja' | 'ru' | 'zh' | 'ko' | 'es'; //The language to use for the response. (optional) (default to 'en')
let ifNoneMatch: string; //The ETag of the previous request. A 304 will be returned if this matches the current ETag. (optional) (default to undefined)
let xTenant: string; //The tenant ID for the request. (optional) (default to 'tranquility')
let ifModifiedSince: string; //The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. (optional) (default to undefined)

const { status, data } = await apiInstance.getUniverseStarsStarId(
    starId,
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
| **starId** | [**number**] |  | defaults to undefined|
| **xCompatibilityDate** | [**&#39;2025-12-16&#39;**]**Array<&#39;2025-12-16&#39;>** | The compatibility date for the request. | defaults to undefined|
| **acceptLanguage** | [**&#39;en&#39; | &#39;de&#39; | &#39;fr&#39; | &#39;ja&#39; | &#39;ru&#39; | &#39;zh&#39; | &#39;ko&#39; | &#39;es&#39;**]**Array<&#39;en&#39; &#124; &#39;de&#39; &#124; &#39;fr&#39; &#124; &#39;ja&#39; &#124; &#39;ru&#39; &#124; &#39;zh&#39; &#124; &#39;ko&#39; &#124; &#39;es&#39;>** | The language to use for the response. | (optional) defaults to 'en'|
| **ifNoneMatch** | [**string**] | The ETag of the previous request. A 304 will be returned if this matches the current ETag. | (optional) defaults to undefined|
| **xTenant** | [**string**] | The tenant ID for the request. | (optional) defaults to 'tranquility'|
| **ifModifiedSince** | [**string**] | The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. | (optional) defaults to undefined|


### Return type

**UniverseStarsStarIdGet**

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

# **getUniverseStationsStationId**
> UniverseStationsStationIdGet getUniverseStationsStationId()

Get information on a station  This route expires daily at 11:05

### Example

```typescript
import {
    UniverseApi,
    Configuration
} from 'eve-esi-client-ts';

const configuration = new Configuration();
const apiInstance = new UniverseApi(configuration);

let stationId: number; // (default to undefined)
let xCompatibilityDate: '2025-12-16'; //The compatibility date for the request. (default to undefined)
let acceptLanguage: 'en' | 'de' | 'fr' | 'ja' | 'ru' | 'zh' | 'ko' | 'es'; //The language to use for the response. (optional) (default to 'en')
let ifNoneMatch: string; //The ETag of the previous request. A 304 will be returned if this matches the current ETag. (optional) (default to undefined)
let xTenant: string; //The tenant ID for the request. (optional) (default to 'tranquility')
let ifModifiedSince: string; //The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. (optional) (default to undefined)

const { status, data } = await apiInstance.getUniverseStationsStationId(
    stationId,
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
| **stationId** | [**number**] |  | defaults to undefined|
| **xCompatibilityDate** | [**&#39;2025-12-16&#39;**]**Array<&#39;2025-12-16&#39;>** | The compatibility date for the request. | defaults to undefined|
| **acceptLanguage** | [**&#39;en&#39; | &#39;de&#39; | &#39;fr&#39; | &#39;ja&#39; | &#39;ru&#39; | &#39;zh&#39; | &#39;ko&#39; | &#39;es&#39;**]**Array<&#39;en&#39; &#124; &#39;de&#39; &#124; &#39;fr&#39; &#124; &#39;ja&#39; &#124; &#39;ru&#39; &#124; &#39;zh&#39; &#124; &#39;ko&#39; &#124; &#39;es&#39;>** | The language to use for the response. | (optional) defaults to 'en'|
| **ifNoneMatch** | [**string**] | The ETag of the previous request. A 304 will be returned if this matches the current ETag. | (optional) defaults to undefined|
| **xTenant** | [**string**] | The tenant ID for the request. | (optional) defaults to 'tranquility'|
| **ifModifiedSince** | [**string**] | The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. | (optional) defaults to undefined|


### Return type

**UniverseStationsStationIdGet**

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

# **getUniverseStructures**
> Set<number> getUniverseStructures()

List all public structures

### Example

```typescript
import {
    UniverseApi,
    Configuration
} from 'eve-esi-client-ts';

const configuration = new Configuration();
const apiInstance = new UniverseApi(configuration);

let xCompatibilityDate: '2025-12-16'; //The compatibility date for the request. (default to undefined)
let filter: 'market' | 'manufacturing_basic'; // (optional) (default to undefined)
let acceptLanguage: 'en' | 'de' | 'fr' | 'ja' | 'ru' | 'zh' | 'ko' | 'es'; //The language to use for the response. (optional) (default to 'en')
let ifNoneMatch: string; //The ETag of the previous request. A 304 will be returned if this matches the current ETag. (optional) (default to undefined)
let xTenant: string; //The tenant ID for the request. (optional) (default to 'tranquility')
let ifModifiedSince: string; //The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. (optional) (default to undefined)

const { status, data } = await apiInstance.getUniverseStructures(
    xCompatibilityDate,
    filter,
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
| **filter** | [**&#39;market&#39; | &#39;manufacturing_basic&#39;**]**Array<&#39;market&#39; &#124; &#39;manufacturing_basic&#39;>** |  | (optional) defaults to undefined|
| **acceptLanguage** | [**&#39;en&#39; | &#39;de&#39; | &#39;fr&#39; | &#39;ja&#39; | &#39;ru&#39; | &#39;zh&#39; | &#39;ko&#39; | &#39;es&#39;**]**Array<&#39;en&#39; &#124; &#39;de&#39; &#124; &#39;fr&#39; &#124; &#39;ja&#39; &#124; &#39;ru&#39; &#124; &#39;zh&#39; &#124; &#39;ko&#39; &#124; &#39;es&#39;>** | The language to use for the response. | (optional) defaults to 'en'|
| **ifNoneMatch** | [**string**] | The ETag of the previous request. A 304 will be returned if this matches the current ETag. | (optional) defaults to undefined|
| **xTenant** | [**string**] | The tenant ID for the request. | (optional) defaults to 'tranquility'|
| **ifModifiedSince** | [**string**] | The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. | (optional) defaults to undefined|


### Return type

**Set<number>**

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

# **getUniverseStructuresStructureId**
> UniverseStructuresStructureIdGet getUniverseStructuresStructureId()

Returns information on requested structure if you are on the ACL. Otherwise, returns \"Forbidden\" for all inputs.

### Example

```typescript
import {
    UniverseApi,
    Configuration
} from 'eve-esi-client-ts';

const configuration = new Configuration();
const apiInstance = new UniverseApi(configuration);

let structureId: number; // (default to undefined)
let xCompatibilityDate: '2025-12-16'; //The compatibility date for the request. (default to undefined)
let acceptLanguage: 'en' | 'de' | 'fr' | 'ja' | 'ru' | 'zh' | 'ko' | 'es'; //The language to use for the response. (optional) (default to 'en')
let ifNoneMatch: string; //The ETag of the previous request. A 304 will be returned if this matches the current ETag. (optional) (default to undefined)
let xTenant: string; //The tenant ID for the request. (optional) (default to 'tranquility')
let ifModifiedSince: string; //The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. (optional) (default to undefined)

const { status, data } = await apiInstance.getUniverseStructuresStructureId(
    structureId,
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
| **structureId** | [**number**] |  | defaults to undefined|
| **xCompatibilityDate** | [**&#39;2025-12-16&#39;**]**Array<&#39;2025-12-16&#39;>** | The compatibility date for the request. | defaults to undefined|
| **acceptLanguage** | [**&#39;en&#39; | &#39;de&#39; | &#39;fr&#39; | &#39;ja&#39; | &#39;ru&#39; | &#39;zh&#39; | &#39;ko&#39; | &#39;es&#39;**]**Array<&#39;en&#39; &#124; &#39;de&#39; &#124; &#39;fr&#39; &#124; &#39;ja&#39; &#124; &#39;ru&#39; &#124; &#39;zh&#39; &#124; &#39;ko&#39; &#124; &#39;es&#39;>** | The language to use for the response. | (optional) defaults to 'en'|
| **ifNoneMatch** | [**string**] | The ETag of the previous request. A 304 will be returned if this matches the current ETag. | (optional) defaults to undefined|
| **xTenant** | [**string**] | The tenant ID for the request. | (optional) defaults to 'tranquility'|
| **ifModifiedSince** | [**string**] | The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. | (optional) defaults to undefined|


### Return type

**UniverseStructuresStructureIdGet**

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

# **getUniverseSystemJumps**
> Array<UniverseSystemJumpsGetInner> getUniverseSystemJumps()

Get the number of jumps in solar systems within the last hour ending at the timestamp of the Last-Modified header, excluding wormhole space. Only systems with jumps will be listed

### Example

```typescript
import {
    UniverseApi,
    Configuration
} from 'eve-esi-client-ts';

const configuration = new Configuration();
const apiInstance = new UniverseApi(configuration);

let xCompatibilityDate: '2025-12-16'; //The compatibility date for the request. (default to undefined)
let acceptLanguage: 'en' | 'de' | 'fr' | 'ja' | 'ru' | 'zh' | 'ko' | 'es'; //The language to use for the response. (optional) (default to 'en')
let ifNoneMatch: string; //The ETag of the previous request. A 304 will be returned if this matches the current ETag. (optional) (default to undefined)
let xTenant: string; //The tenant ID for the request. (optional) (default to 'tranquility')
let ifModifiedSince: string; //The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. (optional) (default to undefined)

const { status, data } = await apiInstance.getUniverseSystemJumps(
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
| **xCompatibilityDate** | [**&#39;2025-12-16&#39;**]**Array<&#39;2025-12-16&#39;>** | The compatibility date for the request. | defaults to undefined|
| **acceptLanguage** | [**&#39;en&#39; | &#39;de&#39; | &#39;fr&#39; | &#39;ja&#39; | &#39;ru&#39; | &#39;zh&#39; | &#39;ko&#39; | &#39;es&#39;**]**Array<&#39;en&#39; &#124; &#39;de&#39; &#124; &#39;fr&#39; &#124; &#39;ja&#39; &#124; &#39;ru&#39; &#124; &#39;zh&#39; &#124; &#39;ko&#39; &#124; &#39;es&#39;>** | The language to use for the response. | (optional) defaults to 'en'|
| **ifNoneMatch** | [**string**] | The ETag of the previous request. A 304 will be returned if this matches the current ETag. | (optional) defaults to undefined|
| **xTenant** | [**string**] | The tenant ID for the request. | (optional) defaults to 'tranquility'|
| **ifModifiedSince** | [**string**] | The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. | (optional) defaults to undefined|


### Return type

**Array<UniverseSystemJumpsGetInner>**

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

# **getUniverseSystemKills**
> Array<UniverseSystemKillsGetInner> getUniverseSystemKills()

Get the number of ship, pod and NPC kills per solar system within the last hour ending at the timestamp of the Last-Modified header, excluding wormhole space. Only systems with kills will be listed

### Example

```typescript
import {
    UniverseApi,
    Configuration
} from 'eve-esi-client-ts';

const configuration = new Configuration();
const apiInstance = new UniverseApi(configuration);

let xCompatibilityDate: '2025-12-16'; //The compatibility date for the request. (default to undefined)
let acceptLanguage: 'en' | 'de' | 'fr' | 'ja' | 'ru' | 'zh' | 'ko' | 'es'; //The language to use for the response. (optional) (default to 'en')
let ifNoneMatch: string; //The ETag of the previous request. A 304 will be returned if this matches the current ETag. (optional) (default to undefined)
let xTenant: string; //The tenant ID for the request. (optional) (default to 'tranquility')
let ifModifiedSince: string; //The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. (optional) (default to undefined)

const { status, data } = await apiInstance.getUniverseSystemKills(
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
| **xCompatibilityDate** | [**&#39;2025-12-16&#39;**]**Array<&#39;2025-12-16&#39;>** | The compatibility date for the request. | defaults to undefined|
| **acceptLanguage** | [**&#39;en&#39; | &#39;de&#39; | &#39;fr&#39; | &#39;ja&#39; | &#39;ru&#39; | &#39;zh&#39; | &#39;ko&#39; | &#39;es&#39;**]**Array<&#39;en&#39; &#124; &#39;de&#39; &#124; &#39;fr&#39; &#124; &#39;ja&#39; &#124; &#39;ru&#39; &#124; &#39;zh&#39; &#124; &#39;ko&#39; &#124; &#39;es&#39;>** | The language to use for the response. | (optional) defaults to 'en'|
| **ifNoneMatch** | [**string**] | The ETag of the previous request. A 304 will be returned if this matches the current ETag. | (optional) defaults to undefined|
| **xTenant** | [**string**] | The tenant ID for the request. | (optional) defaults to 'tranquility'|
| **ifModifiedSince** | [**string**] | The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. | (optional) defaults to undefined|


### Return type

**Array<UniverseSystemKillsGetInner>**

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

# **getUniverseSystems**
> Array<number> getUniverseSystems()

Get a list of solar systems  This route expires daily at 11:05

### Example

```typescript
import {
    UniverseApi,
    Configuration
} from 'eve-esi-client-ts';

const configuration = new Configuration();
const apiInstance = new UniverseApi(configuration);

let xCompatibilityDate: '2025-12-16'; //The compatibility date for the request. (default to undefined)
let acceptLanguage: 'en' | 'de' | 'fr' | 'ja' | 'ru' | 'zh' | 'ko' | 'es'; //The language to use for the response. (optional) (default to 'en')
let ifNoneMatch: string; //The ETag of the previous request. A 304 will be returned if this matches the current ETag. (optional) (default to undefined)
let xTenant: string; //The tenant ID for the request. (optional) (default to 'tranquility')
let ifModifiedSince: string; //The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. (optional) (default to undefined)

const { status, data } = await apiInstance.getUniverseSystems(
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
| **xCompatibilityDate** | [**&#39;2025-12-16&#39;**]**Array<&#39;2025-12-16&#39;>** | The compatibility date for the request. | defaults to undefined|
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

# **getUniverseSystemsSystemId**
> UniverseSystemsSystemIdGet getUniverseSystemsSystemId()

Get information on a solar system.  This route expires daily at 11:05

### Example

```typescript
import {
    UniverseApi,
    Configuration
} from 'eve-esi-client-ts';

const configuration = new Configuration();
const apiInstance = new UniverseApi(configuration);

let systemId: number; // (default to undefined)
let xCompatibilityDate: '2025-12-16'; //The compatibility date for the request. (default to undefined)
let acceptLanguage: 'en' | 'de' | 'fr' | 'ja' | 'ru' | 'zh' | 'ko' | 'es'; //The language to use for the response. (optional) (default to 'en')
let ifNoneMatch: string; //The ETag of the previous request. A 304 will be returned if this matches the current ETag. (optional) (default to undefined)
let xTenant: string; //The tenant ID for the request. (optional) (default to 'tranquility')
let ifModifiedSince: string; //The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. (optional) (default to undefined)

const { status, data } = await apiInstance.getUniverseSystemsSystemId(
    systemId,
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
| **systemId** | [**number**] |  | defaults to undefined|
| **xCompatibilityDate** | [**&#39;2025-12-16&#39;**]**Array<&#39;2025-12-16&#39;>** | The compatibility date for the request. | defaults to undefined|
| **acceptLanguage** | [**&#39;en&#39; | &#39;de&#39; | &#39;fr&#39; | &#39;ja&#39; | &#39;ru&#39; | &#39;zh&#39; | &#39;ko&#39; | &#39;es&#39;**]**Array<&#39;en&#39; &#124; &#39;de&#39; &#124; &#39;fr&#39; &#124; &#39;ja&#39; &#124; &#39;ru&#39; &#124; &#39;zh&#39; &#124; &#39;ko&#39; &#124; &#39;es&#39;>** | The language to use for the response. | (optional) defaults to 'en'|
| **ifNoneMatch** | [**string**] | The ETag of the previous request. A 304 will be returned if this matches the current ETag. | (optional) defaults to undefined|
| **xTenant** | [**string**] | The tenant ID for the request. | (optional) defaults to 'tranquility'|
| **ifModifiedSince** | [**string**] | The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. | (optional) defaults to undefined|


### Return type

**UniverseSystemsSystemIdGet**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | OK |  * Cache-Control -  <br>  * Content-Language -  <br>  * ETag -  <br>  * Last-Modified -  <br>  |
|**0** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getUniverseTypes**
> Array<number> getUniverseTypes()

Get a list of type ids  This route expires daily at 11:05

### Example

```typescript
import {
    UniverseApi,
    Configuration
} from 'eve-esi-client-ts';

const configuration = new Configuration();
const apiInstance = new UniverseApi(configuration);

let xCompatibilityDate: '2025-12-16'; //The compatibility date for the request. (default to undefined)
let page: number; // (optional) (default to undefined)
let acceptLanguage: 'en' | 'de' | 'fr' | 'ja' | 'ru' | 'zh' | 'ko' | 'es'; //The language to use for the response. (optional) (default to 'en')
let ifNoneMatch: string; //The ETag of the previous request. A 304 will be returned if this matches the current ETag. (optional) (default to undefined)
let xTenant: string; //The tenant ID for the request. (optional) (default to 'tranquility')
let ifModifiedSince: string; //The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. (optional) (default to undefined)

const { status, data } = await apiInstance.getUniverseTypes(
    xCompatibilityDate,
    page,
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
| **page** | [**number**] |  | (optional) defaults to undefined|
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
|**200** | OK |  * Cache-Control -  <br>  * ETag -  <br>  * Last-Modified -  <br>  * X-Pages - The total number of pages in the result set. <br>  |
|**0** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getUniverseTypesTypeId**
> UniverseTypesTypeIdGet getUniverseTypesTypeId()

Get information on a type  This route expires daily at 11:05

### Example

```typescript
import {
    UniverseApi,
    Configuration
} from 'eve-esi-client-ts';

const configuration = new Configuration();
const apiInstance = new UniverseApi(configuration);

let typeId: number; // (default to undefined)
let xCompatibilityDate: '2025-12-16'; //The compatibility date for the request. (default to undefined)
let acceptLanguage: 'en' | 'de' | 'fr' | 'ja' | 'ru' | 'zh' | 'ko' | 'es'; //The language to use for the response. (optional) (default to 'en')
let ifNoneMatch: string; //The ETag of the previous request. A 304 will be returned if this matches the current ETag. (optional) (default to undefined)
let xTenant: string; //The tenant ID for the request. (optional) (default to 'tranquility')
let ifModifiedSince: string; //The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. (optional) (default to undefined)

const { status, data } = await apiInstance.getUniverseTypesTypeId(
    typeId,
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
| **typeId** | [**number**] |  | defaults to undefined|
| **xCompatibilityDate** | [**&#39;2025-12-16&#39;**]**Array<&#39;2025-12-16&#39;>** | The compatibility date for the request. | defaults to undefined|
| **acceptLanguage** | [**&#39;en&#39; | &#39;de&#39; | &#39;fr&#39; | &#39;ja&#39; | &#39;ru&#39; | &#39;zh&#39; | &#39;ko&#39; | &#39;es&#39;**]**Array<&#39;en&#39; &#124; &#39;de&#39; &#124; &#39;fr&#39; &#124; &#39;ja&#39; &#124; &#39;ru&#39; &#124; &#39;zh&#39; &#124; &#39;ko&#39; &#124; &#39;es&#39;>** | The language to use for the response. | (optional) defaults to 'en'|
| **ifNoneMatch** | [**string**] | The ETag of the previous request. A 304 will be returned if this matches the current ETag. | (optional) defaults to undefined|
| **xTenant** | [**string**] | The tenant ID for the request. | (optional) defaults to 'tranquility'|
| **ifModifiedSince** | [**string**] | The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. | (optional) defaults to undefined|


### Return type

**UniverseTypesTypeIdGet**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | OK |  * Cache-Control -  <br>  * Content-Language -  <br>  * ETag -  <br>  * Last-Modified -  <br>  |
|**0** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **postUniverseIds**
> UniverseIdsPost postUniverseIds(requestBody)

Resolve a set of names to IDs in the following categories: agents, alliances, characters, constellations, corporations factions, inventory_types, regions, stations, and systems. Only exact matches will be returned. All names searched for are cached for 12 hours

### Example

```typescript
import {
    UniverseApi,
    Configuration
} from 'eve-esi-client-ts';

const configuration = new Configuration();
const apiInstance = new UniverseApi(configuration);

let xCompatibilityDate: '2025-12-16'; //The compatibility date for the request. (default to undefined)
let requestBody: Set<string>; //
let acceptLanguage: 'en' | 'de' | 'fr' | 'ja' | 'ru' | 'zh' | 'ko' | 'es'; //The language to use for the response. (optional) (default to 'en')
let ifNoneMatch: string; //The ETag of the previous request. A 304 will be returned if this matches the current ETag. (optional) (default to undefined)
let xTenant: string; //The tenant ID for the request. (optional) (default to 'tranquility')
let ifModifiedSince: string; //The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. (optional) (default to undefined)

const { status, data } = await apiInstance.postUniverseIds(
    xCompatibilityDate,
    requestBody,
    acceptLanguage,
    ifNoneMatch,
    xTenant,
    ifModifiedSince
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **requestBody** | **Set<string>**|  | |
| **xCompatibilityDate** | [**&#39;2025-12-16&#39;**]**Array<&#39;2025-12-16&#39;>** | The compatibility date for the request. | defaults to undefined|
| **acceptLanguage** | [**&#39;en&#39; | &#39;de&#39; | &#39;fr&#39; | &#39;ja&#39; | &#39;ru&#39; | &#39;zh&#39; | &#39;ko&#39; | &#39;es&#39;**]**Array<&#39;en&#39; &#124; &#39;de&#39; &#124; &#39;fr&#39; &#124; &#39;ja&#39; &#124; &#39;ru&#39; &#124; &#39;zh&#39; &#124; &#39;ko&#39; &#124; &#39;es&#39;>** | The language to use for the response. | (optional) defaults to 'en'|
| **ifNoneMatch** | [**string**] | The ETag of the previous request. A 304 will be returned if this matches the current ETag. | (optional) defaults to undefined|
| **xTenant** | [**string**] | The tenant ID for the request. | (optional) defaults to 'tranquility'|
| **ifModifiedSince** | [**string**] | The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. | (optional) defaults to undefined|


### Return type

**UniverseIdsPost**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | OK |  * Cache-Control -  <br>  * Content-Language -  <br>  * ETag -  <br>  * Last-Modified -  <br>  |
|**0** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **postUniverseNames**
> Array<UniverseNamesPostInner> postUniverseNames(requestBody)

Resolve a set of IDs to names and categories. Supported ID\'s for resolving are: Characters, Corporations, Alliances, Stations, Solar Systems, Constellations, Regions, Types, Factions

### Example

```typescript
import {
    UniverseApi,
    Configuration
} from 'eve-esi-client-ts';

const configuration = new Configuration();
const apiInstance = new UniverseApi(configuration);

let xCompatibilityDate: '2025-12-16'; //The compatibility date for the request. (default to undefined)
let requestBody: Set<number>; //
let acceptLanguage: 'en' | 'de' | 'fr' | 'ja' | 'ru' | 'zh' | 'ko' | 'es'; //The language to use for the response. (optional) (default to 'en')
let ifNoneMatch: string; //The ETag of the previous request. A 304 will be returned if this matches the current ETag. (optional) (default to undefined)
let xTenant: string; //The tenant ID for the request. (optional) (default to 'tranquility')
let ifModifiedSince: string; //The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. (optional) (default to undefined)

const { status, data } = await apiInstance.postUniverseNames(
    xCompatibilityDate,
    requestBody,
    acceptLanguage,
    ifNoneMatch,
    xTenant,
    ifModifiedSince
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **requestBody** | **Set<number>**|  | |
| **xCompatibilityDate** | [**&#39;2025-12-16&#39;**]**Array<&#39;2025-12-16&#39;>** | The compatibility date for the request. | defaults to undefined|
| **acceptLanguage** | [**&#39;en&#39; | &#39;de&#39; | &#39;fr&#39; | &#39;ja&#39; | &#39;ru&#39; | &#39;zh&#39; | &#39;ko&#39; | &#39;es&#39;**]**Array<&#39;en&#39; &#124; &#39;de&#39; &#124; &#39;fr&#39; &#124; &#39;ja&#39; &#124; &#39;ru&#39; &#124; &#39;zh&#39; &#124; &#39;ko&#39; &#124; &#39;es&#39;>** | The language to use for the response. | (optional) defaults to 'en'|
| **ifNoneMatch** | [**string**] | The ETag of the previous request. A 304 will be returned if this matches the current ETag. | (optional) defaults to undefined|
| **xTenant** | [**string**] | The tenant ID for the request. | (optional) defaults to 'tranquility'|
| **ifModifiedSince** | [**string**] | The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. | (optional) defaults to undefined|


### Return type

**Array<UniverseNamesPostInner>**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | OK |  * Cache-Control -  <br>  * ETag -  <br>  * Last-Modified -  <br>  |
|**0** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

