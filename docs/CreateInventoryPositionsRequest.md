

# CreateInventoryPositionsRequest


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**id** | **UUID** | ID позиции |  [optional] [readonly] |
|**accountId** | **UUID** | ID учетной записи |  [optional] [readonly] |
|**assortment** | [**Assortment**](Assortment.md) |  |  [optional] |
|**calculatedQuantity** | **Double** | Расчетный остаток |  [optional] |
|**correctionAmount** | **Double** | Разница между расчетным остатком и фактическим |  [optional] [readonly] |
|**correctionSum** | **Double** | Избыток/недостача |  [optional] [readonly] |
|**pack** | [**Pack**](Pack.md) | Упаковка Товара |  [optional] |
|**price** | **Double** | Цена товара/услуги в копейках |  [optional] |
|**things** | **List&lt;String&gt;** | Серийные номера. Игнорируется, если товар позиции не на серийном учёте; иначе количество единиц в позиции совпадает с числом переданных серийных номеров.  |  [optional] |
|**quantity** | **Double** | Количество товаров/услуг данного вида в позиции. Если позиция - товар,  у которого включен учет по серийным номерам, то значение в этом поле всегда  будет равно количеству серийных номеров для данной позиции в документе.  |  [optional] |



