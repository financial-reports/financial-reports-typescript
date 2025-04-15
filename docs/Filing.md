# Filing

Serializer for regulatory filings.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **number** | Unique identifier for the filing. | [readonly] [default to undefined]
**company** | [**CompanyMinimal**](CompanyMinimal.md) | Basic details of the company that made the filing. | [readonly] [default to undefined]
**filing_type** | [**FilingType**](FilingType.md) | Details of the filing type. | [readonly] [default to undefined]
**language** | [**Language**](Language.md) | Language of the filing document. | [readonly] [default to undefined]
**filing_date** | **string** | The official date the document was filed. | [readonly] [default to undefined]
**title** | **string** | Title of the filing document. | [readonly] [default to undefined]
**added_to_platform** | **string** | Timestamp when the filing was added to our system (UTC). | [readonly] [default to undefined]
**updated_date** | **string** | Timestamp when the filing record was last updated (UTC). | [readonly] [default to undefined]
**dissemination_datetime** | **string** | Timestamp when the filing was disseminated by the source (UTC). | [readonly] [default to undefined]
**release_datetime** | **string** | Timestamp when the filing was released (e.g., for press releases) (UTC). | [readonly] [default to undefined]
**source** | [**Source**](Source.md) | Source from which the filing was obtained. | [readonly] [default to undefined]
**document** | **string** | URL link to the primary filing document (e.g., PDF, HTML). | [readonly] [default to undefined]
**year** | **number** | The financial year the filing pertains to. | [readonly] [default to undefined]

## Example

```typescript
import { Filing } from '@financial-reports/generated-client-ts';

const instance: Filing = {
    id,
    company,
    filing_type,
    language,
    filing_date,
    title,
    added_to_platform,
    updated_date,
    dissemination_datetime,
    release_datetime,
    source,
    document,
    year,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
