$${\color{red}Api<6> \space \color{blue}Reset  \space Counters \space Of \space Office}$$

POST /api/offices/<str:ref_office>/resetcounters

This API endpoint allows an authenticated manager to set the office counter and the window's number of served tickets to zero

### Params

|Name|Location|Type|Required|Description|
|---|---|---|---|---|
|»ref_office|query|string| yes |the reference of an office|
|Cookie|header|string| yes |require the user to be authenticated|

> Response Examples

> Success

```json
{
  "message": "Counters reset successfully"
}
```
