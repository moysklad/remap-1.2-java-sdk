

# CommissionReportInReturnedPosition

Позиция возврата на склад комиссионера Полученного отчета комиссионера

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
|**assortment** | [**Assortment**](Assortment.md) |  |  [optional] |



