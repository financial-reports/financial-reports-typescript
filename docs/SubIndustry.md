# SubIndustry

Serializer for GICS Sub-Industry classification, including its parent Industry.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **string** | GICS Sub-Industry code. | [readonly] [default to undefined]
**name** | **string** | GICS Sub-Industry name. | [readonly] [default to undefined]
**industry** | [**Industry**](Industry.md) | Parent GICS Industry. | [readonly] [default to undefined]

## Example

```typescript
import { SubIndustry } from '@financial-reports/generated-client-ts';

const instance: SubIndustry = {
    code,
    name,
    industry,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
