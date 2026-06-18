

# FinanceOutOperationCommissionReportOut

Выданный отчет комиссионера + linkedSum

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**id** | **UUID** | ID Выданного отчета комиссионера |  [optional] [readonly] |
|**accountId** | **UUID** | ID учетной записи |  [optional] [readonly] |
|**agent** | [**Agent**](Agent.md) | Метаданные контрагента или юрлица |  [optional] |
|**agentAccount** | [**Account**](Account.md) | Метаданные счета контрагента |  [optional] |
|**applicable** | **Boolean** | Отметка о проведении |  [optional] |
|**attributes** | [**List&lt;AttributeAbstract&gt;**](AttributeAbstract.md) | Коллекция метаданных доп. полей |  [optional] |
|**code** | **String** | Код Выданного отчета комиссионера |  [optional] |
|**commissionPeriodEnd** | **String** | Конец периода |  [optional] |
|**commissionPeriodStart** | **String** | Начало периода |  [optional] |
|**commitentSum** | **Double** | Сумма коммитента в установленной валюте |  [optional] [readonly] |
|**contract** | [**Contract**](Contract.md) | Метаданные договора |  [optional] |
|**created** | **String** | Дата создания |  [optional] [readonly] |
|**deleted** | **String** | Момент последнего удаления Выданного отчета комиссионера |  [optional] [readonly] |
|**description** | **String** | Комментарий Выданного отчета комиссионера |  [optional] |
|**externalCode** | **String** | Внешний код Выданного отчета комиссионера |  [optional] |
|**files** | [**FileList**](FileList.md) | Метаданные массива файлов |  [optional] |
|**group** | [**Group**](Group.md) |  |  [optional] |
|**moment** | **String** | Дата документа |  [optional] |
|**name** | **String** | Наименование Выданного отчета комиссионера |  [optional] |
|**organization** | [**Organization**](Organization.md) |  |  [optional] |
|**organizationAccount** | [**Account**](Account.md) | Метаданные счета юрлица |  [optional] |
|**owner** | [**Employee**](Employee.md) | Владелец (Сотрудник) |  [optional] |
|**payedSum** | **Double** | Оплаченная сумма |  [optional] [readonly] |
|**positions** | **CommissionReportOutPositionList** |  |  [optional] |
|**printed** | **Boolean** | Напечатан ли документ |  [optional] [readonly] |
|**project** | [**Project**](Project.md) | Метаданные проекта |  [optional] |
|**published** | **Boolean** | Опубликован ли документ |  [optional] [readonly] |
|**rate** | [**CurrencyRate**](CurrencyRate.md) |  |  [optional] |
|**rewardPercent** | **Integer** | Процент вознаграждения |  [optional] |
|**rewardType** | **String** | Тип Вознаграждения. Известные значения описаны в RewardType |  [optional] |
|**salesChannel** | [**SalesChannel**](SalesChannel.md) | Метаданные канала продаж |  [optional] |
|**shared** | **Boolean** | Общий доступ |  [optional] |
|**state** | [**State**](State.md) | Метаданные статуса Выданного отчета комиссионера |  [optional] |
|**sum** | **Double** | Сумма Выданного отчета комиссионера в копейках |  [optional] |
|**syncId** | **UUID** | ID синхронизации |  [optional] |
|**updated** | **String** | Момент последнего обновления Выданного отчета комиссионера |  [optional] [readonly] |
|**vatEnabled** | **Boolean** | Учитывается ли НДС |  [optional] |
|**vatIncluded** | **Boolean** | Включен ли НДС в цену |  [optional] |
|**vatSum** | **Double** | Сумма НДС |  [optional] |
|**payments** | [**List&lt;CustomerOrderPaymentsInner&gt;**](CustomerOrderPaymentsInner.md) | Массив ссылок на связанные платежи |  [optional] |



