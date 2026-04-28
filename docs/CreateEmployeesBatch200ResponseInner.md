

# CreateEmployeesBatch200ResponseInner


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**id** | **UUID** | ID сотрудника |  [optional] [readonly] |
|**accountId** | **UUID** | ID учетной записи |  [optional] [readonly] |
|**name** | **String** | Наименование сотрудника |  [optional] [readonly] |
|**externalCode** | **String** | Внешний код сотрудника |  [optional] |
|**archived** | **Boolean** | Добавлен ли сотрудник в архив |  [optional] |
|**created** | **String** | Момент создания |  [optional] [readonly] |
|**updated** | **String** | Момент последнего обновления |  [optional] [readonly] |
|**description** | **String** | Комментарий к сотруднику |  [optional] |
|**email** | **String** | Адрес электронной почты |  [optional] |
|**phone** | **String** | Номер телефона |  [optional] |
|**firstName** | **String** | Имя |  [optional] |
|**middleName** | **String** | Отчество |  [optional] |
|**lastName** | **String** | Фамилия |  [optional] |
|**fullName** | **String** | Полное имя сотрудника |  [optional] [readonly] |
|**shortFio** | **String** | Краткое ФИО сотрудника |  [optional] [readonly] |
|**shared** | **Boolean** | Общий доступ |  [optional] |
|**group** | [**Group**](Group.md) |  |  [optional] |
|**owner** | [**Employee**](Employee.md) | Метаданные владельца (Сотрудника) |  [optional] |
|**inn** | **String** | ИНН сотрудника (в формате ИНН физического лица) |  [optional] |
|**position** | **String** | Должность сотрудника |  [optional] |
|**uid** | **String** | Логин сотрудника |  [optional] [readonly] |
|**salary** | [**EmployeeSalary**](EmployeeSalary.md) |  |  [optional] |
|**cashiers** | [**List&lt;Cashier&gt;**](Cashier.md) | Массив кассиров |  [optional] [readonly] |
|**image** | [**Image**](Image.md) | Фотография сотрудника |  [optional] |
|**attributes** | [**List&lt;AttributeAbstract&gt;**](AttributeAbstract.md) | Дополнительные поля |  [optional] |
|**errors** | [**List&lt;ErrorErrorsInner&gt;**](ErrorErrorsInner.md) |  |  |



