

# Bundle

Комплект

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**id** | **UUID** | ID Комплекта |  [optional] [readonly] |
|**accountId** | **UUID** | ID учетной записи |  [optional] [readonly] |
|**name** | **String** | Наименование Комплекта |  [optional] |
|**code** | **String** | Код Комплекта |  [optional] |
|**externalCode** | **String** | Внешний код Комплекта |  [optional] |
|**syncId** | **UUID** | ID синхронизации |  [optional] |
|**updated** | **String** | Момент последнего обновления сущности |  [optional] [readonly] |
|**archived** | **Boolean** | Добавлен ли Комплект в архив |  [optional] |
|**shared** | **Boolean** | Общий доступ |  [optional] |
|**description** | **String** | Описание Комплекта |  [optional] |
|**article** | **String** | Артикул |  [optional] |
|**pathName** | **String** | Наименование группы, в которую входит Комплект |  [optional] [readonly] |
|**discountProhibited** | **Boolean** | Признак запрета скидок |  [optional] |
|**partialDisposal** | **Boolean** | Управление состоянием частичного выбытия маркированного товара |  [optional] |
|**vat** | **Integer** | НДС % |  [optional] |
|**vatEnabled** | **Boolean** | Включен ли НДС для товара |  [optional] |
|**useParentVat** | **Boolean** | Используется ли ставка НДС родительской группы |  [optional] |
|**effectiveVat** | **Integer** | Реальный НДС % |  [optional] [readonly] |
|**effectiveVatEnabled** | **Boolean** | Дополнительный признак для определения разграничения реального НДС |  [optional] [readonly] |
|**paymentItemType** | **String** | Признак предмета расчета. Известные значения описаны в PaymentItemType |  [optional] |
|**taxSystem** | **String** | Код системы налогообложения. Известные значения описаны в TaxSystem |  [optional] |
|**trackingType** | **String** | Тип маркируемой продукции. Известные значения описаны в TrackingType |  [optional] |
|**tnved** | **String** | Код ТН ВЭД |  [optional] |
|**weight** | **Float** | Вес |  [optional] |
|**volume** | **Float** | Объем |  [optional] |
|**group** | [**Group**](Group.md) |  |  [optional] |
|**owner** | [**Employee**](Employee.md) | Метаданные владельца (Сотрудника) |  [optional] |
|**country** | [**Country**](Country.md) | Метаданные Страны |  [optional] |
|**uom** | [**Uom**](Uom.md) | Единицы измерения |  [optional] |
|**productFolder** | [**ProductFolder**](ProductFolder.md) | Метаданные группы Комплекта |  [optional] |
|**images** | [**ImageList**](ImageList.md) | Массив метаданных Изображений |  [optional] |
|**files** | [**FileList**](FileList.md) | Метаданные массива Файлов |  [optional] |
|**barcodes** | [**List&lt;Barcode&gt;**](Barcode.md) | Штрихкоды Комплекта |  [optional] |
|**packs** | [**List&lt;Pack&gt;**](Pack.md) | Упаковки Комплекта |  [optional] |
|**salePrices** | [**List&lt;SalePrice&gt;**](SalePrice.md) | Цены продажи |  [optional] |
|**buyPrice** | [**BuyPrice**](BuyPrice.md) |  |  [optional] |
|**minPrice** | [**MinPrice**](MinPrice.md) |  |  [optional] |
|**overhead** | [**BundleOverhead**](BundleOverhead.md) |  |  [optional] |
|**attributes** | [**List&lt;AttributeAbstract&gt;**](AttributeAbstract.md) | Коллекция метаданных доп. полей |  [optional] |
|**components** | **BundleComponentList** | Массив компонентов Комплекта |  [optional] |



