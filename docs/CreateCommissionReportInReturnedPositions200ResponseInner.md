

# CreateCommissionReportInReturnedPositions200ResponseInner


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**id** | **UUID** | ID позиции |  [optional] [readonly] |
|**accountId** | **UUID** | ID учетной записи |  [optional] [readonly] |
|**quantity** | **Double** | Количество товаров/услуг в позиции |  [optional] |
|**price** | **Double** | Цена товара в копейках |  [optional] |
|**reward** | **Double** | Вознаграждение |  [optional] |
|**vat** | **Integer** | НДС для позиции |  [optional] |
|**vatEnabled** | **Boolean** | Включен ли НДС для позиции |  [optional] |
|**assortment** | [**ProductMarker**](ProductMarker.md) | Метаданные товара/партии/модификации/комплекта, которую представляет позиция |  [optional] |
|**errors** | [**List&lt;Error&gt;**](Error.md) |  |  |



