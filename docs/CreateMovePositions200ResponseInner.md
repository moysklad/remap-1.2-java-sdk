

# CreateMovePositions200ResponseInner


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**id** | **UUID** | ID позиции |  [optional] [readonly] |
|**accountId** | **UUID** | ID учетной записи |  [optional] [readonly] |
|**assortment** | [**Assortment**](Assortment.md) |  |  [optional] |
|**overhead** | **Integer** | Накладные расходы по позиции. Если позиции Перемещения не заданы, накладные расходы на уровне документа задать нельзя.  |  [optional] [readonly] |
|**pack** | [**Pack**](Pack.md) | Упаковка Товара |  [optional] |
|**price** | **Double** | Цена товара/услуги в копейках |  [optional] |
|**quantity** | **Double** | Количество товаров/услуг данного вида в позиции. Если позиция — товар с учётом по серийным номерам, значение всегда равно количеству серийных номеров для этой позиции в документе.  |  [optional] |
|**sourceSlot** | [**StoreSlot**](StoreSlot.md) | Ячейка на складе, с которого совершается перемещение |  [optional] |
|**targetSlot** | [**StoreSlot**](StoreSlot.md) | Ячейка на складе, на который совершается перемещение |  [optional] |
|**things** | **List&lt;String&gt;** | Серийные номера. Игнорируется, если товар позиции не на серийном учёте; иначе количество единиц в позиции совпадает с числом переданных серийных номеров.  |  [optional] |
|**errors** | [**List&lt;ErrorErrorsInner&gt;**](ErrorErrorsInner.md) |  |  |



