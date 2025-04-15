# FilingTypesApi

All URIs are relative to *https://api.financialreports.eu*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**filingTypesList**](#filingtypeslist) | **GET** /filing-types/ | |
|[**filingTypesRetrieve**](#filingtypesretrieve) | **GET** /filing-types/{id}/ | |

# **filingTypesList**
> PaginatedFilingTypeList filingTypesList()

Retrieve a list of all available filing types.

### Example

```typescript
import {
    FilingTypesApi,
    Configuration
} from '@financial-reports/generated-client-ts';

const configuration = new Configuration();
const apiInstance = new FilingTypesApi(configuration);

let page: number; //A page number within the paginated result set. (optional) (default to undefined)
let pageSize: number; //Number of results to return per page. (optional) (default to undefined)
let search: string; //A search term. (optional) (default to undefined)

const { status, data } = await apiInstance.filingTypesList(
    page,
    pageSize,
    search
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **page** | [**number**] | A page number within the paginated result set. | (optional) defaults to undefined|
| **pageSize** | [**number**] | Number of results to return per page. | (optional) defaults to undefined|
| **search** | [**string**] | A search term. | (optional) defaults to undefined|


### Return type

**PaginatedFilingTypeList**

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

# **filingTypesRetrieve**
> FilingType filingTypesRetrieve()

Retrieve details for a single filing type by its primary key (likely ID, depends on model).

### Example

```typescript
import {
    FilingTypesApi,
    Configuration
} from '@financial-reports/generated-client-ts';

const configuration = new Configuration();
const apiInstance = new FilingTypesApi(configuration);

let id: number; // (default to undefined)

const { status, data } = await apiInstance.filingTypesRetrieve(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] |  | defaults to undefined|


### Return type

**FilingType**

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

