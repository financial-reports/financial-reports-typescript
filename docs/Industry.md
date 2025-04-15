# Industry

Serializer for GICS Industry classification, including its parent Industry Group.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **string** | GICS Industry code. | [readonly] [default to undefined]
**name** | **string** | GICS Industry name. | [readonly] [default to undefined]
**industry_group** | [**IndustryGroup**](IndustryGroup.md) | Parent GICS Industry Group. | [readonly] [default to undefined]

## Example

```typescript
import { Industry } from '@financial-reports/generated-client-ts';

const instance: Industry = {
    code,
    name,
    industry_group,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
