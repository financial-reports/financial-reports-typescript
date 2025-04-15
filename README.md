## @financial-reports/generated-client-ts@0.1.1

This generator creates TypeScript/JavaScript client that utilizes [axios](https://github.com/axios/axios). The generated Node module can be used in the following environments:

Environment
* Node.js
* Webpack
* Browserify

Language level
* ES5 - you must have a Promises/A+ library installed
* ES6

Module system
* CommonJS
* ES6 module system

It can be used in both TypeScript and JavaScript. In TypeScript, the definition will be automatically resolved via `package.json`. ([Reference](https://www.typescriptlang.org/docs/handbook/declaration-files/consumption.html))

### Building

To build and compile the typescript sources to javascript use:
```
npm install
npm run build
```

### Publishing

First build the package then run `npm publish`

### Consuming

navigate to the folder of your consuming project and run one of the following commands.

_published:_

```
npm install @financial-reports/generated-client-ts@0.1.1 --save
```

_unPublished (not recommended):_

```
npm install PATH_TO_GENERATED_PACKAGE --save
```

### Documentation for API Endpoints

All URIs are relative to *https://api.financialreports.eu*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*CompaniesApi* | [**companiesList**](docs/CompaniesApi.md#companieslist) | **GET** /companies/ | 
*CompaniesApi* | [**companiesRetrieve**](docs/CompaniesApi.md#companiesretrieve) | **GET** /companies/{id}/ | 
*FilingTypesApi* | [**filingTypesList**](docs/FilingTypesApi.md#filingtypeslist) | **GET** /filing-types/ | 
*FilingTypesApi* | [**filingTypesRetrieve**](docs/FilingTypesApi.md#filingtypesretrieve) | **GET** /filing-types/{id}/ | 
*FilingsApi* | [**filingsList**](docs/FilingsApi.md#filingslist) | **GET** /filings/ | 
*FilingsApi* | [**filingsRetrieve**](docs/FilingsApi.md#filingsretrieve) | **GET** /filings/{id}/ | 
*IndustriesApi* | [**industriesList**](docs/IndustriesApi.md#industrieslist) | **GET** /industries/ | 
*IndustriesApi* | [**industriesRetrieve**](docs/IndustriesApi.md#industriesretrieve) | **GET** /industries/{id}/ | 
*IndustryGroupsApi* | [**industryGroupsList**](docs/IndustryGroupsApi.md#industrygroupslist) | **GET** /industry-groups/ | 
*IndustryGroupsApi* | [**industryGroupsRetrieve**](docs/IndustryGroupsApi.md#industrygroupsretrieve) | **GET** /industry-groups/{id}/ | 
*SchemaApi* | [**schemaRetrieve**](docs/SchemaApi.md#schemaretrieve) | **GET** /schema/ | 
*SectorsApi* | [**sectorsList**](docs/SectorsApi.md#sectorslist) | **GET** /sectors/ | 
*SectorsApi* | [**sectorsRetrieve**](docs/SectorsApi.md#sectorsretrieve) | **GET** /sectors/{id}/ | 
*SourcesApi* | [**sourcesList**](docs/SourcesApi.md#sourceslist) | **GET** /sources/ | 
*SourcesApi* | [**sourcesRetrieve**](docs/SourcesApi.md#sourcesretrieve) | **GET** /sources/{id}/ | 
*SubIndustriesApi* | [**subIndustriesList**](docs/SubIndustriesApi.md#subindustrieslist) | **GET** /sub-industries/ | 
*SubIndustriesApi* | [**subIndustriesRetrieve**](docs/SubIndustriesApi.md#subindustriesretrieve) | **GET** /sub-industries/{id}/ | 


### Documentation For Models

 - [Company](docs/Company.md)
 - [CompanyMinimal](docs/CompanyMinimal.md)
 - [Filing](docs/Filing.md)
 - [FilingType](docs/FilingType.md)
 - [Industry](docs/Industry.md)
 - [IndustryGroup](docs/IndustryGroup.md)
 - [Language](docs/Language.md)
 - [PaginatedCompanyList](docs/PaginatedCompanyList.md)
 - [PaginatedFilingList](docs/PaginatedFilingList.md)
 - [PaginatedFilingTypeList](docs/PaginatedFilingTypeList.md)
 - [PaginatedIndustryGroupList](docs/PaginatedIndustryGroupList.md)
 - [PaginatedIndustryList](docs/PaginatedIndustryList.md)
 - [PaginatedSectorList](docs/PaginatedSectorList.md)
 - [PaginatedSourceList](docs/PaginatedSourceList.md)
 - [PaginatedSubIndustryList](docs/PaginatedSubIndustryList.md)
 - [Sector](docs/Sector.md)
 - [Source](docs/Source.md)
 - [SubIndustry](docs/SubIndustry.md)


<a id="documentation-for-authorization"></a>
## Documentation For Authorization


Authentication schemes defined for the API:
<a id="basicAuth"></a>
### basicAuth

- **Type**: HTTP basic authentication

<a id="cookieAuth"></a>
### cookieAuth

- **Type**: API key
- **API key parameter name**: sessionid
- **Location**: 

