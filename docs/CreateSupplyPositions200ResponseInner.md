

# CreateSupplyPositions200ResponseInner


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**id** | **UUID** | ID позиции |  [optional] [readonly] |
|**accountId** | **UUID** | ID учетной записи |  [optional] [readonly] |
|**assortment** | [**Assortment**](Assortment.md) |  |  [optional] |
|**country** | [**Country**](Country.md) | Метаданные страны |  [optional] |
|**discount** | **Double** | Процент скидки или наценки |  [optional] |
|**gtd** | [**Gtd**](Gtd.md) |  |  [optional] |
|**pack** | [**Pack**](Pack.md) | Упаковка Товара |  [optional] |
|**price** | **Double** | Цена товара/услуги в копейках |  [optional] |
|**quantity** | **Double** | Количество товаров/услуг данного вида в позиции. Если позиция — товар с учётом по серийным номерам, значение всегда равно количеству серийных номеров для этой позиции в документе.  |  [optional] |
|**slot** | [**StoreSlot**](StoreSlot.md) | Ячейка на складе |  [optional] |
|**things** | **List&lt;String&gt;** | Серийные номера. Игнорируется, если товар позиции не на серийном учёте; иначе количество единиц в позиции совпадает с числом переданных серийных номеров.  |  [optional] |
|**trackingCodes** | [**List&lt;PositionTrackingCode&gt;**](PositionTrackingCode.md) | Коды маркировки товаров и транспортных упаковок (иерархическая структура). Количество кодов маркировки не влияет на поле quantity позиции.  |  [optional] |
|**overhead** | **Integer** | Накладные расходы по позиции. Если позиции Приемки не заданы, накладные расходы на уровне документа задать нельзя.  |  [optional] [readonly] |
|**vat** | **Integer** | НДС, которым облагается текущая позиция |  [optional] |
|**vatEnabled** | **Boolean** | Включён ли НДС для позиции. Пара &#x60;(vat &#x3D; 0, vatEnabled &#x3D; false)&#x60; соответствует НДС «без НДС»; &#x60;(vat &#x3D; 0, vatEnabled &#x3D; true)&#x60; — НДС 0%.  |  [optional] |
|**errors** | [**List&lt;ErrorErrorsInner&gt;**](ErrorErrorsInner.md) |  |  |



