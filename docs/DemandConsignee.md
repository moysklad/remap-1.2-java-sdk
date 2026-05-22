

# DemandConsignee

Грузополучатель (контрагент или юрлицо)

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**id** | **UUID** | ID юрлица |  [optional] [readonly] |
|**syncId** | **UUID** | ID синхронизации |  [optional] |
|**accountId** | **UUID** | ID учетной записи |  [optional] [readonly] |
|**name** | **String** | Наименование юрлица |  [optional] |
|**code** | **String** | Код юрлица |  [optional] |
|**externalCode** | **String** | Внешний код юрлица |  [optional] |
|**archived** | **Boolean** | Добавлено ли юрлицо в архив |  [optional] |
|**created** | **String** | Дата создания |  [optional] [readonly] |
|**updated** | **String** | Момент последнего обновления юрлица |  [optional] [readonly] |
|**description** | **String** | Комментарий к юрлицу |  [optional] |
|**companyType** | **String** | Тип юрлица. Известные значения описаны в CompanyType |  [optional] |
|**email** | **String** | Адрес электронной почты |  [optional] |
|**phone** | **String** | Номер городского телефона |  [optional] |
|**fax** | **String** | Номер факса |  [optional] |
|**actualAddress** | **String** | Фактический адрес юрлица |  [optional] |
|**actualAddressFull** | [**Address**](Address.md) | Фактический адрес юрлица с детализацией по отдельным полям |  [optional] |
|**legalAddress** | **String** | Юридический адрес юрлица |  [optional] |
|**legalAddressFull** | [**Address**](Address.md) | Юридический адрес юрлица с детализацией по отдельным полям |  [optional] |
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
|**bonusProgram** | [**BonusProgram**](BonusProgram.md) | Метаданные активной бонусной программы |  [optional] |
|**priceType** | [**PriceType**](PriceType.md) |  |  [optional] |
|**state** | [**State**](State.md) |  |  [optional] |
|**accounts** | [**OrganizationAccounts**](OrganizationAccounts.md) |  |  [optional] |
|**contactpersons** | [**CounterpartyContactpersons**](CounterpartyContactpersons.md) |  |  [optional] |
|**notes** | [**CounterpartyNotes**](CounterpartyNotes.md) |  |  [optional] |
|**files** | [**FileList**](FileList.md) |  |  [optional] |
|**tags** | **List&lt;String&gt;** | Группы контрагента |  [optional] |
|**attributes** | [**List&lt;AttributeAbstract&gt;**](AttributeAbstract.md) | Дополнительные поля |  [optional] |
|**trackingContractNumber** | **String** | Номер договора с ЦРПТ |  [optional] |
|**trackingContractDate** | **String** | Дата договора с ЦРПТ |  [optional] |
|**advancePaymentVat** | **Double** | Налоговая ставка для авансов для плательщиков НДС |  [optional] |
|**payerVat** | **Boolean** | Является ли данное юрлицо плательщиком НДС |  [optional] |
|**director** | **String** | Руководитель |  [optional] |
|**directorPosition** | **String** | Должность руководителя |  [optional] |
|**chiefAccountant** | **String** | Главный бухгалтер |  [optional] |
|**directorSign** | [**Image**](Image.md) | Подпись руководителя |  [optional] |
|**chiefAccountSign** | [**Image**](Image.md) | Подпись главного бухгалтера |  [optional] |
|**stamp** | [**Image**](Image.md) | Печать |  [optional] |



