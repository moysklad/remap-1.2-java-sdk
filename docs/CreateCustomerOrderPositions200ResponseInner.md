

# CreateCustomerOrderPositions200ResponseInner


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**id** | **UUID** | ID позиции |  [optional] [readonly] |
|**accountId** | **UUID** | ID учетной записи |  [optional] [readonly] |
|**quantity** | **Double** | Количество товаров данного вида в позиции |  [optional] |
|**price** | **Double** | Цена товара/услуги в копейках |  [optional] |
|**discount** | **Double** | Процент скидки или наценки |  [optional] |
|**reserve** | **Double** | Резерв данной позиции |  [optional] |
|**shipped** | **Double** | Доставлено |  [optional] [readonly] |
|**vat** | **Integer** | НДС, которым облагается текущая позиция |  [optional] |
|**vatEnabled** | **Boolean** | Включен ли НДС для позиции |  [optional] |
|**taxSystem** | [**TaxSystemEnum**](#TaxSystemEnum) | Код системы налогообложения |  [optional] |
|**assortment** | [**Assortment**](Assortment.md) |  |  [optional] |
|**pack** | [**Pack**](Pack.md) | Упаковка Товара |  [optional] |
|**stock** | [**PositionStock**](PositionStock.md) | Остатки и себестоимость позиции. Не выводится по умолчанию. Для получения передайте параметр &#x60;?fields&#x3D;stock&#x60;.  |  [optional] |
|**errors** | [**List&lt;ErrorErrorsInner&gt;**](ErrorErrorsInner.md) |  |  |



## Enum: TaxSystemEnum

| Name | Value |
|---- | -----|
| GENERAL_TAX_SYSTEM | &quot;GENERAL_TAX_SYSTEM&quot; |
| SIMPLIFIED_TAX_SYSTEM_INCOME | &quot;SIMPLIFIED_TAX_SYSTEM_INCOME&quot; |
| SIMPLIFIED_TAX_SYSTEM_INCOME_OUTCOME | &quot;SIMPLIFIED_TAX_SYSTEM_INCOME_OUTCOME&quot; |
| UNIFIED_AGRICULTURAL_TAX | &quot;UNIFIED_AGRICULTURAL_TAX&quot; |
| PRESUMPTIVE_TAX_SYSTEM | &quot;PRESUMPTIVE_TAX_SYSTEM&quot; |
| PATENT_BASED | &quot;PATENT_BASED&quot; |



