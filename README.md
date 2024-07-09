## api-endpoints

$${\color{red}Api1 \space \color{blue}Assign  \space Agent \space To \space Window }$$

POST /api/windows/<int:number_window>/assign-agent/

This API endpoint allows an authenticated manager to assign an agent user to a specific office window

> Body Parameters

```json
{
  "agent_id": 12345,
  "office_id": "ref789"
}
```

### Params

|Name|Location|Type|Required|Description|
|---|---|---|---|---|
|Cookie|header|string| yes |require the user to be authenticated|
|body|body|object| yes |json data|
|» agent_id|body|integer| yes |the unique id of agent user|
|» office_id|body|string| yes |the unique reference of an office|

> Response Examples

> Success

```json
{
  "message": "Agent assigned to existing window successfully"
}
```
