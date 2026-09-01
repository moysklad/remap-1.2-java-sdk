

# LossPosition

Позиция Списания

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**id** | **UUID** | ID позиции |  [optional] |
|**accountId** | **UUID** | ID учетной записи |  [optional] [readonly] |
|**assortment** | [**ProductMarker**](ProductMarker.md) | Метаданные товара/услуги/партии/модификации, которую представляет собой позиция |  [optional] |
|**declaration** | [**List&lt;DeclarationInner&gt;**](DeclarationInner.md) | Информация о прослеживаемости импортных товаров. Не входит в ответ по умолчанию; может быть возвращена только при явном запросе &#x60;fields&#x3D;declaration&#x60;. Только для чтения.  |  [optional] [readonly] |
|**pack** | [**Pack**](Pack.md) | Упаковка Товара |  [optional] |
|**price** | **Double** | Цена товара/услуги в копейках |  [optional] |
|**quantity** | **Double** | Количество товаров/услуг данного вида в позиции |  [optional] |
|**reason** | **String** | Причина списания данной позиции |  [optional] |
|**slot** | [**StoreSlot**](StoreSlot.md) | Ячейка на складе |  [optional] |
|**things** | **List&lt;String&gt;** | Серийные номера |  [optional] |



