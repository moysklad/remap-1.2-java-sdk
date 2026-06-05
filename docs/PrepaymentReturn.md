

# PrepaymentReturn

Возврат предоплаты

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**id** | **UUID** | ID Возврата предоплаты |  [optional] [readonly] |
|**accountId** | **UUID** | ID учетной записи |  [optional] [readonly] |
|**name** | **String** | Наименование Возврата предоплаты |  [optional] |
|**code** | **String** | Код Возврата предоплаты |  [optional] |
|**externalCode** | **String** | Внешний код Возврата предоплаты |  [optional] |
|**syncId** | **UUID** | ID синхронизации |  [optional] |
|**description** | **String** | Комментарий Возврата предоплаты |  [optional] |
|**created** | **String** | Дата создания |  [optional] [readonly] |
|**deleted** | **String** | Момент последнего удаления Возврата предоплаты |  [optional] [readonly] |
|**updated** | **String** | Момент последнего обновления Возврата предоплаты |  [optional] [readonly] |
|**moment** | **String** | Дата документа |  [optional] |
|**applicable** | **Boolean** | Отметка о проведении |  [optional] |
|**printed** | **Boolean** | Напечатан ли документ |  [optional] [readonly] |
|**published** | **Boolean** | Опубликован ли документ |  [optional] [readonly] |
|**shared** | **Boolean** | Общий доступ |  [optional] |
|**vatEnabled** | **Boolean** | Учитывается ли НДС |  [optional] |
|**vatIncluded** | **Boolean** | Включен ли НДС в цену |  [optional] |
|**vatSum** | **Double** | Сумма НДС |  [optional] |
|**sum** | **Double** | Сумма Возврата предоплаты в копейках |  [optional] [readonly] |
|**cashSum** | **Double** | Оплачено наличными |  [optional] |
|**noCashSum** | **Double** | Оплачено картой |  [optional] |
|**qrSum** | **Double** | Оплачено по QR-коду |  [optional] |
|**agent** | [**Agent**](Agent.md) | Метаданные Контрагента или юрлица |  [optional] |
|**organization** | [**Organization**](Organization.md) |  |  [optional] |
|**owner** | [**Employee**](Employee.md) | Владелец (Сотрудник) |  [optional] |
|**group** | [**Group**](Group.md) |  |  [optional] |
|**attributes** | [**List&lt;AttributeAbstract&gt;**](AttributeAbstract.md) | Коллекция метаданных доп. полей |  [optional] |
|**files** | [**FileList**](FileList.md) | Метаданные массива Файлов |  [optional] |
|**rate** | **CurrencyRate** | Валюта документа.  Если значение курса валюты не указано, используется курс из справочника валют.  |  [optional] |
|**positions** | [**PrepaymentReturnPositionList**](PrepaymentReturnPositionList.md) |  |  [optional] |
|**prepayment** | [**Prepayment**](Prepayment.md) |  |  [optional] |
|**retailShift** | [**RetailShift**](RetailShift.md) |  |  [optional] |
|**retailStore** | [**RetailStore**](RetailStore.md) |  |  [optional] |
|**state** | [**State**](State.md) | Метаданные статуса Возврата предоплаты |  [optional] |
|**taxSystem** | **String** | Код системы налогообложения. Известные значения описаны в TaxSystem |  [optional] |



