

# EmployeeSecurity

Права сотрудника

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**isActive** | **Boolean** | Доступ к сервису МойСклад |  [optional] |
|**login** | **String** | Логин сотрудника для входа в МойСклад |  [optional] |
|**email** | **String** | Почта сотрудника |  [optional] |
|**group** | [**EmployeeSecurityGroup**](EmployeeSecurityGroup.md) |  |  [optional] |
|**authorizedHosts** | **List&lt;String&gt;** | Список ipv4 адресов, с которых разрешен доступ на аккаунт |  [optional] |
|**authorizedIpNetwork** | **String** | Ipv4 адрес, идентифицирующий соответствующую подсеть, с правом доступа на аккаунт |  [optional] |
|**authorizedIpNetmask** | **String** | Маска подсети с правом доступа на аккаунт |  [optional] |
|**role** | [**EmployeeRole**](EmployeeRole.md) |  |  [optional] |



