

# PriceListPosition

Позиция Прайс-листа

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**id** | **UUID** | ID позиции |  [optional] |
|**accountId** | **UUID** | ID учетной записи |  [optional] [readonly] |
|**assortment** | [**ProductMarker**](ProductMarker.md) | Метаданные номенклатуры, которую представляет собой позиция |  [optional] |
|**cells** | [**List&lt;PriceListCell&gt;**](PriceListCell.md) | Массив значений столбцов в позиции Прайс-листа |  [optional] |



