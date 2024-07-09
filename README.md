$${\color{red}Api<4> \space \color{blue}Delete  \space Office}$$

DELETE /api/offices/<str:ref_office>/delete

This API endpoint allows an authenticated manager to delete an office 

### Params

|Name|Location|Type|Required|Description|
|---|---|---|---|---|
|»ref_office|query|string| yes |the reference of an office|
|Cookie|header|string| yes |require the user to be authenticated|

> Response Examples

> Success

```json
{
  "message": "office was deleted successfully"
}
```


$${\color{red}Api<4> \space \color{blue}Delete  \space Agent \space From \space Office}$$

DELETE /api/offices/<str:ref_office>/agents/<int:agent_id>/delete

This API endpoint allows an authenticated manager to delete an Agent From Office 

### Params

|Name|Location|Type|Required|Description|
|---|---|---|---|---|
|»ref_office|query|string| yes |the reference of an office|
|»agent_id|query|int| yes |the id of an Agent user|
|Cookie|header|string| yes |require the user to be authenticated|

> Response Examples

> Success

```json
{
  "message": "Agent deleted successfully"
}
```
