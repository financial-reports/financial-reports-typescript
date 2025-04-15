# FilingType

Serializer for FilingType model, representing the type of a regulatory filing.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **string** | Unique code identifying the filing type. | [readonly] [default to undefined]
**name** | **string** | Human-readable name of the filing type. | [readonly] [default to undefined]
**description** | **string** | Detailed description of the filing type. | [readonly] [default to undefined]

## Example

```typescript
import { FilingType } from '@financial-reports/generated-client-ts';

const instance: FilingType = {
    code,
    name,
    description,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
