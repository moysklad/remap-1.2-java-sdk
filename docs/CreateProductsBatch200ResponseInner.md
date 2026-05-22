

# CreateProductsBatch200ResponseInner


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**id** | **UUID** | ID товара |  [optional] [readonly] |
|**accountId** | **UUID** | ID учетной записи |  [optional] [readonly] |
|**alcoholic** | [**ProductAlcoholic**](ProductAlcoholic.md) |  |  [optional] |
|**archived** | **Boolean** | Добавлен ли товар в архив |  [optional] |
|**tobacco** | **Boolean** | Признак товара, как табачной продукции |  [optional] [readonly] |
|**name** | **String** | Наименование товара |  [optional] |
|**code** | **String** | Код товара |  [optional] |
|**externalCode** | **String** | Внешний код товара |  [optional] |
|**pathName** | **String** | Наименование группы, в которую входит товар |  [optional] [readonly] |
|**article** | **String** | Артикул |  [optional] |
|**description** | **String** | Описание товара |  [optional] |
|**vat** | **Integer** | НДС % |  [optional] |
|**vatEnabled** | **Boolean** | Включен ли НДС для товара |  [optional] |
|**useParentVat** | **Boolean** | Используется ли ставка НДС родительской группы |  [optional] |
|**effectiveVat** | **Integer** | Реальный НДС % |  [optional] [readonly] |
|**effectiveVatEnabled** | **Boolean** | Дополнительный признак для определения разграничения реального НДС |  [optional] [readonly] |
|**discountProhibited** | **Boolean** | Признак запрета скидок |  [optional] |
|**variantsCount** | **Integer** | Количество модификаций у данного товара |  [optional] [readonly] |
|**isSerialTrackable** | **Boolean** | Учет по серийным номерам |  [optional] |
|**shared** | **Boolean** | Общий доступ |  [optional] |
|**group** | [**Group**](Group.md) |  |  [optional] |
|**owner** | [**Employee**](Employee.md) | Метаданные владельца (Сотрудника) |  [optional] |
|**updated** | **String** | Момент последнего обновления сущности |  [optional] [readonly] |
|**weight** | **Float** | Вес |  [optional] |
|**volume** | **Double** | Объем |  [optional] |
|**buyPrice** | [**BuyPrice**](BuyPrice.md) |  |  [optional] |
|**salePrices** | [**List&lt;SalePrice&gt;**](SalePrice.md) | Цены продажи |  [optional] |
|**supplier** | [**Counterparty**](Counterparty.md) | Метаданные контрагента-поставщика |  [optional] |
|**country** | [**Country**](Country.md) | Метаданные Страны |  [optional] |
|**uom** | [**Uom**](Uom.md) | Метаданные единиц измерения |  [optional] |
|**productFolder** | [**ProductFolder**](ProductFolder.md) | Метаданные группы Товара |  [optional] |
|**images** | [**ImageList**](ImageList.md) | Массив изображений |  [optional] |
|**files** | [**FileList**](FileList.md) | Метаданные массива Файлов |  [optional] |
|**barcodes** | [**List&lt;Barcode&gt;**](Barcode.md) | Штрихкоды товара |  [optional] |
|**packs** | [**List&lt;Pack&gt;**](Pack.md) | Упаковки товара |  [optional] |
|**trackingType** | **String** | Тип маркируемой продукции. Известные значения описаны в TrackingType |  [optional] |
|**tnved** | **String** | Код ТН ВЭД |  [optional] |
|**paymentItemType** | **String** | Признак предмета расчета. Известные значения описаны в PaymentItemType |  [optional] |
|**taxSystem** | **String** | Код системы налогообложения. Известные значения описаны в TaxSystem |  [optional] |
|**attributes** | [**List&lt;AttributeAbstract&gt;**](AttributeAbstract.md) | Дополнительные поля |  [optional] |
|**minimumStock** | [**MinimumStockAbstract**](MinimumStockAbstract.md) | Неснижаемый остаток. Не выводится по умолчанию. Для получения передайте параметр &#x60;?fields&#x3D;minimumStock&#x60;.  |  [optional] |
|**minPrice** | [**MinPrice**](MinPrice.md) |  |  [optional] |
|**weighed** | **Boolean** | Поле, показывающее является ли товар весовым |  [optional] |
|**onTap** | **Boolean** | Поле, показывающее является ли товар разливным |  [optional] |
|**partialDisposal** | **Boolean** | Управление состоянием частичного выбытия маркированного товара |  [optional] |
|**things** | **List&lt;String&gt;** | Серийные номера |  [optional] |
|**syncId** | **UUID** | ID синхронизации |  [optional] |
|**ppeType** | **String** | Код вида номенклатурной классификации медицинских средств индивидуальной защиты. Известные значения описаны в PpeType |  [optional] |
|**errors** | [**List&lt;ErrorErrorsInner&gt;**](ErrorErrorsInner.md) |  |  |



