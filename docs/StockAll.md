

# StockAll

Строка Расширенного отчета об остатках.  Тип каждой строки задается её `meta.type` (product, variant или consignment). Параметр запроса `groupBy` определяет набор возможных типов в выдаче: `product` — только товары; `variant` — товары и модификации; `consignment` — товары, модификации и партии. 

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**name** | **String** | Наименование |  [optional] |
|**code** | **String** | Код |  [optional] |
|**article** | **String** | Артикул |  [optional] |
|**externalCode** | **String** | Внешний код сущности, по которой выводится остаток |  [optional] |
|**folder** | [**ProductFolder**](ProductFolder.md) |  |  [optional] |
|**image** | [**Image**](Image.md) |  |  [optional] |
|**uom** | [**Uom**](Uom.md) |  |  [optional] |
|**stock** | **Double** | Остаток |  [optional] |
|**inTransit** | **Double** | Ожидание |  [optional] |
|**reserve** | **Double** | Резерв |  [optional] |
|**quantity** | **Double** | Доступно |  [optional] |
|**stockDays** | **Integer** | Количество дней на складе |  [optional] |
|**price** | **Double** | Себестоимость в копейках |  [optional] |
|**salePrice** | **Double** | Цена продажи |  [optional] |



