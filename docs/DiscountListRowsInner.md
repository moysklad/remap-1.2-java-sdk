

# DiscountListRowsInner

Логический вид строки в JSON задаётся `meta.type` (см. описание массива `rows` выше).  Здесь `anyOf`, а не `oneOf`: у вариантов общий базис (`DiscountBase`), минимальный объект одновременно удовлетворяет нескольким веткам, и строгие валидаторы (в т.ч. Schemathesis) падают с ошибкой «валидно более чем по одной схеме `oneOf`».  Сгенерированный PHP SDK для такого `items` обычно выдаёт один **объединённый** тип строки (все поля вариантов в одной модели), а не `Discount` / `PersonalDiscount` на элемент. Отображение в доменные классы по `meta.type` — ответственность приложения (ручной разбор или повторный decode в нужную модель). 

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**allProducts** | **Boolean** | Для всех ли товаров скидка |  [optional] |
|**assortment** | [**List&lt;DiscountAssortmentItem&gt;**](DiscountAssortmentItem.md) | Товары, услуги и модификации со скидкой |  [optional] |
|**productFolders** | [**List&lt;ProductFolder&gt;**](ProductFolder.md) | Группы товаров со скидкой |  [optional] |
|**id** | **UUID** | ID дополнительного поля |  [optional] [readonly] |
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**accountId** | **UUID** | ID учетной записи |  [optional] [readonly] |
|**name** | **String** | Наименование товара |  [optional] |
|**active** | **Boolean** | Включена ли скидка |  [optional] |
|**allAgents** | **Boolean** | Для всех ли агентов скидка |  [optional] |
|**agentTags** | **List&lt;String&gt;** | Тэги агентов |  [optional] |
|**usePriceType** | **Boolean** | Использовать ли специальную цену |  [optional] |
|**discount** | **Float** | Процент скидки (используется при usePriceType&#x3D;false) |  [optional] |
|**specialPrice** | [**Object**](Object.md) | Спец. цена (используется при usePriceType&#x3D;true) |  [optional] |
|**levels** | [**List&lt;Object&gt;**](Object.md) | Проценты скидок при определенной сумме продаж |  [optional] |
|**earnRateRoublesToPoint** | **Integer** | Курс начисления |  [optional] |
|**earnWhileRedeeming** | **Boolean** | Разрешить одновременное начисление и списание бонусов |  [optional] |
|**postponedBonusesDelayDays** | **Integer** | Баллы начисляются через N дней |  [optional] |
|**spendRatePointsToRouble** | **Integer** | Курс списания |  [optional] |
|**welcomeBonusesEnabled** | **Boolean** | Возможность начисления приветственных баллов |  [optional] |
|**welcomeBonusesValue** | **Integer** | Количество приветственных баллов, начисляемых участникам бонусной программы |  [optional] |
|**welcomeBonusesMode** | **String** | Условие начисления приветственных баллов. Известные значения описаны в WelcomeBonusesMode |  [optional] |
|**maxPaidRatePercents** | **Integer** | Максимальный процент оплаты баллами |  [optional] |



