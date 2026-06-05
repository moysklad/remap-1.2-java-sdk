

# Loss

Списание

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**id** | **UUID** | ID Списания |  [optional] [readonly] |
|**accountId** | **UUID** | ID учетной записи |  [optional] [readonly] |
|**applicable** | **Boolean** | Отметка о проведении |  [optional] |
|**attributes** | [**List&lt;AttributeAbstract&gt;**](AttributeAbstract.md) | Коллекция метаданных доп. полей |  [optional] |
|**code** | **String** | Код Списания |  [optional] |
|**created** | **String** | Дата создания |  [optional] [readonly] |
|**deleted** | **String** | Момент последнего удаления Списания |  [optional] [readonly] |
|**description** | **String** | Комментарий Списания |  [optional] |
|**expenseItem** | [**ExpenseItem**](ExpenseItem.md) | Метаданные Статьи расходов |  [optional] [readonly] |
|**externalCode** | **String** | Внешний код Списания |  [optional] |
|**files** | [**FileList**](FileList.md) | Метаданные массива Файлов (Максимальное количество файлов - 100) |  [optional] |
|**group** | [**Group**](Group.md) |  |  [optional] |
|**moment** | **String** | Дата документа |  [optional] |
|**name** | **String** | Наименование Списания |  [optional] |
|**organization** | [**Organization**](Organization.md) |  |  [optional] |
|**owner** | [**Employee**](Employee.md) | Владелец (Сотрудник) |  [optional] |
|**positions** | [**LossPositionList**](LossPositionList.md) |  |  [optional] |
|**printed** | **Boolean** | Напечатан ли документ |  [optional] [readonly] |
|**project** | [**Project**](Project.md) | Метаданные проекта |  [optional] |
|**published** | **Boolean** | Опубликован ли документ |  [optional] [readonly] |
|**rate** | **CurrencyRate** | Валюта документа.  Если значение курса валюты не указано, используется курс из справочника валют.  |  [optional] |
|**shared** | **Boolean** | Общий доступ |  [optional] |
|**state** | [**State**](State.md) | Метаданные статуса Списания |  [optional] |
|**store** | [**Store**](Store.md) |  |  [optional] |
|**sum** | **Double** | Сумма Списания в копейках |  [optional] [readonly] |
|**syncId** | **UUID** | ID синхронизации |  [optional] |
|**updated** | **String** | Момент последнего обновления Списания |  [optional] [readonly] |
|**salesReturn** | [**SalesReturn**](SalesReturn.md) | Связанный со Списанием возврат покупателя |  [optional] |
|**inventory** | [**Inventory**](Inventory.md) | Связанная со Списанием инвентаризация |  [optional] |



