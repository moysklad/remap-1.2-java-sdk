

# EmissionOrderPosition

Позиция Заказа кодов маркировки

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**id** | **UUID** | ID позиции |  [optional] [readonly] |
|**accountId** | **UUID** | ID учетной записи |  [optional] [readonly] |
|**assortment** | [**Assortment**](Assortment.md) |  |  [optional] |
|**quantity** | **Float** | Количество товаров данного вида в позиции |  [optional] |
|**status** | **String** | Статус кодов. Известные значения описаны в EmissionOrderPositionStatus |  [optional] [readonly] |



