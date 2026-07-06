

# FinanceInOperationRetailShift

Смена + linkedSum

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**id** | **UUID** | ID Розничной смены |  [optional] [readonly] |
|**accountId** | **UUID** | ID учетной записи |  [optional] [readonly] |
|**name** | **String** | Наименование смены |  [optional] |
|**moment** | **String** | Дата смены |  [optional] |
|**retailStore** | [**RetailStore**](RetailStore.md) | Метаданные точки продаж |  [optional] |
|**payments** | [**List&lt;RetailShiftPaymentsInner&gt;**](RetailShiftPaymentsInner.md) | Связанные платежи |  [optional] |
|**acquire** | [**Agent**](Agent.md) | Метаданные Банка-эквайера по операциям по карте |  [optional] |
|**agentAccount** | [**Account**](Account.md) | Метаданные счета контрагента |  [optional] [readonly] |
|**attributes** | [**List&lt;AttributeAbstract&gt;**](AttributeAbstract.md) | Коллекция метаданных доп. полей |  [optional] |
|**bankComission** | **Double** | Сумма комиссии эквайера за проведение безналичных платежей по банковской карте |  [optional] |
|**bankPercent** | **Double** | Комиссия банка-эквайера по операциям по карте (в процентах) |  [optional] |
|**cheque** | [**RetailShiftCheque**](RetailShiftCheque.md) | Информация о смене ККТ |  [optional] |
|**closeDate** | **String** | Дата закрытия смены |  [optional] |
|**contract** | [**Contract**](Contract.md) | Метаданные договора |  [optional] [readonly] |
|**created** | **String** | Дата создания |  [optional] [readonly] |
|**deleted** | **String** | Момент последнего удаления Розничной смены |  [optional] [readonly] |
|**description** | **String** | Комментарий Розничной смены |  [optional] |
|**externalCode** | **String** | Внешний код Розничной смены |  [optional] |
|**files** | [**FileList**](FileList.md) | Метаданные массива Файлов |  [optional] |
|**group** | [**Group**](Group.md) | Отдел сотрудника |  [optional] |
|**operations** | [**List&lt;RetailShiftOperation&gt;**](RetailShiftOperation.md) | Связанные операции. Допустимые типы по &#x60;meta.type&#x60;: retaildemand, retailsalesreturn, retaildrawercashin, retaildrawercashout, prepayment, prepaymentreturn.  |  [optional] [readonly] |
|**organization** | [**Organization**](Organization.md) |  |  [optional] |
|**organizationAccount** | [**Account**](Account.md) | Метаданные счета юрлица |  [optional] |
|**owner** | [**Employee**](Employee.md) | Владелец (Сотрудник) |  [optional] |
|**paymentOperations** | [**List&lt;RetailShiftPaymentOperation&gt;**](RetailShiftPaymentOperation.md) | Коллекция метаданных платежных операций |  [optional] [readonly] |
|**printed** | **Boolean** | Напечатан ли документ |  [optional] [readonly] |
|**proceedsCash** | **Double** | Выручка наличными |  [optional] [readonly] |
|**proceedsNoCash** | **Double** | Выручка безнал |  [optional] [readonly] |
|**published** | **Boolean** | Опубликован ли документ |  [optional] [readonly] |
|**qrAcquire** | [**Agent**](Agent.md) | Метаданные Банка-эквайера по операциям по QR-коду |  [optional] |
|**qrBankComission** | **Double** | Сумма комиссии эквайера за проведение безналичных платежей по QR-коду |  [optional] |
|**qrBankPercent** | **Double** | Комиссия банка-эквайера по операция по QR-коду (в процентах) |  [optional] |
|**receivedCash** | **Double** | Получено наличными |  [optional] [readonly] |
|**receivedNoCash** | **Double** | Получено безнал |  [optional] [readonly] |
|**shared** | **Boolean** | Общий доступ |  [optional] |
|**store** | [**Store**](Store.md) |  |  [optional] |
|**syncId** | **UUID** | ID синхронизации |  [optional] |
|**updated** | **String** | Момент последнего обновления Розничной смены |  [optional] [readonly] |
|**vatEnabled** | **Boolean** | Учитывается ли НДС |  [optional] [readonly] |
|**vatIncluded** | **Boolean** | Включен ли НДС в цену |  [optional] |



