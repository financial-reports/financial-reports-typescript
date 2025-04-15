# Source

Serializer for Source model, representing the origin of the filing data.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **string** | Name of the data source. | [readonly] [default to undefined]
**url** | **string** | URL of the data source homepage or relevant section. | [readonly] [default to undefined]
**description** | **string** | Description of the data source. | [readonly] [default to undefined]

## Example

```typescript
import { Source } from '@financial-reports/generated-client-ts';

const instance: Source = {
    name,
    url,
    description,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
