

# RetailStore

Точка продаж

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**id** | **UUID** | ID Точки продаж |  [optional] [readonly] |
|**accountId** | **UUID** | ID учетной записи владельца Точки продаж |  [optional] [readonly] |
|**name** | **String** | Наименование Точки продаж |  [optional] |
|**description** | **String** | Комментарий к Точке продаж |  [optional] |
|**active** | **Boolean** | Признак активности Точки продаж |  [optional] |
|**archived** | **Boolean** | Признак архивности Точки продаж |  [optional] |
|**shared** | **Boolean** | Общий доступ к Точке продаж |  [optional] |
|**address** | **String** | Адрес Точки продаж одной строкой |  [optional] |
|**addressFull** | [**Address**](Address.md) |  |  [optional] |
|**externalCode** | **String** | Внешний код Точки продаж |  [optional] [readonly] |
|**updated** | **String** | Момент последнего обновления Точки продаж |  [optional] [readonly] |
|**meta** | [**Meta**](Meta.md) |  |  [optional] |
|**organization** | **Organization** | Метаданные юрлица-владельца Точки продаж |  [optional] |
|**store** | [**Store**](Store.md) |  |  [optional] |
|**group** | [**Group**](Group.md) |  |  [optional] |
|**owner** | [**Employee**](Employee.md) | Метаданные владельца (сотрудника) |  [optional] |
|**priceType** | [**PriceType**](PriceType.md) |  |  [optional] |
|**environment** | [**RetailStoreEnvironment**](RetailStoreEnvironment.md) |  |  [optional] |
|**state** | [**RetailStoreState**](RetailStoreState.md) |  |  [optional] |
|**fiscalType** | [**FiscalTypeEnum**](#FiscalTypeEnum) | Фискальный режим работы Точки продаж |  [optional] |
|**defaultTaxSystem** | [**DefaultTaxSystemEnum**](#DefaultTaxSystemEnum) | Система налогообложения по умолчанию |  [optional] |
|**orderTaxSystem** | [**OrderTaxSystemEnum**](#OrderTaxSystemEnum) | Система налогообложения заказов |  [optional] |
|**minionToMasterType** | [**MinionToMasterTypeEnum**](#MinionToMasterTypeEnum) | Ограничение связи касс-слуг с кассами-мастерами |  [optional] |
|**tobaccoMrcControlType** | [**TobaccoMrcControlTypeEnum**](#TobaccoMrcControlTypeEnum) | Режим контроля минимальных розничных цен на табак |  [optional] |
|**markingSellingMode** | [**MarkingSellingModeEnum**](#MarkingSellingModeEnum) | Режим продажи маркированных товаров |  [optional] |
|**marksCheckMode** | [**MarksCheckModeEnum**](#MarksCheckModeEnum) | Режим проверки кодов маркировки |  [optional] |
|**priorityOfdSend** | [**PriorityOfdSendEnum**](#PriorityOfdSendEnum) | Приоритетный способ отправки чека покупателю |  [optional] |
|**allowCreateProducts** | **Boolean** | Признак разрешения создания новых товаров при продаже |  [optional] |
|**allowCustomPrice** | **Boolean** | Признак разрешения устанавливать произвольные цены |  [optional] [readonly] |
|**allowDeleteReceiptPositions** | **Boolean** | Признак разрешения удалять позиции из чека |  [optional] |
|**allowSellTobaccoWithoutMRC** | **Boolean** | Признак разрешения продажи табачной продукции без проверки МРЦ |  [optional] |
|**authTokenAttached** | **Boolean** | Признак подключения авторизационного токена |  [optional] [readonly] |
|**controlCashierChoice** | **Boolean** | Признак контроля выбора кассира |  [optional] |
|**controlShippingStock** | **Boolean** | Признак контроля отгрузки только из наличия |  [optional] |
|**createCashInOnRetailShiftClosing** | **Boolean** | Признак создания операции внесения при закрытии смены |  [optional] |
|**createPaymentInOnRetailShiftClosing** | **Boolean** | Признак создания операции прихода денег при закрытии смены |  [optional] |
|**createAgentsTags** | **List&lt;String&gt;** | Теги, создаваемые у агентов |  [optional] |
|**filterAgentsTags** | **List&lt;String&gt;** | Группы, по которым фильтруются агенты |  [optional] |
|**createOrderWithState** | [**State**](State.md) | Статус, в котором создаются заказы покупателей |  [optional] |
|**customerOrderStates** | [**List&lt;State&gt;**](State.md) | Возможные состояния заказов покупателей |  [optional] |
|**discountEnable** | **Boolean** | Признак включения скидок |  [optional] |
|**discountMaxPercent** | **Integer** | Максимально допустимый процент скидки |  [optional] |
|**enableReturnsWithNoReason** | **Boolean** | Признак разрешения возвратов без причины |  [optional] |
|**issueOrders** | **Boolean** | Признак оформления заказов покупателей |  [optional] |
|**lastOperationNames** | [**List&lt;RetailStoreLastOperationNamesInner&gt;**](RetailStoreLastOperationNamesInner.md) | Последние операции |  [optional] |
|**masterRetailStores** | [**RetailStoreList**](RetailStoreList.md) | Список касс-мастеров |  [optional] |
|**ofdEnabled** | **Boolean** | Признак использования ОФД |  [optional] [readonly] |
|**onlyInStock** | **Boolean** | Признак продажи только из наличия |  [optional] |
|**orderToState** | [**State**](State.md) | Метаданные статуса заказа покупателя |  [optional] |
|**printAlways** | **Boolean** | Признак обязательной печати чеков |  [optional] |
|**productFolders** | [**ProductFolderList**](ProductFolderList.md) | Список групп товаров |  [optional] |
|**receiptTemplate** | [**RetailStoreReceiptTemplate**](RetailStoreReceiptTemplate.md) |  |  [optional] |
|**requiredFio** | **Boolean** | Признак обязательности ФИО покупателя |  [optional] |
|**requiredPhone** | **Boolean** | Признак обязательности телефона покупателя |  [optional] |
|**requiredEmail** | **Boolean** | Признак обязательности email покупателя |  [optional] |
|**requiredBirthdate** | **Boolean** | Признак обязательности даты рождения покупателя |  [optional] |
|**requiredSex** | **Boolean** | Признак обязательности пола покупателя |  [optional] |
|**requiredDiscountCardNumber** | **Boolean** | Признак обязательности номера дисконтной карты покупателя |  [optional] |
|**reservePrepaidGoods** | **Boolean** | Признак резервирования предоплаченных товаров |  [optional] |
|**returnFromClosedShiftEnabled** | **Boolean** | Признак разрешения возвратов из закрытой смены |  [optional] |
|**sellReserves** | **Boolean** | Признак разрешения продажи резервов |  [optional] |
|**sendMarksForCheck** | **Boolean** | Признак отправки кодов маркировки на проверку |  [optional] |
|**sendMarksToChestnyZnakOnCloud** | **Boolean** | Признак отправки кодов маркировки в Честный ЗНАК в облаке |  [optional] |
|**syncAgents** | **Boolean** | Признак синхронизации агентов |  [optional] |
|**showBeerOnTap** | **Boolean** | Признак отображения разливного пива |  [optional] |
|**qrPayEnabled** | **Boolean** | Признак включения оплаты через QR |  [optional] |
|**bankPercent** | **Double** | Банковский процент |  [optional] |
|**qrBankPercent** | **Double** | Банковский процент при оплате по QR |  [optional] |
|**demandPrefix** | **String** | Префикс номера заказа |  [optional] |
|**qrTerminalId** | **String** | Идентификатор QR-терминала |  [optional] |
|**idQR** | **String** | Идентификатор QR |  [optional] |
|**acquire** | [**Counterparty**](Counterparty.md) |  |  [optional] |
|**cashiers** | [**CashierList**](CashierList.md) | Кассиры, работающие на точке продаж |  [optional] |
|**qrAcquire** | [**Counterparty**](Counterparty.md) | Эквайер для QR-платежей |  [optional] |



## Enum: FiscalTypeEnum

| Name | Value |
|---- | -----|
| STANDARD | &quot;STANDARD&quot; |
| MASTER | &quot;MASTER&quot; |
| CLOUD | &quot;CLOUD&quot; |



## Enum: DefaultTaxSystemEnum

| Name | Value |
|---- | -----|
| GENERAL_TAX_SYSTEM | &quot;GENERAL_TAX_SYSTEM&quot; |
| SIMPLIFIED_TAX_SYSTEM_INCOME | &quot;SIMPLIFIED_TAX_SYSTEM_INCOME&quot; |
| SIMPLIFIED_TAX_SYSTEM_INCOME_OUTCOME | &quot;SIMPLIFIED_TAX_SYSTEM_INCOME_OUTCOME&quot; |
| UNIFIED_AGRICULTURAL_TAX | &quot;UNIFIED_AGRICULTURAL_TAX&quot; |
| PRESUMPTIVE_TAX_SYSTEM | &quot;PRESUMPTIVE_TAX_SYSTEM&quot; |
| PATENT_BASED | &quot;PATENT_BASED&quot; |



## Enum: OrderTaxSystemEnum

| Name | Value |
|---- | -----|
| GENERAL_TAX_SYSTEM | &quot;GENERAL_TAX_SYSTEM&quot; |
| SIMPLIFIED_TAX_SYSTEM_INCOME | &quot;SIMPLIFIED_TAX_SYSTEM_INCOME&quot; |
| SIMPLIFIED_TAX_SYSTEM_INCOME_OUTCOME | &quot;SIMPLIFIED_TAX_SYSTEM_INCOME_OUTCOME&quot; |
| UNIFIED_AGRICULTURAL_TAX | &quot;UNIFIED_AGRICULTURAL_TAX&quot; |
| PRESUMPTIVE_TAX_SYSTEM | &quot;PRESUMPTIVE_TAX_SYSTEM&quot; |
| PATENT_BASED | &quot;PATENT_BASED&quot; |



## Enum: MinionToMasterTypeEnum

| Name | Value |
|---- | -----|
| ANY | &quot;ANY&quot; |
| SAME_GROUP | &quot;SAME_GROUP&quot; |
| CHOSEN | &quot;CHOSEN&quot; |



## Enum: TobaccoMrcControlTypeEnum

| Name | Value |
|---- | -----|
| USER_PRICE | &quot;USER_PRICE&quot; |
| MRC_PRICE | &quot;MRC_PRICE&quot; |
| SAME_PRICE | &quot;SAME_PRICE&quot; |



## Enum: MarkingSellingModeEnum

| Name | Value |
|---- | -----|
| CORRECT_MARKS_ONLY | &quot;CORRECT_MARKS_ONLY&quot; |
| WITHOUT_ERRORS | &quot;WITHOUT_ERRORS&quot; |
| ALL | &quot;ALL&quot; |



## Enum: MarksCheckModeEnum

| Name | Value |
|---- | -----|
| CORRECT_MARKS_ONLY | &quot;CORRECT_MARKS_ONLY&quot; |
| WITHOUT_ERRORS | &quot;WITHOUT_ERRORS&quot; |
| ALL | &quot;ALL&quot; |
| ALL_CHECKED | &quot;ALL_CHECKED&quot; |



## Enum: PriorityOfdSendEnum

| Name | Value |
|---- | -----|
| PHONE | &quot;phone&quot; |
| EMAIL | &quot;email&quot; |
| NONE | &quot;none&quot; |



