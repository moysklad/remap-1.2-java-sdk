

# Payroll

Начисление зарплаты

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**id** | **UUID** | ID Начисления зарплаты |  [optional] [readonly] |
|**accountId** | **UUID** | ID учетной записи |  [optional] [readonly] |
|**applicable** | **Boolean** | Отметка о проведении |  [optional] |
|**attributes** | [**List&lt;AttributeAbstract&gt;**](AttributeAbstract.md) | Коллекция метаданных доп. полей |  [optional] |
|**created** | **String** | Дата создания |  [optional] [readonly] |
|**description** | **String** | Описание Начисления зарплаты |  [optional] |
|**endPayrollPeriod** | **String** | Окончание расчётного периода, за который начисляется зарплата. Разница начала и окончания расчётного периода должна быть кратна 24 часам; секунды игнорируются.  |  [optional] |
|**externalCode** | **String** | Внешний код Начисления зарплаты |  [optional] |
|**files** | [**FileList**](FileList.md) | Метаданные массива Файлов (максимальное количество файлов — 100) |  [optional] |
|**group** | [**Group**](Group.md) |  |  [optional] |
|**moment** | **String** | Дата документа |  [optional] |
|**name** | **String** | Наименование Начисления зарплаты |  [optional] |
|**organization** | [**Organization**](Organization.md) |  |  [optional] |
|**owner** | [**Employee**](Employee.md) | Владелец (Сотрудник) |  [optional] |
|**positions** | [**PayrollPositionList**](PayrollPositionList.md) |  |  [optional] |
|**printed** | **Boolean** | Напечатан ли документ |  [optional] [readonly] |
|**published** | **Boolean** | Опубликован ли документ |  [optional] [readonly] |
|**shared** | **Boolean** | Общий доступ |  [optional] |
|**startPayrollPeriod** | **String** | Начало расчётного периода, за который начисляется зарплата. Разница начала и окончания расчётного периода должна быть кратна 24 часам; секунды игнорируются.  |  [optional] |
|**state** | [**State**](State.md) | Метаданные статуса Начисления зарплаты |  [optional] |
|**sum** | **Double** | Сумма Начисления зарплаты в копейках |  [optional] [readonly] |
|**syncId** | **UUID** | ID синхронизации. После заполнения недоступен для изменения |  [optional] |
|**updated** | **String** | Момент последнего обновления Начисления зарплаты |  [optional] [readonly] |



