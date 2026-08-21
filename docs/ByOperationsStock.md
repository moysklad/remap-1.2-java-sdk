

# ByOperationsStock

Строка отчета по документам номенклатуры, отображающего остатки

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**assortment** | [**ByOperationsStockAssortment**](ByOperationsStockAssortment.md) |  |  [optional] |
|**operation** | [**ByOperationsStockOperation**](ByOperationsStockOperation.md) |  |  [optional] |
|**moment** | **String** | Дата документа |  [optional] |
|**store** | [**ByOperationsStockStore**](ByOperationsStockStore.md) |  |  [optional] |
|**stock** | **Double** | Остатки |  [optional] |
|**costPerUnit** | **Double** | Себестоимость за единицу. Не возвращается при отсутствии пермиссии «Видеть себестоимость, цену закупки, прибыль товаров».  |  [optional] |
|**sumCost** | **Double** | Сумма себестоимости. Не возвращается при отсутствии пермиссии «Видеть себестоимость, цену закупки, прибыль товаров».  |  [optional] |
|**avgStockDays** | **Double** | Количество дней на складе |  [optional] |



