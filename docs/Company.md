# Company

Provides a detailed representation of a Company.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **number** | Unique identifier for the company. | [readonly] [default to undefined]
**name** | **string** | Company name. | [readonly] [default to undefined]
**lei** | **string** | Legal Entity Identifier (ISO 17442). | [readonly] [default to undefined]
**country_code** | **string** | ISO 3166-1 alpha-2 country code of the company\&#39;s primary registration or headquarters. | [readonly] [default to undefined]
**sector** | [**Sector**](Sector.md) | Company\&#39;s GICS Sector classification. | [readonly] [default to undefined]
**industry_group** | [**IndustryGroup**](IndustryGroup.md) | Company\&#39;s GICS Industry Group classification. | [readonly] [default to undefined]
**industry** | [**Industry**](Industry.md) | Company\&#39;s GICS Industry classification. | [readonly] [default to undefined]
**sub_industry** | [**SubIndustry**](SubIndustry.md) | Company\&#39;s GICS Sub-Industry classification. | [readonly] [default to undefined]
**ir_link** | **string** | Link to the company\&#39;s Investor Relations page. | [readonly] [default to undefined]
**homepage_link** | **string** | Link to the company\&#39;s main homepage. | [readonly] [default to undefined]
**date_public** | **string** | Date the company first became public. | [readonly] [default to undefined]
**date_ipo** | **string** | Date of the company\&#39;s Initial Public Offering. | [readonly] [default to undefined]
**main_stock_exchange** | **string** | Primary stock exchange where the company is listed. | [readonly] [default to undefined]
**social_facebook** | **string** | Facebook profile/page identifier. | [readonly] [default to undefined]
**social_instagram** | **string** | Instagram profile identifier. | [readonly] [default to undefined]
**social_twitter** | **string** | Twitter handle (without @). | [readonly] [default to undefined]
**social_linkedin** | **string** | LinkedIn company page identifier/URL path. | [readonly] [default to undefined]
**social_youtube** | **string** | YouTube channel identifier. | [readonly] [default to undefined]
**social_tiktok** | **string** | TikTok profile identifier. | [readonly] [default to undefined]
**social_pinterest** | **string** | Pinterest profile identifier. | [readonly] [default to undefined]
**social_xing** | **string** | Xing company profile identifier. | [readonly] [default to undefined]
**social_glassdoor** | **string** | Glassdoor company identifier. | [readonly] [default to undefined]
**year_founded** | **number** | Year the company was founded. | [readonly] [default to undefined]
**corporate_video_id** | **string** | Identifier for a corporate video (e.g., YouTube ID). | [readonly] [default to undefined]
**served_area** | **string** | Geographical area served by the company. | [readonly] [default to undefined]
**headcount** | **number** | Approximate number of employees. | [readonly] [default to undefined]
**contact_email** | **string** | General contact email address. | [readonly] [default to undefined]
**ticker** | **string** | Primary stock ticker symbol. | [readonly] [default to undefined]
**is_listed** | **boolean** | Indicates if the company is currently publicly listed. | [readonly] [default to undefined]

## Example

```typescript
import { Company } from '@financial-reports/generated-client-ts';

const instance: Company = {
    id,
    name,
    lei,
    country_code,
    sector,
    industry_group,
    industry,
    sub_industry,
    ir_link,
    homepage_link,
    date_public,
    date_ipo,
    main_stock_exchange,
    social_facebook,
    social_instagram,
    social_twitter,
    social_linkedin,
    social_youtube,
    social_tiktok,
    social_pinterest,
    social_xing,
    social_glassdoor,
    year_founded,
    corporate_video_id,
    served_area,
    headcount,
    contact_email,
    ticker,
    is_listed,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
