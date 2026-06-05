

# CreateEnterPositionsRequest


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**id** | **UUID** | ID позиции |  [optional] [readonly] |
|**accountId** | **UUID** | ID учетной записи |  [optional] [readonly] |
|**assortment** | [**Assortment**](Assortment.md) |  |  [optional] |
|**country** | [**Country**](Country.md) | Метаданные страны |  [optional] |
|**gtd** | [**Gtd**](Gtd.md) |  |  [optional] |
|**overhead** | **Integer** | Накладные расходы |  [optional] [readonly] |
|**pack** | [**Pack**](Pack.md) | Упаковка Товара |  [optional] |
|**price** | **Double** | Цена товара/услуги в копейках |  [optional] |
|**quantity** | **Double** | Количество товаров данного вида в позиции |  [optional] |
|**reason** | **String** | Причина оприходования данной позиции |  [optional] |
|**slot** | [**StoreSlot**](StoreSlot.md) | Ячейка на складе |  [optional] |
|**things** | **List&lt;String&gt;** | Серийные номера. Игнорируется, если товар позиции не на серийном учёте; иначе количество единиц в позиции совпадает с числом переданных серийных номеров.  |  [optional] |



