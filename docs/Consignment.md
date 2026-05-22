

# Consignment

Партия

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**id** | **UUID** | ID Партии |  [optional] [readonly] |
|**accountId** | **UUID** | ID учетной записи |  [optional] [readonly] |
|**archived** | **Boolean** | Добавлена ли Партия в архив |  [optional] |
|**attributes** | [**List&lt;AttributeAbstract&gt;**](AttributeAbstract.md) | Коллекция доп. полей Партии |  [optional] |
|**assortment** | [**Assortment**](Assortment.md) |  |  [optional] |
|**barcodes** | [**List&lt;Barcode&gt;**](Barcode.md) | Штрихкоды Партии |  [optional] |
|**code** | **String** | Код Партии |  [optional] |
|**description** | **String** | Описание Партии |  [optional] |
|**expiryDate** | **String** | Срок годности Партии |  [optional] |
|**externalCode** | **String** | Внешний код Партии |  [optional] |
|**images** | [**ImageList**](ImageList.md) | Массив метаданных Изображений товара, к которому относится данная партия |  [optional] [readonly] |
|**label** | **String** | Метка Партии |  [optional] |
|**name** | **String** | Наименование Партии |  [optional] [readonly] |
|**updated** | **String** | Момент последнего обновления сущности |  [optional] [readonly] |



