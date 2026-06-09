

# CashInOperationAnyOf3

Счет покупателю + linkedSum

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**id** | **UUID** | ID Счета покупателя |  [optional] [readonly] |
|**accountId** | **UUID** | ID учетной записи |  [optional] [readonly] |
|**name** | **String** | Наименование Счета покупателя |  [optional] |
|**code** | **String** | Код Счета покупателя |  [optional] |
|**externalCode** | **String** | Внешний код Счета покупателя |  [optional] |
|**syncId** | **UUID** | ID синхронизации |  [optional] |
|**description** | **String** | Комментарий Счета покупателя |  [optional] |
|**created** | **String** | Дата создания |  [optional] [readonly] |
|**deleted** | **String** | Момент последнего удаления Счета покупателя |  [optional] [readonly] |
|**updated** | **String** | Момент последнего обновления Счета покупателя |  [optional] [readonly] |
|**moment** | **String** | Дата документа |  [optional] |
|**paymentPlannedMoment** | **String** | Планируемая дата оплаты |  [optional] |
|**applicable** | **Boolean** | Отметка о проведении |  [optional] |
|**printed** | **Boolean** | Напечатан ли документ |  [optional] [readonly] |
|**published** | **Boolean** | Опубликован ли документ |  [optional] [readonly] |
|**shared** | **Boolean** | Общий доступ |  [optional] |
|**vatEnabled** | **Boolean** | Учитывается ли НДС |  [optional] |
|**vatIncluded** | **Boolean** | Включен ли НДС в цену |  [optional] |
|**vatSum** | **Double** | Сумма НДС |  [optional] [readonly] |
|**sum** | **Double** | Сумма Счета в установленной валюте |  [optional] [readonly] |
|**payedSum** | **Double** | Сумма входящих платежей по Счету покупателя |  [optional] [readonly] |
|**shippedSum** | **Double** | Сумма отгруженного |  [optional] [readonly] |
|**organization** | [**Organization**](Organization.md) |  |  [optional] |
|**organizationAccount** | [**Account**](Account.md) | Метаданные счета юрлица |  [optional] |
|**agent** | [**Agent**](Agent.md) | Метаданные контрагента |  [optional] |
|**agentAccount** | [**Account**](Account.md) | Метаданные счета контрагента |  [optional] |
|**store** | [**Store**](Store.md) | Метаданные склада |  [optional] |
|**state** | [**State**](State.md) | Метаданные статуса счета |  [optional] |
|**contract** | [**Contract**](Contract.md) | Метаданные договора |  [optional] |
|**project** | [**Project**](Project.md) | Метаданные проекта |  [optional] |
|**owner** | [**Employee**](Employee.md) | Владелец (Сотрудник) |  [optional] |
|**group** | [**Group**](Group.md) |  |  [optional] |
|**attributes** | [**List&lt;AttributeAbstract&gt;**](AttributeAbstract.md) | Коллекция метаданных доп. полей |  [optional] |
|**files** | [**FileList**](FileList.md) | Метаданные массива Файлов |  [optional] |
|**rate** | [**CurrencyRate**](CurrencyRate.md) |  |  [optional] |
|**positions** | [**InvoiceOutPositionList**](InvoiceOutPositionList.md) |  |  [optional] |
|**salesChannel** | [**SalesChannel**](SalesChannel.md) | Метаданные канала продаж |  [optional] |
|**customerOrder** | [**CustomerOrder**](CustomerOrder.md) | Заказ покупателя, с которым связан Счет покупателю |  [optional] |
|**demands** | [**List&lt;Demand&gt;**](Demand.md) | Массив ссылок на связанные отгрузки |  [optional] |
|**payments** | [**List&lt;CustomerOrderPaymentsInner&gt;**](CustomerOrderPaymentsInner.md) | Массив ссылок на связанные операции |  [optional] |
|**linkedSum** | **Double** | Сумма, оплаченная по данному документу |  |



