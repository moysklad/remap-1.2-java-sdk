

# State

Статус

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**id** | **UUID** | ID статуса |  [optional] [readonly] |
|**name** | **String** | Наименование статуса |  [optional] |
|**accountId** | **UUID** | ID учетной записи |  [optional] [readonly] |
|**color** | **Integer** | Цвет Статуса |  [optional] |
|**entityType** | **String** | Тип сущности, к которой относится Статус (ключевое слово в рамках JSON API) |  [optional] [readonly] |
|**stateType** | [**StateTypeEnum**](#StateTypeEnum) | Тип Статуса |  [optional] |



## Enum: StateTypeEnum

| Name | Value |
|---- | -----|
| REGULAR | &quot;Regular&quot; |
| SUCCESSFUL | &quot;Successful&quot; |
| UNSUCCESSFUL | &quot;Unsuccessful&quot; |



