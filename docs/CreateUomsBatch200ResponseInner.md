

# CreateUomsBatch200ResponseInner


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**id** | **UUID** | ID единицы измерения |  [optional] [readonly] |
|**accountId** | **UUID** | ID учетной записи |  [optional] [readonly] |
|**name** | **String** | Наименование единицы измерения |  [optional] |
|**description** | **String** | Описание единицы измерения |  [optional] |
|**code** | **String** | Код единицы измерения |  [optional] |
|**group** | [**Group**](Group.md) |  |  [optional] |
|**owner** | [**Employee**](Employee.md) | Метаданные владельца (Сотрудника) |  [optional] |
|**updated** | **String** | Момент последнего обновления сущности |  [optional] [readonly] |
|**shared** | **Boolean** | Общий доступ |  [optional] |
|**externalCode** | **String** | Внешний код единицы измерения |  [optional] |
|**errors** | [**List&lt;ErrorErrorsInner&gt;**](ErrorErrorsInner.md) |  |  |



