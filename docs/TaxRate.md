

# TaxRate

Ставка НДС

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**id** | **UUID** | ID налоговой ставки |  [optional] [readonly] |
|**accountId** | **UUID** | ID учетной записи |  [optional] [readonly] |
|**owner** | [**Employee**](Employee.md) | Метаданные владельца (Сотрудника) |  [optional] |
|**shared** | **Boolean** | Флаг общего доступа |  [optional] |
|**group** | [**Group**](Group.md) |  |  [optional] |
|**updated** | **String** | Момент последнего обновления сущности |  [optional] [readonly] |
|**rate** | **Float** | Значение налоговой ставки |  [optional] |
|**archived** | **Boolean** | Флаг принадлежности ставки к архивным ставкам |  [optional] |
|**comment** | **String** | Комментарий к налоговой ставке |  [optional] |



