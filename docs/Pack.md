

# Pack

Упаковка товара

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**id** | **UUID** | ID упаковки товара. Обязательное при ответе |  [optional] [readonly] |
|**uom** | [**Uom**](Uom.md) |  |  [optional] |
|**quantity** | **Double** | Количество товаров в упаковке. Обязательное при ответе |  [optional] |
|**barcodes** | [**List&lt;Barcode&gt;**](Barcode.md) | Штрихкоды упаковки (не более одного). Без штрихкода поле не выводится. При обновлении переданный массив полностью заменяет штрихкоды упаковки.  |  [optional] |



