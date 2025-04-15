# IndustryGroupsApi

All URIs are relative to *https://api.financialreports.eu*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**industryGroupsList**](#industrygroupslist) | **GET** /industry-groups/ | |
|[**industryGroupsRetrieve**](#industrygroupsretrieve) | **GET** /industry-groups/{id}/ | |

# **industryGroupsList**
> PaginatedIndustryGroupList industryGroupsList()

Retrieve a list of all available GICS Industry Groups. Can be filtered by parent sector ID.

### Example

```typescript
import {
    IndustryGroupsApi,
    Configuration
} from '@financial-reports/generated-client-ts';

const configuration = new Configuration();
const apiInstance = new IndustryGroupsApi(configuration);

let page: number; //A page number within the paginated result set. (optional) (default to undefined)
let pageSize: number; //Number of results to return per page. (optional) (default to undefined)
let search: string; //A search term. (optional) (default to undefined)
let sector: number; // (optional) (default to undefined)

const { status, data } = await apiInstance.industryGroupsList(
    page,
    pageSize,
    search,
    sector
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **page** | [**number**] | A page number within the paginated result set. | (optional) defaults to undefined|
| **pageSize** | [**number**] | Number of results to return per page. | (optional) defaults to undefined|
| **search** | [**string**] | A search term. | (optional) defaults to undefined|
| **sector** | [**number**] |  | (optional) defaults to undefined|


### Return type

**PaginatedIndustryGroupList**

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

# **industryGroupsRetrieve**
> IndustryGroup industryGroupsRetrieve()

Retrieve details for a single GICS Industry Group by its primary key.

### Example

```typescript
import {
    IndustryGroupsApi,
    Configuration
} from '@financial-reports/generated-client-ts';

const configuration = new Configuration();
const apiInstance = new IndustryGroupsApi(configuration);

let id: number; // (default to undefined)

const { status, data } = await apiInstance.industryGroupsRetrieve(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] |  | defaults to undefined|


### Return type

**IndustryGroup**

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

