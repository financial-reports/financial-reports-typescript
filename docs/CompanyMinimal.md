# CompanyMinimal

Provides a minimal representation of a Company, suitable for nesting.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **number** | Unique identifier for the company. | [readonly] [default to undefined]
**name** | **string** | Company name. | [readonly] [default to undefined]
**lei** | **string** | Legal Entity Identifier (ISO 17442). | [readonly] [default to undefined]
**sub_industry_code** | **string** | GICS Sub-Industry code classifying the company. | [readonly] [default to undefined]
**country_code** | **string** | ISO 3166-1 alpha-2 country code of the company\&#39;s primary registration or headquarters. | [readonly] [default to undefined]

## Example

```typescript
import { CompanyMinimal } from '@financial-reports/generated-client-ts';

const instance: CompanyMinimal = {
    id,
    name,
    lei,
    sub_industry_code,
    country_code,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
