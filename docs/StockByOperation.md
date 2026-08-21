

# StockByOperation

Строка отчета «Остатки по документам».  `meta` — ссылка на документ, по которому выдаются остатки. Поддерживаемые типы документов: demand, customerorder, retaildemand, invoicein, invoiceout, purchaseorder, supply, retailsalesreturn, purchasereturn, salesreturn. 

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**positions** | [**List&lt;StockByOperationPosition&gt;**](StockByOperationPosition.md) | Массив остатков по каждой из позиций документа |  [optional] |



