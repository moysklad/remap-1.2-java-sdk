

# CreateTaskMetadataStatesRequest


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**id** | **UUID** | ID статуса |  [optional] [readonly] |
|**name** | **String** | Наименование статуса |  [optional] |
|**accountId** | **UUID** | ID учетной записи |  [optional] [readonly] |
|**color** | **Integer** | Цвет Статуса |  [optional] |
|**entityType** | **String** | Тип сущности, к которой относится Статус (ключевое слово в рамках JSON API) |  [optional] [readonly] |
|**stateType** | **String** | Тип Статуса. Известные значения описаны в StateType |  [optional] |



