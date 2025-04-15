# SourcesApi

All URIs are relative to *https://api.financialreports.eu*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**sourcesList**](#sourceslist) | **GET** /sources/ | |
|[**sourcesRetrieve**](#sourcesretrieve) | **GET** /sources/{id}/ | |

# **sourcesList**
> PaginatedSourceList sourcesList()

Retrieve a list of all available data sources.

### Example

```typescript
import {
    SourcesApi,
    Configuration
} from '@financial-reports/generated-client-ts';

const configuration = new Configuration();
const apiInstance = new SourcesApi(configuration);

let page: number; //A page number within the paginated result set. (optional) (default to undefined)
let pageSize: number; //Number of results to return per page. (optional) (default to undefined)

const { status, data } = await apiInstance.sourcesList(
    page,
    pageSize
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **page** | [**number**] | A page number within the paginated result set. | (optional) defaults to undefined|
| **pageSize** | [**number**] | Number of results to return per page. | (optional) defaults to undefined|


### Return type

**PaginatedSourceList**

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

# **sourcesRetrieve**
> Source sourcesRetrieve()

Retrieve details for a single data source by its primary key.

### Example

```typescript
import {
    SourcesApi,
    Configuration
} from '@financial-reports/generated-client-ts';

const configuration = new Configuration();
const apiInstance = new SourcesApi(configuration);

let id: number; // (default to undefined)

const { status, data } = await apiInstance.sourcesRetrieve(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] |  | defaults to undefined|


### Return type

**Source**

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

