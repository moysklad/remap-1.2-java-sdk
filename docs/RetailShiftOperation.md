

# RetailShiftOperation

Элемент массива `operations` розничной смены. Допустимые `meta.type`: retaildemand, retailsalesreturn, retaildrawercashin, retaildrawercashout, prepayment, prepaymentreturn. 

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
|**payedSum** | **Double** | Сумма входящих платежей по Розничной продаже |  [optional] [readonly] |
|**cashSum** | **Double** | Оплачено наличными |  [optional] |
|**noCashSum** | **Double** | Оплачено картой |  [optional] |
|**qrSum** | **Double** | Оплачено по QR-коду |  [optional] |
|**prepaymentCashSum** | **Double** | Предоплата наличными |  [optional] |
|**prepaymentNoCashSum** | **Double** | Предоплата картой |  [optional] |
|**prepaymentQrSum** | **Double** | Предоплата по QR-коду |  [optional] |
|**advancePaymentSum** | **Double** | Оплачено из аванса |  [optional] |
|**checkNumber** | **Integer** | Номер чека |  [optional] |
|**checkSum** | **Double** | Сумма чека |  [optional] |
|**documentNumber** | **Integer** | Номер документа |  [optional] |
|**sessionNumber** | **Integer** | Номер сессии |  [optional] |
|**taxSystem** | **String** | Код системы налогообложения. Известные значения описаны в TaxSystem |  [optional] |
|**state** | [**State**](State.md) | Метаданные статуса Возврата предоплаты |  [optional] |
|**organization** | [**Organization**](Organization.md) |  |  [optional] |
|**organizationAccount** | [**Account**](Account.md) | Метаданные счета юрлица |  [optional] |
|**agent** | [**Agent**](Agent.md) | Метаданные Контрагента или юрлица |  [optional] |
|**agentAccount** | [**Account**](Account.md) | Метаданные счета контрагента |  [optional] |
|**store** | [**Store**](Store.md) |  |  [optional] |
|**retailStore** | [**RetailStore**](RetailStore.md) |  |  [optional] |
|**retailShift** | [**RetailShift**](RetailShift.md) |  |  [optional] |
|**customerOrder** | [**CustomerOrder**](CustomerOrder.md) | Метаданные заказа покупателя |  [optional] |
|**owner** | [**Employee**](Employee.md) | Владелец (Сотрудник) |  [optional] |
|**group** | [**Group**](Group.md) |  |  [optional] |
|**attributes** | [**List&lt;AttributeAbstract&gt;**](AttributeAbstract.md) | Коллекция метаданных доп. полей |  [optional] |
|**files** | [**FileList**](FileList.md) | Метаданные массива Файлов |  [optional] |
|**rate** | **CurrencyRate** |  |  [optional] |
|**positions** | [**PrepaymentReturnPositionList**](PrepaymentReturnPositionList.md) |  |  [optional] |
|**giftCards** | [**List&lt;RetailDemandGiftCard&gt;**](RetailDemandGiftCard.md) | Коллекция подарочных сертификатов, используемых при оплате продажи |  [optional] |
|**cheque** | [**RetailDemandCheque**](RetailDemandCheque.md) | Фискальные данные продажи |  [optional] [readonly] |
|**contract** | [**Contract**](Contract.md) | Метаданные договора |  [optional] |
|**demand** | [**RetailDemand**](RetailDemand.md) | Метаданные связанной Розничной продажи |  [optional] |
|**prepayment** | [**Prepayment**](Prepayment.md) |  |  [optional] |



