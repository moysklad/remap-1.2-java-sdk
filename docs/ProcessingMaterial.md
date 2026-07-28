

# ProcessingMaterial

Материал техоперации

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**id** | **UUID** | ID материала техоперации |  [optional] [readonly] |
|**accountId** | **UUID** | ID учетной записи |  [optional] [readonly] |
|**assortment** | [**ProductMarker**](ProductMarker.md) |  |  [optional] |
|**quantity** | **Double** | Количество товаров данного вида в позиции |  [optional] |
|**things** | **List&lt;String&gt;** | Серийные номера. Игнорируется, если товар позиции не на серийном учёте; иначе количество единиц в позиции совпадает с числом переданных серийных номеров.  |  [optional] |



