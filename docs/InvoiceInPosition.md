

# InvoiceInPosition

Позиция Счета поставщику

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**id** | **UUID** | ID позиции |  [optional] [readonly] |
|**accountId** | **UUID** | ID учетной записи |  [optional] [readonly] |
|**quantity** | **Double** | Количество товаров/услуг данного вида в позиции |  [optional] |
|**price** | **Double** | Цена товара/услуги в копейках |  [optional] |
|**discount** | **Double** | Процент скидки или наценки |  [optional] |
|**vat** | **Integer** | НДС, которым облагается текущая позиция |  [optional] |
|**vatEnabled** | **Boolean** | Включен ли НДС для позиции |  [optional] |
|**assortment** | [**Assortment**](Assortment.md) |  |  [optional] |
|**pack** | [**Pack**](Pack.md) | Упаковка Товара |  [optional] |



