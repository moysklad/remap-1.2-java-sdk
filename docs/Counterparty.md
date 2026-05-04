

# Counterparty

Контрагент

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**id** | **UUID** | ID контрагента |  [optional] [readonly] |
|**syncId** | **UUID** | ID синхронизации |  [optional] |
|**accountId** | **UUID** | ID учетной записи |  [optional] [readonly] |
|**name** | **String** | Наименование контрагента |  [optional] |
|**code** | **String** | Код контрагента |  [optional] |
|**externalCode** | **String** | Внешний код контрагента |  [optional] |
|**archived** | **Boolean** | Добавлен ли контрагент в архив |  [optional] |
|**created** | **String** | Момент создания |  [optional] [readonly] |
|**updated** | **String** | Момент последнего обновления |  [optional] [readonly] |
|**description** | **String** | Комментарий к контрагенту |  [optional] |
|**companyType** | **String** | Тип контрагента. Известные значения описаны в CompanyType |  [optional] |
|**email** | **String** | Адрес электронной почты |  [optional] |
|**phone** | **String** | Номер телефона |  [optional] |
|**fax** | **String** | Номер факса |  [optional] |
|**actualAddress** | **String** | Фактический адрес контрагента |  [optional] |
|**actualAddressFull** | [**Address**](Address.md) | Полный адрес |  [optional] |
|**legalAddress** | **String** | Юридический адрес контрагента |  [optional] |
|**legalAddressFull** | [**Address**](Address.md) | Полный юридический адрес контрагента |  [optional] |
|**inn** | **String** | ИНН |  [optional] |
|**kpp** | **String** | КПП |  [optional] |
|**ogrn** | **String** | ОГРН |  [optional] |
|**ogrnip** | **String** | ОГРНИП |  [optional] |
|**okpo** | **String** | ОКПО |  [optional] |
|**certificateNumber** | **String** | Номер свидетельства |  [optional] |
|**certificateDate** | **String** | Дата свидетельства |  [optional] |
|**legalTitle** | **String** | Полное наименование |  [optional] |
|**legalFirstName** | **String** | Имя для ИП и физлица |  [optional] |
|**legalLastName** | **String** | Фамилия для ИП и физлица |  [optional] |
|**legalMiddleName** | **String** | Отчество для ИП и физлица |  [optional] |
|**birthDate** | **String** | Дата рождения для физлица |  [optional] |
|**sex** | **String** | Пол контрагента. Известные значения описаны в Sex |  [optional] |
|**discountCardNumber** | **String** | Номер дисконтной карты контрагента |  [optional] |
|**discounts** | [**List&lt;AgentDiscount&gt;**](AgentDiscount.md) | Массив скидок контрагента |  [optional] |
|**shared** | **Boolean** | Общий доступ |  [optional] |
|**group** | [**Group**](Group.md) |  |  [optional] |
|**owner** | [**Employee**](Employee.md) | Метаданные владельца (Сотрудника) |  [optional] |
|**salesAmount** | **Float** | Сумма продаж |  [optional] [readonly] |
|**bonusPoints** | **Integer** | Бонусные баллы по активной бонусной программе |  [optional] [readonly] |
|**bonusProgram** | [**BonusProgram**](BonusProgram.md) |  |  [optional] |
|**priceType** | [**PriceType**](PriceType.md) |  |  [optional] |
|**state** | [**State**](State.md) |  |  [optional] |
|**accounts** | [**CounterpartyAccounts**](CounterpartyAccounts.md) |  |  [optional] |
|**contactpersons** | [**CounterpartyContactpersons**](CounterpartyContactpersons.md) |  |  [optional] |
|**notes** | [**CounterpartyNotes**](CounterpartyNotes.md) |  |  [optional] |
|**files** | [**FileList**](FileList.md) |  |  [optional] |
|**tags** | **List&lt;String&gt;** | Группы контрагента |  [optional] |
|**attributes** | [**List&lt;AttributeAbstract&gt;**](AttributeAbstract.md) | Дополнительные поля |  [optional] |



