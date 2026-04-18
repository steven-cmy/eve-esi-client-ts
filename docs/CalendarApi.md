# CalendarApi

All URIs are relative to *https://esi.evetech.net*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**getCharactersCharacterIdCalendar**](#getcharacterscharacteridcalendar) | **GET** /characters/{character_id}/calendar | List calendar event summaries|
|[**getCharactersCharacterIdCalendarEventId**](#getcharacterscharacteridcalendareventid) | **GET** /characters/{character_id}/calendar/{event_id} | Get an event|
|[**getCharactersCharacterIdCalendarEventIdAttendees**](#getcharacterscharacteridcalendareventidattendees) | **GET** /characters/{character_id}/calendar/{event_id}/attendees | Get attendees|
|[**putCharactersCharacterIdCalendarEventId**](#putcharacterscharacteridcalendareventid) | **PUT** /characters/{character_id}/calendar/{event_id} | Respond to an event|

# **getCharactersCharacterIdCalendar**
> Array<CharactersCharacterIdCalendarGetInner> getCharactersCharacterIdCalendar()

Get 50 event summaries from the calendar. If no from_event ID is given, the resource will return the next 50 chronological event summaries from now. If a from_event ID is specified, it will return the next 50 chronological event summaries from after that event

### Example

```typescript
import {
    CalendarApi,
    Configuration
} from 'eve-esi-client-ts';

const configuration = new Configuration();
const apiInstance = new CalendarApi(configuration);

let characterId: number; //The ID of the character (default to undefined)
let xCompatibilityDate: '2025-12-16'; //The compatibility date for the request. (default to undefined)
let fromEvent: number; // (optional) (default to undefined)
let acceptLanguage: 'en' | 'de' | 'fr' | 'ja' | 'ru' | 'zh' | 'ko' | 'es'; //The language to use for the response. (optional) (default to 'en')
let ifNoneMatch: string; //The ETag of the previous request. A 304 will be returned if this matches the current ETag. (optional) (default to undefined)
let xTenant: string; //The tenant ID for the request. (optional) (default to 'tranquility')
let ifModifiedSince: string; //The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. (optional) (default to undefined)

const { status, data } = await apiInstance.getCharactersCharacterIdCalendar(
    characterId,
    xCompatibilityDate,
    fromEvent,
    acceptLanguage,
    ifNoneMatch,
    xTenant,
    ifModifiedSince
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **characterId** | [**number**] | The ID of the character | defaults to undefined|
| **xCompatibilityDate** | [**&#39;2025-12-16&#39;**]**Array<&#39;2025-12-16&#39;>** | The compatibility date for the request. | defaults to undefined|
| **fromEvent** | [**number**] |  | (optional) defaults to undefined|
| **acceptLanguage** | [**&#39;en&#39; | &#39;de&#39; | &#39;fr&#39; | &#39;ja&#39; | &#39;ru&#39; | &#39;zh&#39; | &#39;ko&#39; | &#39;es&#39;**]**Array<&#39;en&#39; &#124; &#39;de&#39; &#124; &#39;fr&#39; &#124; &#39;ja&#39; &#124; &#39;ru&#39; &#124; &#39;zh&#39; &#124; &#39;ko&#39; &#124; &#39;es&#39;>** | The language to use for the response. | (optional) defaults to 'en'|
| **ifNoneMatch** | [**string**] | The ETag of the previous request. A 304 will be returned if this matches the current ETag. | (optional) defaults to undefined|
| **xTenant** | [**string**] | The tenant ID for the request. | (optional) defaults to 'tranquility'|
| **ifModifiedSince** | [**string**] | The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. | (optional) defaults to undefined|


### Return type

**Array<CharactersCharacterIdCalendarGetInner>**

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

# **getCharactersCharacterIdCalendarEventId**
> CharactersCharacterIdCalendarEventIdGet getCharactersCharacterIdCalendarEventId()

Get all the information for a specific event

### Example

```typescript
import {
    CalendarApi,
    Configuration
} from 'eve-esi-client-ts';

const configuration = new Configuration();
const apiInstance = new CalendarApi(configuration);

let characterId: number; //The ID of the character (default to undefined)
let eventId: number; // (default to undefined)
let xCompatibilityDate: '2025-12-16'; //The compatibility date for the request. (default to undefined)
let acceptLanguage: 'en' | 'de' | 'fr' | 'ja' | 'ru' | 'zh' | 'ko' | 'es'; //The language to use for the response. (optional) (default to 'en')
let ifNoneMatch: string; //The ETag of the previous request. A 304 will be returned if this matches the current ETag. (optional) (default to undefined)
let xTenant: string; //The tenant ID for the request. (optional) (default to 'tranquility')
let ifModifiedSince: string; //The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. (optional) (default to undefined)

const { status, data } = await apiInstance.getCharactersCharacterIdCalendarEventId(
    characterId,
    eventId,
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
| **characterId** | [**number**] | The ID of the character | defaults to undefined|
| **eventId** | [**number**] |  | defaults to undefined|
| **xCompatibilityDate** | [**&#39;2025-12-16&#39;**]**Array<&#39;2025-12-16&#39;>** | The compatibility date for the request. | defaults to undefined|
| **acceptLanguage** | [**&#39;en&#39; | &#39;de&#39; | &#39;fr&#39; | &#39;ja&#39; | &#39;ru&#39; | &#39;zh&#39; | &#39;ko&#39; | &#39;es&#39;**]**Array<&#39;en&#39; &#124; &#39;de&#39; &#124; &#39;fr&#39; &#124; &#39;ja&#39; &#124; &#39;ru&#39; &#124; &#39;zh&#39; &#124; &#39;ko&#39; &#124; &#39;es&#39;>** | The language to use for the response. | (optional) defaults to 'en'|
| **ifNoneMatch** | [**string**] | The ETag of the previous request. A 304 will be returned if this matches the current ETag. | (optional) defaults to undefined|
| **xTenant** | [**string**] | The tenant ID for the request. | (optional) defaults to 'tranquility'|
| **ifModifiedSince** | [**string**] | The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. | (optional) defaults to undefined|


### Return type

**CharactersCharacterIdCalendarEventIdGet**

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

# **getCharactersCharacterIdCalendarEventIdAttendees**
> Array<CharactersCharacterIdCalendarEventIdAttendeesGetInner> getCharactersCharacterIdCalendarEventIdAttendees()

Get all invited attendees for a given event

### Example

```typescript
import {
    CalendarApi,
    Configuration
} from 'eve-esi-client-ts';

const configuration = new Configuration();
const apiInstance = new CalendarApi(configuration);

let characterId: number; //The ID of the character (default to undefined)
let eventId: number; // (default to undefined)
let xCompatibilityDate: '2025-12-16'; //The compatibility date for the request. (default to undefined)
let acceptLanguage: 'en' | 'de' | 'fr' | 'ja' | 'ru' | 'zh' | 'ko' | 'es'; //The language to use for the response. (optional) (default to 'en')
let ifNoneMatch: string; //The ETag of the previous request. A 304 will be returned if this matches the current ETag. (optional) (default to undefined)
let xTenant: string; //The tenant ID for the request. (optional) (default to 'tranquility')
let ifModifiedSince: string; //The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. (optional) (default to undefined)

const { status, data } = await apiInstance.getCharactersCharacterIdCalendarEventIdAttendees(
    characterId,
    eventId,
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
| **characterId** | [**number**] | The ID of the character | defaults to undefined|
| **eventId** | [**number**] |  | defaults to undefined|
| **xCompatibilityDate** | [**&#39;2025-12-16&#39;**]**Array<&#39;2025-12-16&#39;>** | The compatibility date for the request. | defaults to undefined|
| **acceptLanguage** | [**&#39;en&#39; | &#39;de&#39; | &#39;fr&#39; | &#39;ja&#39; | &#39;ru&#39; | &#39;zh&#39; | &#39;ko&#39; | &#39;es&#39;**]**Array<&#39;en&#39; &#124; &#39;de&#39; &#124; &#39;fr&#39; &#124; &#39;ja&#39; &#124; &#39;ru&#39; &#124; &#39;zh&#39; &#124; &#39;ko&#39; &#124; &#39;es&#39;>** | The language to use for the response. | (optional) defaults to 'en'|
| **ifNoneMatch** | [**string**] | The ETag of the previous request. A 304 will be returned if this matches the current ETag. | (optional) defaults to undefined|
| **xTenant** | [**string**] | The tenant ID for the request. | (optional) defaults to 'tranquility'|
| **ifModifiedSince** | [**string**] | The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. | (optional) defaults to undefined|


### Return type

**Array<CharactersCharacterIdCalendarEventIdAttendeesGetInner>**

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

# **putCharactersCharacterIdCalendarEventId**
> putCharactersCharacterIdCalendarEventId(putCharactersCharacterIdCalendarEventIdRequest)

Set your response status to an event

### Example

```typescript
import {
    CalendarApi,
    Configuration,
    PutCharactersCharacterIdCalendarEventIdRequest
} from 'eve-esi-client-ts';

const configuration = new Configuration();
const apiInstance = new CalendarApi(configuration);

let characterId: number; //The ID of the character (default to undefined)
let eventId: number; // (default to undefined)
let xCompatibilityDate: '2025-12-16'; //The compatibility date for the request. (default to undefined)
let putCharactersCharacterIdCalendarEventIdRequest: PutCharactersCharacterIdCalendarEventIdRequest; //
let acceptLanguage: 'en' | 'de' | 'fr' | 'ja' | 'ru' | 'zh' | 'ko' | 'es'; //The language to use for the response. (optional) (default to 'en')
let ifNoneMatch: string; //The ETag of the previous request. A 304 will be returned if this matches the current ETag. (optional) (default to undefined)
let xTenant: string; //The tenant ID for the request. (optional) (default to 'tranquility')
let ifModifiedSince: string; //The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. (optional) (default to undefined)

const { status, data } = await apiInstance.putCharactersCharacterIdCalendarEventId(
    characterId,
    eventId,
    xCompatibilityDate,
    putCharactersCharacterIdCalendarEventIdRequest,
    acceptLanguage,
    ifNoneMatch,
    xTenant,
    ifModifiedSince
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **putCharactersCharacterIdCalendarEventIdRequest** | **PutCharactersCharacterIdCalendarEventIdRequest**|  | |
| **characterId** | [**number**] | The ID of the character | defaults to undefined|
| **eventId** | [**number**] |  | defaults to undefined|
| **xCompatibilityDate** | [**&#39;2025-12-16&#39;**]**Array<&#39;2025-12-16&#39;>** | The compatibility date for the request. | defaults to undefined|
| **acceptLanguage** | [**&#39;en&#39; | &#39;de&#39; | &#39;fr&#39; | &#39;ja&#39; | &#39;ru&#39; | &#39;zh&#39; | &#39;ko&#39; | &#39;es&#39;**]**Array<&#39;en&#39; &#124; &#39;de&#39; &#124; &#39;fr&#39; &#124; &#39;ja&#39; &#124; &#39;ru&#39; &#124; &#39;zh&#39; &#124; &#39;ko&#39; &#124; &#39;es&#39;>** | The language to use for the response. | (optional) defaults to 'en'|
| **ifNoneMatch** | [**string**] | The ETag of the previous request. A 304 will be returned if this matches the current ETag. | (optional) defaults to undefined|
| **xTenant** | [**string**] | The tenant ID for the request. | (optional) defaults to 'tranquility'|
| **ifModifiedSince** | [**string**] | The date the resource was last modified. A 304 will be returned if the resource has not been modified since this date. | (optional) defaults to undefined|


### Return type

void (empty response body)

### Authorization

[OAuth2](../README.md#OAuth2)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**204** | Event updated |  * Cache-Control -  <br>  * ETag -  <br>  * Last-Modified -  <br>  |
|**0** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

