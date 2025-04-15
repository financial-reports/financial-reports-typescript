# CompaniesApi

All URIs are relative to *https://api.financialreports.eu*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**companiesList**](#companieslist) | **GET** /companies/ | |
|[**companiesRetrieve**](#companiesretrieve) | **GET** /companies/{id}/ | |

# **companiesList**
> PaginatedCompanyList companiesList()

Retrieve a paginated list of companies.  Supports filtering via query parameters defined in the CompanyFilter and searching via the \'search\' parameter (searches name, ISINs, and LEI).

### Example

```typescript
import {
    CompaniesApi,
    Configuration
} from '@financial-reports/generated-client-ts';

const configuration = new Configuration();
const apiInstance = new CompaniesApi(configuration);

let countries: string; //Filter by Company country ISO Alpha-2 code(s). Comma-separated for multiple values (e.g., US,GB,DE). (optional) (default to undefined)
let industry: string; //Filter by GICS Industry code. (optional) (default to undefined)
let industryGroup: string; //Filter by GICS Industry Group code. (optional) (default to undefined)
let page: number; //A page number within the paginated result set. (optional) (default to undefined)
let pageSize: number; //Number of results to return per page. (optional) (default to undefined)
let search: string; //A search term. (optional) (default to undefined)
let sector: string; //Filter by GICS Sector code. (optional) (default to undefined)
let subIndustry: string; //Filter by GICS Sub-Industry code. (optional) (default to undefined)

const { status, data } = await apiInstance.companiesList(
    countries,
    industry,
    industryGroup,
    page,
    pageSize,
    search,
    sector,
    subIndustry
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **countries** | [**string**] | Filter by Company country ISO Alpha-2 code(s). Comma-separated for multiple values (e.g., US,GB,DE). | (optional) defaults to undefined|
| **industry** | [**string**] | Filter by GICS Industry code. | (optional) defaults to undefined|
| **industryGroup** | [**string**] | Filter by GICS Industry Group code. | (optional) defaults to undefined|
| **page** | [**number**] | A page number within the paginated result set. | (optional) defaults to undefined|
| **pageSize** | [**number**] | Number of results to return per page. | (optional) defaults to undefined|
| **search** | [**string**] | A search term. | (optional) defaults to undefined|
| **sector** | [**string**] | Filter by GICS Sector code. | (optional) defaults to undefined|
| **subIndustry** | [**string**] | Filter by GICS Sub-Industry code. | (optional) defaults to undefined|


### Return type

**PaginatedCompanyList**

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

# **companiesRetrieve**
> Company companiesRetrieve()

Retrieve detailed information for a single company by its ID.

### Example

```typescript
import {
    CompaniesApi,
    Configuration
} from '@financial-reports/generated-client-ts';

const configuration = new Configuration();
const apiInstance = new CompaniesApi(configuration);

let id: number; // (default to undefined)

const { status, data } = await apiInstance.companiesRetrieve(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] |  | defaults to undefined|


### Return type

**Company**

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

