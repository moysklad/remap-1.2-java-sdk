

# RetailDemand

Розничная продажа

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**id** | **UUID** | ID Розничной продажи |  [optional] [readonly] |
|**accountId** | **UUID** | ID учетной записи |  [optional] [readonly] |
|**name** | **String** | Наименование Розничной продажи |  [optional] |
|**code** | **String** | Код Розничной продажи |  [optional] |
|**externalCode** | **String** | Внешний код Розничной продажи |  [optional] |
|**syncId** | **UUID** | ID синхронизации |  [optional] |
|**description** | **String** | Комментарий Розничной продажи |  [optional] |
|**created** | **String** | Дата создания |  [optional] [readonly] |
|**deleted** | **String** | Момент последнего удаления Розничной продажи |  [optional] [readonly] |
|**updated** | **String** | Момент последнего обновления Розничной продажи |  [optional] [readonly] |
|**moment** | **String** | Дата документа |  [optional] |
|**applicable** | **Boolean** | Отметка о проведении |  [optional] |
|**printed** | **Boolean** | Напечатан ли документ |  [optional] [readonly] |
|**published** | **Boolean** | Опубликован ли документ |  [optional] [readonly] |
|**shared** | **Boolean** | Общий доступ |  [optional] |
|**vatEnabled** | **Boolean** | Учитывается ли НДС |  [optional] |
|**vatIncluded** | **Boolean** | Включен ли НДС в цену |  [optional] |
|**vatSum** | **Double** | Сумма НДС |  [optional] [readonly] |
|**sum** | **Double** | Сумма Розничной продажи в копейках |  [optional] [readonly] |
|**payedSum** | **Double** | Сумма входящих платежей по Розничной продаже |  [optional] [readonly] |
|**cashSum** | **Double** | Оплачено наличными |  [optional] |
|**noCashSum** | **Double** | Оплачено картой |  [optional] |
|**qrSum** | **Double** | Оплачено по QR-коду |  [optional] |
|**prepaymentCashSum** | **Double** | Предоплата наличными |  [optional] |
|**prepaymentNoCashSum** | **Double** | Предоплата картой |  [optional] |
|**prepaymentQrSum** | **Double** | Предоплата по QR-коду |  [optional] |
|**advancePaymentSum** | **Double** | Оплачено из аванса |  [optional] |
|**checkNumber** | **String** | Номер чека |  [optional] |
|**checkSum** | **Double** | Сумма чека |  [optional] |
|**documentNumber** | **String** | Номер документа |  [optional] |
|**sessionNumber** | **String** | Номер сессии |  [optional] |
|**taxSystem** | **String** | Код системы налогообложения. Известные значения описаны в TaxSystem |  [optional] |
|**state** | [**State**](State.md) | Метаданные статуса Розничной продажи |  [optional] |
|**organization** | [**Organization**](Organization.md) |  |  [optional] |
|**organizationAccount** | [**Account**](Account.md) | Метаданные счета юрлица |  [optional] |
|**agent** | [**Agent**](Agent.md) | Метаданные контрагента или юрлица |  [optional] |
|**agentAccount** | [**Account**](Account.md) | Метаданные счета контрагента |  [optional] |
|**store** | [**Store**](Store.md) |  |  [optional] |
|**retailStore** | [**RetailStore**](RetailStore.md) |  |  [optional] |
|**retailShift** | [**RetailShift**](RetailShift.md) |  |  [optional] |
|**customerOrder** | [**CustomerOrder**](CustomerOrder.md) | Метаданные заказа покупателя |  [optional] |
|**owner** | [**Employee**](Employee.md) | Владелец (Сотрудник) |  [optional] |
|**group** | [**Group**](Group.md) |  |  [optional] |
|**attributes** | [**List&lt;AttributeAbstract&gt;**](AttributeAbstract.md) | Коллекция метаданных доп. полей |  [optional] |
|**files** | [**FileList**](FileList.md) | Метаданные массива файлов |  [optional] |
|**rate** | [**CurrencyRate**](CurrencyRate.md) |  |  [optional] |
|**positions** | [**RetailDemandPositionList**](RetailDemandPositionList.md) |  |  [optional] |
|**giftCards** | [**List&lt;RetailDemandGiftCard&gt;**](RetailDemandGiftCard.md) | Коллекция подарочных сертификатов, используемых при оплате продажи |  [optional] |
|**cheque** | [**RetailDemandCheque**](RetailDemandCheque.md) | Фискальные данные продажи |  [optional] [readonly] |



