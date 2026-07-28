

# ProcessingOrderPosition

Позиция Заказа на производство

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**id** | **UUID** | ID позиции |  [optional] [readonly] |
|**accountId** | **UUID** | ID учетной записи |  [optional] [readonly] |
|**quantity** | **Double** | Количество товаров данного вида в позиции |  [optional] |
|**reserve** | **Double** | Резерв данной позиции |  [optional] |
|**assortment** | [**ProductMarker**](ProductMarker.md) | Метаданные товара/услуги/партии/модификации позиции |  [optional] |
|**pack** | [**Pack**](Pack.md) | Упаковка Товара |  [optional] |



