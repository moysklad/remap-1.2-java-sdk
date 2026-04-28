

# Contract

Договор

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**id** | **UUID** | ID Договора |  [optional] [readonly] |
|**accountId** | **UUID** | ID учетной записи |  [optional] [readonly] |
|**name** | **String** | Номер договора |  [optional] |
|**description** | **String** | Описание Договора |  [optional] |
|**code** | **String** | Код Договора |  [optional] |
|**externalCode** | **String** | Внешний код Договора |  [optional] |
|**archived** | **Boolean** | Добавлен ли Договор в архив |  [optional] |
|**moment** | **String** | Дата Договора |  [optional] |
|**sum** | **Integer** | Сумма Договора |  [optional] |
|**contractType** | [**ContractTypeEnum**](#ContractTypeEnum) | Тип Договора |  [optional] |
|**rewardType** | [**RewardTypeEnum**](#RewardTypeEnum) | Тип Вознаграждения |  [optional] |
|**rewardPercent** | **Integer** | Вознаграждение в процентах (от 0 до 100) |  [optional] |
|**shared** | **Boolean** | Общий доступ |  [optional] |
|**printed** | **Boolean** | Напечатан ли документ |  [optional] [readonly] |
|**published** | **Boolean** | Опубликован ли документ |  [optional] [readonly] |
|**updated** | **String** | Момент последнего обновления сущности |  [optional] [readonly] |
|**owner** | [**Employee**](Employee.md) | Метаданные владельца (Сотрудника) |  [optional] |
|**group** | [**Group**](Group.md) |  |  [optional] |
|**ownAgent** | [**Organization**](Organization.md) |  |  [optional] |
|**agent** | [**Counterparty**](Counterparty.md) |  |  [optional] |
|**state** | [**State**](State.md) | Метаданные статуса договора |  [optional] |
|**organizationAccount** | [**Account**](Account.md) | Метаданные счета вашего юрлица |  [optional] |
|**agentAccount** | [**Account**](Account.md) | Метаданные счета контрагента |  [optional] |
|**rate** | [**CurrencyRate**](CurrencyRate.md) |  |  [optional] |
|**attributes** | [**List&lt;AttributeAbstract&gt;**](AttributeAbstract.md) | Коллекция доп. полей |  [optional] |



## Enum: ContractTypeEnum

| Name | Value |
|---- | -----|
| COMMISSION | &quot;Commission&quot; |
| SALES | &quot;Sales&quot; |



## Enum: RewardTypeEnum

| Name | Value |
|---- | -----|
| PERCENT_OF_SALES | &quot;PercentOfSales&quot; |
| NONE | &quot;None&quot; |



