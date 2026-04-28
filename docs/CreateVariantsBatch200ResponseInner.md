

# CreateVariantsBatch200ResponseInner


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**id** | **UUID** | ID Модификации |  [optional] [readonly] |
|**accountId** | **UUID** | ID учетной записи |  [optional] [readonly] |
|**updated** | **String** | Момент последнего обновления сущности |  [optional] [readonly] |
|**name** | **String** | Наименование Модификации |  [optional] |
|**code** | **String** | Код Модификации |  [optional] |
|**externalCode** | **String** | Внешний код Модификации |  [optional] |
|**archived** | **Boolean** | Добавлена ли Модификация в архив |  [optional] |
|**description** | **String** | Описание Модификации |  [optional] |
|**discountProhibited** | **Boolean** | Признак запрета скидок |  [optional] |
|**product** | [**Product**](Product.md) |  |  [optional] |
|**characteristics** | [**List&lt;VariantCharacteristicValue&gt;**](VariantCharacteristicValue.md) | Характеристики Модификации |  [optional] |
|**salePrices** | [**List&lt;SalePrice&gt;**](SalePrice.md) | Цены продажи |  [optional] |
|**buyPrice** | [**BuyPrice**](BuyPrice.md) | Закупочная цена |  [optional] |
|**minPrice** | [**MinPrice**](MinPrice.md) |  |  [optional] |
|**barcodes** | [**List&lt;Barcode&gt;**](Barcode.md) | Штрихкоды Модификации |  [optional] |
|**packs** | [**List&lt;VariantPack&gt;**](VariantPack.md) | Упаковки Модификации |  [optional] |
|**images** | [**ImageList**](ImageList.md) | Массив метаданных Изображений |  [optional] |
|**minimumStock** | [**MinimumStockAbstract**](MinimumStockAbstract.md) | Неснижаемый остаток. Не выводится по умолчанию. Для получения передайте параметр &#x60;?fields&#x3D;minimumStock&#x60;.  |  [optional] |
|**things** | **List&lt;String&gt;** | Серийные номера |  [optional] |
|**errors** | [**List&lt;ErrorErrorsInner&gt;**](ErrorErrorsInner.md) |  |  |



