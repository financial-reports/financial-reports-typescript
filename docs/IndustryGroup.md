# IndustryGroup

Serializer for GICS Industry Group classification, including its parent Sector.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **string** | GICS Industry Group code. | [readonly] [default to undefined]
**name** | **string** | GICS Industry Group name. | [readonly] [default to undefined]
**sector** | [**Sector**](Sector.md) | Parent GICS Sector. | [readonly] [default to undefined]

## Example

```typescript
import { IndustryGroup } from '@financial-reports/generated-client-ts';

const instance: IndustryGroup = {
    code,
    name,
    sector,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
