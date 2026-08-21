

# StockByStore

Строка отчета «Остатки по складам».  Тип номенклатуры в строке задается `meta.type` (product, variant или consignment). Параметр запроса `groupBy` определяет набор возможных типов в выдаче: `product` — только товары; `variant` — товары и модификации; `consignment` — товары, модификации и партии. 

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**stockByStore** | [**List&lt;StockByStoreItem&gt;**](StockByStoreItem.md) | Остатки по складам. Размерность массива равна количеству складов в системе.  |  [optional] |



