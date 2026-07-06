

# RetailSalesReturnPosition

Позиция Розничного возврата

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**id** | **UUID** | ID позиции |  [optional] [readonly] |
|**accountId** | **UUID** | ID учетной записи |  [optional] [readonly] |
|**assortment** | [**Assortment**](Assortment.md) |  |  [optional] |
|**cost** | **Integer** | Себестоимость (выводится, если документ был создан без основания) |  [optional] |
|**discount** | **Double** | Процент скидки или наценки. Наценка указывается отрицательным числом, например &#x60;-10&#x60; задает наценку 10%. |  [optional] |
|**pack** | [**Pack**](Pack.md) | Упаковка Товара |  [optional] |
|**price** | **Double** | Цена товара/услуги в копейках |  [optional] |
|**quantity** | **Double** | Количество товаров/услуг данного вида в позиции. Если позиция - товар с учетом по серийным номерам, значение всегда равно количеству серийных номеров для данной позиции в документе. |  [optional] |
|**things** | **List&lt;String&gt;** | Серийные номера. Игнорируется, если товар позиции не находится на серийном учете; иначе количество единиц в позиции совпадает с числом переданных серийных номеров. |  [optional] |
|**vat** | **Integer** | НДС, которым облагается текущая позиция |  [optional] |
|**vatEnabled** | **Boolean** | Включен ли НДС для позиции. Пара &#x60;(vat &#x3D; 0, vatEnabled &#x3D; false)&#x60; соответствует НДС \&quot;без НДС\&quot;; &#x60;(vat &#x3D; 0, vatEnabled &#x3D; true)&#x60; - НДС 0%. |  [optional] |



