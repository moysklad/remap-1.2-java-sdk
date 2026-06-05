

# FactureOut

Счет-фактура выданный (factureout)

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**id** | **UUID** | ID Счета-фактуры выданного |  [optional] [readonly] |
|**accountId** | **UUID** | ID учетной записи |  [optional] [readonly] |
|**agent** | [**Agent**](Agent.md) | Метаданные контрагента или юрлица |  [optional] |
|**applicable** | **Boolean** | Отметка о проведении |  [optional] |
|**attributes** | [**List&lt;AttributeAbstract&gt;**](AttributeAbstract.md) | Коллекция метаданных доп. полей |  [optional] |
|**code** | **String** | Код Счета-фактуры выданного |  [optional] |
|**contract** | [**Contract**](Contract.md) | Метаданные договора |  [optional] |
|**created** | **String** | Дата создания |  [optional] [readonly] |
|**deleted** | **String** | Момент последнего удаления Счета-фактуры выданного |  [optional] [readonly] |
|**description** | **String** | Комментарий Счета-фактуры выданного |  [optional] |
|**externalCode** | **String** | Внешний код Счета-фактуры выданного |  [optional] |
|**files** | [**FileList**](FileList.md) | Метаданные массива файлов |  [optional] |
|**group** | [**Group**](Group.md) |  |  [optional] |
|**moment** | **String** | Дата документа |  [optional] |
|**name** | **String** | Наименование Счета-фактуры выданного |  [optional] |
|**organization** | [**Organization**](Organization.md) |  |  [optional] |
|**owner** | [**Employee**](Employee.md) | Владелец (Сотрудник) |  [optional] |
|**printed** | **Boolean** | Напечатан ли документ |  [optional] [readonly] |
|**published** | **Boolean** | Опубликован ли документ |  [optional] [readonly] |
|**rate** | [**CurrencyRate**](CurrencyRate.md) |  |  [optional] |
|**shared** | **Boolean** | Общий доступ |  [optional] |
|**state** | [**State**](State.md) | Метаданные статуса Счета-фактуры выданного |  [optional] |
|**stateContractId** | **String** | Идентификатор государственного контракта, договора (соглашения) |  [optional] |
|**sum** | **Double** | Сумма Счета-фактуры выданного в копейках |  [optional] [readonly] |
|**syncId** | **UUID** | ID синхронизации |  [optional] |
|**updated** | **String** | Момент последнего обновления Счета-фактуры выданного |  [optional] [readonly] |
|**advancePaymentVat** | **Integer** | Ставка НДС для авансового платежа (в процентах) |  [optional] |
|**paymentPurpose** | **String** | Назначение платежа |  [optional] |
|**vatSum** | **Double** | Сумма включая НДС |  [optional] [readonly] |
|**demands** | [**List&lt;Demand&gt;**](Demand.md) | Связанные отгрузки (метаданные) |  [optional] |
|**payments** | [**List&lt;PaymentIn&gt;**](PaymentIn.md) | Связанные входящие платежи (метаданные) |  [optional] |
|**returns** | [**List&lt;PurchaseReturn&gt;**](PurchaseReturn.md) | Связанные возвраты поставщикам (метаданные) |  [optional] |
|**consignee** | [**Agent**](Agent.md) | Грузополучатель (контрагент или юрлицо) |  [optional] |
|**paymentNumber** | **String** | Название платежного документа |  [optional] |
|**paymentDate** | **String** | Дата платежного документа |  [optional] |



