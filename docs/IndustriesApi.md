# IndustriesApi

All URIs are relative to *https://api.financialreports.eu*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**industriesList**](#industrieslist) | **GET** /industries/ | |
|[**industriesRetrieve**](#industriesretrieve) | **GET** /industries/{id}/ | |

# **industriesList**
> PaginatedIndustryList industriesList()

Retrieve a list of all available GICS Industries. Can be filtered by parent industry group ID.

### Example

```typescript
import {
    IndustriesApi,
    Configuration
} from '@financial-reports/generated-client-ts';

const configuration = new Configuration();
const apiInstance = new IndustriesApi(configuration);

let industryGroup: number; // (optional) (default to undefined)
let page: number; //A page number within the paginated result set. (optional) (default to undefined)
let pageSize: number; //Number of results to return per page. (optional) (default to undefined)
let search: string; //A search term. (optional) (default to undefined)

const { status, data } = await apiInstance.industriesList(
    industryGroup,
    page,
    pageSize,
    search
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **industryGroup** | [**number**] |  | (optional) defaults to undefined|
| **page** | [**number**] | A page number within the paginated result set. | (optional) defaults to undefined|
| **pageSize** | [**number**] | Number of results to return per page. | (optional) defaults to undefined|
| **search** | [**string**] | A search term. | (optional) defaults to undefined|


### Return type

**PaginatedIndustryList**

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

# **industriesRetrieve**
> Industry industriesRetrieve()

Retrieve details for a single GICS Industry by its primary key.

### Example

```typescript
import {
    IndustriesApi,
    Configuration
} from '@financial-reports/generated-client-ts';

const configuration = new Configuration();
const apiInstance = new IndustriesApi(configuration);

let id: number; // (default to undefined)

const { status, data } = await apiInstance.industriesRetrieve(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] |  | defaults to undefined|


### Return type

**Industry**

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

