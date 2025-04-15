# FilingsApi

All URIs are relative to *https://api.financialreports.eu*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**filingsList**](#filingslist) | **GET** /filings/ | |
|[**filingsRetrieve**](#filingsretrieve) | **GET** /filings/{id}/ | |

# **filingsList**
> PaginatedFilingList filingsList()

Retrieve a paginated list of filings.  Supports filtering via query parameters defined in the FilingFilter, searching via the \'search\' parameter (searches company name and title), and ordering via the \'ordering\' parameter (allowed fields: release_datetime, added_to_platform).

### Example

```typescript
import {
    FilingsApi,
    Configuration
} from '@financial-reports/generated-client-ts';

const configuration = new Configuration();
const apiInstance = new FilingsApi(configuration);

let addedToPlatformFrom: string; //Filter by date added to platform (inclusive start date, YYYY-MM-DDTHH:MM:SSZ format). (optional) (default to undefined)
let addedToPlatformTo: string; //Filter by date added to platform (inclusive end date, YYYY-MM-DDTHH:MM:SSZ format). (optional) (default to undefined)
let company: number; //Filter by internal Company ID. (optional) (default to undefined)
let companyIsin: string; //Filter by Company ISIN. Case-insensitive. (optional) (default to undefined)
let countries: string; //Filter by Company country ISO Alpha-2 code(s). Comma-separated for multiple values (e.g., US,GB,DE). (optional) (default to undefined)
let disseminationDatetimeFrom: string; //Filter by dissemination datetime (inclusive start, YYYY-MM-DDTHH:MM:SSZ format). (optional) (default to undefined)
let disseminationDatetimeTo: string; //Filter by dissemination datetime (inclusive end, YYYY-MM-DDTHH:MM:SSZ format). (optional) (default to undefined)
let language: string; //Filter by a single filing language ISO 639-1 code (e.g., en). (optional) (default to undefined)
let languages: string; //Filter by filing language ISO 639-1 code(s). Comma-separated for multiple values (e.g., en,de). (optional) (default to undefined)
let lei: string; //Filter by Company Legal Entity Identifier (LEI). (optional) (default to undefined)
let ordering: string; //Which field to use when ordering the results. (optional) (default to undefined)
let page: number; //A page number within the paginated result set. (optional) (default to undefined)
let pageSize: number; //Number of results to return per page. (optional) (default to undefined)
let releaseDatetimeFrom: string; //Filter by release datetime (inclusive start, YYYY-MM-DDTHH:MM:SSZ format). (optional) (default to undefined)
let releaseDatetimeTo: string; //Filter by release datetime (inclusive end, YYYY-MM-DDTHH:MM:SSZ format). (optional) (default to undefined)
let search: string; //A search term. (optional) (default to undefined)
let source: number; // (optional) (default to undefined)
let type: string; //Filter by Filing Type code (e.g., ANNREP). (optional) (default to undefined)

const { status, data } = await apiInstance.filingsList(
    addedToPlatformFrom,
    addedToPlatformTo,
    company,
    companyIsin,
    countries,
    disseminationDatetimeFrom,
    disseminationDatetimeTo,
    language,
    languages,
    lei,
    ordering,
    page,
    pageSize,
    releaseDatetimeFrom,
    releaseDatetimeTo,
    search,
    source,
    type
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **addedToPlatformFrom** | [**string**] | Filter by date added to platform (inclusive start date, YYYY-MM-DDTHH:MM:SSZ format). | (optional) defaults to undefined|
| **addedToPlatformTo** | [**string**] | Filter by date added to platform (inclusive end date, YYYY-MM-DDTHH:MM:SSZ format). | (optional) defaults to undefined|
| **company** | [**number**] | Filter by internal Company ID. | (optional) defaults to undefined|
| **companyIsin** | [**string**] | Filter by Company ISIN. Case-insensitive. | (optional) defaults to undefined|
| **countries** | [**string**] | Filter by Company country ISO Alpha-2 code(s). Comma-separated for multiple values (e.g., US,GB,DE). | (optional) defaults to undefined|
| **disseminationDatetimeFrom** | [**string**] | Filter by dissemination datetime (inclusive start, YYYY-MM-DDTHH:MM:SSZ format). | (optional) defaults to undefined|
| **disseminationDatetimeTo** | [**string**] | Filter by dissemination datetime (inclusive end, YYYY-MM-DDTHH:MM:SSZ format). | (optional) defaults to undefined|
| **language** | [**string**] | Filter by a single filing language ISO 639-1 code (e.g., en). | (optional) defaults to undefined|
| **languages** | [**string**] | Filter by filing language ISO 639-1 code(s). Comma-separated for multiple values (e.g., en,de). | (optional) defaults to undefined|
| **lei** | [**string**] | Filter by Company Legal Entity Identifier (LEI). | (optional) defaults to undefined|
| **ordering** | [**string**] | Which field to use when ordering the results. | (optional) defaults to undefined|
| **page** | [**number**] | A page number within the paginated result set. | (optional) defaults to undefined|
| **pageSize** | [**number**] | Number of results to return per page. | (optional) defaults to undefined|
| **releaseDatetimeFrom** | [**string**] | Filter by release datetime (inclusive start, YYYY-MM-DDTHH:MM:SSZ format). | (optional) defaults to undefined|
| **releaseDatetimeTo** | [**string**] | Filter by release datetime (inclusive end, YYYY-MM-DDTHH:MM:SSZ format). | (optional) defaults to undefined|
| **search** | [**string**] | A search term. | (optional) defaults to undefined|
| **source** | [**number**] |  | (optional) defaults to undefined|
| **type** | [**string**] | Filter by Filing Type code (e.g., ANNREP). | (optional) defaults to undefined|


### Return type

**PaginatedFilingList**

### Authorization

[basicAuth](../README.md#basicAuth), [cookieAuth](../README.md#cookieAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **filingsRetrieve**
> Filing filingsRetrieve()

Retrieve detailed information for a single filing by its ID.

### Example

```typescript
import {
    FilingsApi,
    Configuration
} from '@financial-reports/generated-client-ts';

const configuration = new Configuration();
const apiInstance = new FilingsApi(configuration);

let id: number; // (default to undefined)

const { status, data } = await apiInstance.filingsRetrieve(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] |  | defaults to undefined|


### Return type

**Filing**

### Authorization

[basicAuth](../README.md#basicAuth), [cookieAuth](../README.md#cookieAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

