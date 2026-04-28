

# SpecialPriceDiscount

Специальная цена (specialpricediscount)

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**assortment** | [**List&lt;DiscountAssortmentItem&gt;**](DiscountAssortmentItem.md) | Товары, услуги и модификации со скидкой |  [optional] |
|**productFolders** | [**List&lt;ProductFolder&gt;**](ProductFolder.md) | Группы товаров со скидкой |  [optional] |
|**allProducts** | **Boolean** | Для всех ли товаров скидка |  [optional] |
|**usePriceType** | **Boolean** | Использовать ли специальную цену |  [optional] |
|**discount** | **Float** | Процент скидки (используется при usePriceType&#x3D;false) |  [optional] |
|**specialPrice** | [**Object**](Object.md) | Спец. цена (используется при usePriceType&#x3D;true) |  [optional] |
|**id** | **UUID** | ID дополнительного поля |  [optional] [readonly] |
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**accountId** | **UUID** | ID учетной записи |  [optional] [readonly] |
|**name** | **String** | Наименование товара |  [optional] |
|**active** | **Boolean** | Включена ли скидка |  [optional] |
|**allAgents** | **Boolean** | Для всех ли агентов скидка |  [optional] |
|**agentTags** | **List&lt;String&gt;** | Тэги агентов |  [optional] |



