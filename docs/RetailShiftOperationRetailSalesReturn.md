

# RetailShiftOperationRetailSalesReturn

Розничный возврат

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**id** | **UUID** | ID Розничного возврата |  [optional] [readonly] |
|**accountId** | **UUID** | ID учетной записи |  [optional] [readonly] |
|**agent** | [**Agent**](Agent.md) | Метаданные контрагента |  [optional] |
|**agentAccount** | [**Account**](Account.md) | Метаданные счета контрагента |  [optional] |
|**applicable** | **Boolean** | Отметка о проведении |  [optional] |
|**attributes** | [**List&lt;AttributeAbstract&gt;**](AttributeAbstract.md) | Коллекция метаданных доп. полей |  [optional] |
|**cashSum** | **Double** | Оплачено наличными |  [optional] |
|**code** | **String** | Код Розничного возврата |  [optional] |
|**contract** | [**Contract**](Contract.md) | Метаданные договора |  [optional] |
|**created** | **String** | Дата создания |  [optional] [readonly] |
|**deleted** | **String** | Момент последнего удаления Розничного возврата |  [optional] [readonly] |
|**demand** | [**RetailDemand**](RetailDemand.md) | Метаданные связанной Розничной продажи |  [optional] |
|**description** | **String** | Комментарий Розничного возврата |  [optional] |
|**externalCode** | **String** | Внешний код Розничного возврата |  [optional] |
|**group** | [**Group**](Group.md) |  |  [optional] |
|**moment** | **String** | Дата документа |  [optional] |
|**name** | **String** | Наименование Розничного возврата |  [optional] |
|**noCashSum** | **Double** | Оплачено картой |  [optional] |
|**organization** | [**Organization**](Organization.md) |  |  [optional] |
|**organizationAccount** | [**Account**](Account.md) | Метаданные счета юрлица |  [optional] |
|**owner** | [**Employee**](Employee.md) | Владелец (Сотрудник) |  [optional] |
|**positions** | [**RetailSalesReturnPositionList**](RetailSalesReturnPositionList.md) |  |  [optional] |
|**printed** | **Boolean** | Напечатан ли документ |  [optional] [readonly] |
|**published** | **Boolean** | Опубликован ли документ |  [optional] [readonly] |
|**qrSum** | **Double** | Оплачено по QR-коду |  [optional] |
|**rate** | **CurrencyRate** |  |  [optional] |
|**retailShift** | [**RetailShift**](RetailShift.md) |  |  [optional] |
|**retailStore** | [**RetailStore**](RetailStore.md) |  |  [optional] |
|**shared** | **Boolean** | Общий доступ |  [optional] |
|**state** | [**State**](State.md) | Метаданные статуса Розничного возврата |  [optional] |
|**store** | [**Store**](Store.md) |  |  [optional] |
|**sum** | **Double** | Сумма Розничного возврата в копейках |  [optional] [readonly] |
|**syncId** | **UUID** | ID синхронизации |  [optional] |
|**taxSystem** | **String** | Код системы налогообложения. Известные значения описаны в TaxSystem |  [optional] |
|**updated** | **String** | Момент последнего обновления Розничного возврата |  [optional] [readonly] |
|**vatEnabled** | **Boolean** | Учитывается ли НДС |  [optional] |
|**vatIncluded** | **Boolean** | Включен ли НДС в цену |  [optional] |
|**vatSum** | **Double** | Сумма НДС |  [optional] [readonly] |



