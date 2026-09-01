

# CustomerOrderPosition

Позиция Заказа покупателя

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**id** | **UUID** | ID позиции |  [optional] |
|**accountId** | **UUID** | ID учетной записи |  [optional] [readonly] |
|**quantity** | **Double** | Количество товаров данного вида в позиции |  [optional] |
|**price** | **Double** | Цена товара/услуги в копейках |  [optional] |
|**discount** | **Double** | Процент скидки или наценки |  [optional] |
|**reserve** | **Double** | Резерв данной позиции |  [optional] |
|**shipped** | **Double** | Доставлено |  [optional] [readonly] |
|**vat** | **Integer** | НДС, которым облагается текущая позиция |  [optional] |
|**vatEnabled** | **Boolean** | Включен ли НДС для позиции |  [optional] |
|**taxSystem** | **String** | Код системы налогообложения. Известные значения описаны в TaxSystem |  [optional] |
|**assortment** | [**ProductMarker**](ProductMarker.md) | Метаданные товара/услуги/модификации/комплекта, которую представляет собой позиция |  [optional] |
|**pack** | [**Pack**](Pack.md) | Упаковка Товара |  [optional] |
|**stock** | [**PositionStock**](PositionStock.md) | Остатки и себестоимость позиции. Не выводится по умолчанию. Для получения передайте параметр &#x60;?fields&#x3D;stock&#x60;.  |  [optional] |



