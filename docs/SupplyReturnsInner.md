

# SupplyReturnsInner


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
|**payedSum** | **Double** | Сумма входящих платежей по Возврату поставщику |  [optional] [readonly] |
|**organization** | [**Organization**](Organization.md) |  |  [optional] |
|**organizationAccount** | [**Account**](Account.md) | Метаданные счета юрлица |  [optional] |
|**agent** | [**Agent**](Agent.md) | Метаданные Контрагента или юрлица |  [optional] |
|**agentAccount** | [**Account**](Account.md) | Метаданные счета контрагента |  [optional] |
|**store** | [**Store**](Store.md) |  |  [optional] |
|**state** | [**State**](State.md) | Метаданные статуса Возврата предоплаты |  [optional] |
|**contract** | [**Contract**](Contract.md) | Метаданные договора |  [optional] |
|**project** | [**Project**](Project.md) | Метаданные проекта |  [optional] |
|**owner** | [**Employee**](Employee.md) | Владелец (Сотрудник) |  [optional] |
|**group** | [**Group**](Group.md) |  |  [optional] |
|**attributes** | [**List&lt;AttributeAbstract&gt;**](AttributeAbstract.md) | Коллекция метаданных доп. полей |  [optional] |
|**files** | [**FileList**](FileList.md) | Метаданные массива Файлов |  [optional] |
|**rate** | **CurrencyRate** |  |  [optional] |
|**positions** | [**PrepaymentReturnPositionList**](PrepaymentReturnPositionList.md) |  |  [optional] |
|**salesChannel** | [**SalesChannel**](SalesChannel.md) | Метаданные канала продаж |  [optional] |
|**demand** | [**Demand**](Demand.md) | Отгрузка, по которой произошел возврат |  [optional] |
|**losses** | [**List&lt;Loss&gt;**](Loss.md) | Массив ссылок на связанные списания |  [optional] |
|**payments** | [**List&lt;CustomerOrderPaymentsInner&gt;**](CustomerOrderPaymentsInner.md) | Массив ссылок на связанные платежи |  [optional] |
|**factureOut** | [**FactureOut**](FactureOut.md) | Счет-фактура выданный, с которым связан этот возврат |  [optional] |
|**supply** | [**Supply**](Supply.md) | Приемка, по которой произошел возврат |  [optional] |
|**factureIn** | [**FactureIn**](FactureIn.md) | Счет-фактура полученный, с которым связан этот возврат |  [optional] |
|**cashSum** | **Double** | Оплачено наличными |  [optional] |
|**noCashSum** | **Double** | Оплачено картой |  [optional] |
|**qrSum** | **Double** | Оплачено по QR-коду |  [optional] |
|**prepayment** | [**Prepayment**](Prepayment.md) |  |  [optional] |
|**retailShift** | [**RetailShift**](RetailShift.md) |  |  [optional] |
|**retailStore** | [**RetailStore**](RetailStore.md) |  |  [optional] |
|**taxSystem** | **String** | Код системы налогообложения. Известные значения описаны в TaxSystem |  [optional] |



