# SectorsApi

All URIs are relative to *https://api.financialreports.eu*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**sectorsList**](#sectorslist) | **GET** /sectors/ | |
|[**sectorsRetrieve**](#sectorsretrieve) | **GET** /sectors/{id}/ | |

# **sectorsList**
> PaginatedSectorList sectorsList()

Retrieve a list of all available GICS Sectors.

### Example

```typescript
import {
    SectorsApi,
    Configuration
} from '@financial-reports/generated-client-ts';

const configuration = new Configuration();
const apiInstance = new SectorsApi(configuration);

let page: number; //A page number within the paginated result set. (optional) (default to undefined)
let pageSize: number; //Number of results to return per page. (optional) (default to undefined)
let search: string; //A search term. (optional) (default to undefined)

const { status, data } = await apiInstance.sectorsList(
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

**PaginatedSectorList**

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

# **sectorsRetrieve**
> Sector sectorsRetrieve()

Retrieve details for a single GICS Sector by its primary key.

### Example

```typescript
import {
    SectorsApi,
    Configuration
} from '@financial-reports/generated-client-ts';

const configuration = new Configuration();
const apiInstance = new SectorsApi(configuration);

let id: number; // (default to undefined)

const { status, data } = await apiInstance.sectorsRetrieve(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] |  | defaults to undefined|


### Return type

**Sector**

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

