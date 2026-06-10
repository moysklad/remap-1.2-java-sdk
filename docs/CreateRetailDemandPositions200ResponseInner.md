

# CreateRetailDemandPositions200ResponseInner


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**id** | **UUID** | ID позиции |  [optional] [readonly] |
|**accountId** | **UUID** | ID учетной записи |  [optional] [readonly] |
|**assortment** | [**Assortment**](Assortment.md) |  |  [optional] |
|**cost** | **Integer** | Себестоимость (только для услуг) |  [optional] |
|**declaration** | [**List&lt;DeclarationInner&gt;**](DeclarationInner.md) | Информация о прослеживаемости импортных товаров. Не входит в ответ по умолчанию; может быть возвращена только при явном запросе &#x60;fields&#x3D;declaration&#x60;. Только для чтения.  |  [optional] [readonly] |
|**discount** | **Double** | Процент скидки или наценки. Наценка указывается отрицательным числом (например, &#x60;-10&#x60; задаёт наценку 10%). |  [optional] |
|**pack** | [**Pack**](Pack.md) | Упаковка товара |  [optional] |
|**price** | **Double** | Цена товара/услуги в копейках |  [optional] |
|**quantity** | **Double** | Количество товаров/услуг данного вида в позиции. Если позиция является товаром с учётом по серийным номерам, значение всегда равно количеству серийных номеров для этой позиции в документе.  |  [optional] |
|**things** | **List&lt;String&gt;** | Серийные номера. Игнорируется, если товар позиции не на серийном учёте; иначе количество единиц в позиции совпадает с числом переданных серийных номеров.  |  [optional] |
|**vat** | **Integer** | НДС, которым облагается текущая позиция |  [optional] |
|**vatEnabled** | **Boolean** | Включен ли НДС для позиции |  [optional] |
|**errors** | [**List&lt;ErrorErrorsInner&gt;**](ErrorErrorsInner.md) |  |  |



