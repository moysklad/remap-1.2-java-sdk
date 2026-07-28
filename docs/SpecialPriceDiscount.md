

# SpecialPriceDiscount

Специальная цена (specialpricediscount)

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**id** | **UUID** | ID дополнительного поля |  [optional] [readonly] |
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**productFolders** | [**List&lt;ProductFolder&gt;**](ProductFolder.md) | Группы товаров со скидкой |  [optional] |
|**usePriceType** | **Boolean** | Использовать ли специальную цену |  [optional] |
|**discount** | **Float** | Процент скидки (используется при usePriceType&#x3D;false) |  [optional] |
|**specialPrice** | [**SpecialPriceDiscountSpecialPrice**](SpecialPriceDiscountSpecialPrice.md) |  |  [optional] |



