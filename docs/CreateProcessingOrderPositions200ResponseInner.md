

# CreateProcessingOrderPositions200ResponseInner


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**id** | **UUID** | ID позиции |  [optional] |
|**accountId** | **UUID** | ID учетной записи |  [optional] [readonly] |
|**quantity** | **Double** | Количество товаров данного вида в позиции |  [optional] |
|**reserve** | **Double** | Резерв данной позиции |  [optional] |
|**assortment** | [**ProductMarker**](ProductMarker.md) | Метаданные товара/услуги/партии/модификации позиции |  [optional] |
|**pack** | [**Pack**](Pack.md) | Упаковка Товара |  [optional] |
|**errors** | [**List&lt;Error&gt;**](Error.md) |  |  |



