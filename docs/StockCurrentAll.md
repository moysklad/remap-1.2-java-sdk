

# StockCurrentAll

Строка краткого отчета об остатках по всей номенклатуре. В ответе возвращается только одно поле значения остатка, выбранное параметром `stockType`. 

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**assortmentId** | **UUID** | ID товара, модификации или партии |  [optional] |
|**stock** | **Double** | Физический остаток на складах, без учета резерва и ожидания |  [optional] |
|**freeStock** | **Double** | Остаток на складах за вычетом резерва |  [optional] |
|**quantity** | **Double** | Доступно (учитывает резерв и ожидания) |  [optional] |
|**reserve** | **Double** | Резерв |  [optional] |
|**inTransit** | **Double** | Ожидание |  [optional] |



