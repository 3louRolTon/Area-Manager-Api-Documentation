# [Site](#info_site)
## [All users](#info_all_users)
+ [Login](#info_login)
+ [Logout](#info_logout)
## [Admin](#info_admin)
+ [Index](#info_admin_index)
+ [Register](#info_admin_register)
+ Update(В разработке)
+ Logs(В разработке)
## [User](#info_user)
+ [Bind house](#info_user_bind_house)
+ [Unbind house](#info_user_unbind_house)
+ [Bind spot](#info_user_bind_spot)
+ [Unbind spot](#info_user_unbind_spot)
+ [Create](#info_user_create)
    + [Area](#info_user_create_area)
    + [District](#info_user_create_district)
    + [City](#info_user_create_city)
    + [Street](#info_user_create_street)
    + [House](#info_user_create_house)
    + [Spot](#info_user_create_spot)
    + [Deputat](#info_user_create_deputat)
+ Update(В разработке)
    + Area
    + District
    + City
    + Street
    + House
    + Spot
    + Deputat
+ Logs(В разработке)
## Validate
+ В разработке
# [API](#info_api)
## [Area](#info_api_area)
+ [Get All](#info_api_area_get_all)
+ [Get One](#info_api_area_get_one)
+ [Create](#info_api_area_create)
+ [Update](#info_api_area_update)
+ [Delete](#info_api_area_delete)
## [District](#info_api_district)
+ [Get All](#info_api_district_get_all)
+ [Get One](#info_api_district_get_one)
+ [Get By field](#info_api_district_get_by_field)
+ [Create](#info_api_district_create)
+ [Update]
+ [Delete](#info_api_district_delete)
## [City](#info_api_city)
+ [Get All](#info_api_city_get_all)
+ [Get One](#info_api_city_get_one)
+ [Get By field](#info_api_city_get_by_field)
+ [Create](#info_api_city_create)
+ [Update]
+ [Delete](#info_api_city_delete)
+ [Bind](#info_api_city_bind)
+ [Unbind](#info_api_city_unbind)
## [Street]
+ [Get All]
+ [Get One]
+ [Get By field]
+ [Create]
+ [Update]
+ [Delete]
## [House]
+ [Get All]
+ [Get One]
+ [Get By field]
+ [Create]
+ [Update]
+ [Delete]
+ [Bind]
+ [Unbind]
## [Spot]
+ [Get All]
+ [Get One]
+ [Get By field]
+ [Create]
+ [Update]
+ [Delete]
+ [Bind]
+ [Unbind]
## [Deputat]
+ [Get All]
+ [Get One]
+ [Get By field]
+ [Create]
+ [Update]
+ [Delete]

# <a name="info_site"></a> Site
{site} - адрес сайта
## <a name="info_all_users"></a> All Users

### <a name="info_login"></a> Login
Страница для входа в систему.

Имеет поля:
+ login - Имя пользователя
+ password - Пароль пользователя
Ссылка:
{site}/auth/login

### <a name="info_logout"></a> Logout
Страница для выхода из системы.

Ссылка:
{site}/auth/login

## <a name="info_admin"></a> Admin

### <a name="info_admin_index"></a> Index
Страница для ???

Ссылка:
{site}/admin

### <a name="info_admin_register"></a> Register
Страница для создания пользователей.

Имеет поля:
+ Роль (обязательно для заполения)
+ Область (обязательно для заполения Admin/User/Validate)
+ Район (обязательно для заполения User/Validate)
+ Логин (обязательно для заполения)
+ Пароль (обязательно для заполения)

Admin имеет право создавать пользователей с ролями User/Validate

SuperAdmin имеет право создавать пользователей с ролями Admin/User/Validate

Ссылка:
{site}/admin/register

### Update

В разработке

### Logs 

В разработке

## <a name="info_user"></a> User

### <a name="info_user_bind_house"></a> Bind house

Страница для привязки домов/городов к участкам

Имеет поля:
+ Область
+ Район
+ Участок (обязательно для заполения)
+ Город
+ Улица
+ Дома (обязательно для заполения)

Ссылка:
{site}/user

### <a name="info_user_unbind_house"></a> Unbind house

Страница для отвязки домов/городов от участков

Имеет поля:
+ Область
+ Район
+ Участок
+ Город (обязательно для заполения)
+ Дома (обязательно для заполения)

Ссылка:
{site}/user/unbind

### <a name="info_user_bind_spot"></a> Bind spot

Страница для привязки участков к депутатам

Имеет поля:
+ Область
+ Район
+ Депутаты (обязательно для заполения)
+ Участки (обязательно для заполения)

Ссылка:
{site}/user/bindSpot

### <a name="info_user_unbind_spot"></a> Unbind spot

Страница для отвязки участков от депутатов

Имеет поля:
+ Область
+ Район
+ Депутаты
+ Участки (обязательно для заполения)

Ссылка:
{site}/user/unbindSpot

### <a name="info_user_create"></a> Create

### <a name="info_user_create_area"></a> Area (SuperAdmin only)

Страница для создания области

Имеет поля: 
+ Название области (обязательно для заполения)

Ссылка:
{site}/user/create/area

### <a name="info_user_create_district"></a> District (SuperAdmin/Admin only)

Страница для создания района

Имеет поля: 
+ Область (обязательно для заполения)
+ Название района (обязательно для заполения)

Ссылка:
{site}/user/create/district

### <a name="info_user_create_city"></a> City

Страница для создания города

Имеет поля: 
+ Область 
+ Район (обязательно для заполения)
+ Название города (обязательно для заполения)
+ Тип города
+ Сельсовет

Ссылка:
{site}/user/create/city

### <a name="info_user_create_street"></a> Street

Страница для создания улицы

Имеет поля: 
+ Область 
+ Район 
+ Город (обязательно для заполения)
+ Название улицы (обязательно для заполения)
+ Тип улицы (обязательно для заполения)

Ссылка:
{site}/user/create/street

### <a name="info_user_create_house"></a> House

Страница для создания дома

Имеет поля: 
+ Область 
+ Район 
+ Город 
+ Улица (обязательно для заполения)
+ Номер дома (обязательно для заполения)
+ Информация

Ссылка:
{site}/user/create/house

### <a name="info_user_create_spot"></a> Spot

Страница для создания участка

Имеет поля: 
+ Область 
+ Район (обязательно для заполения)
+ Город 
+ Улица 
+ Дом (обязательно для заполения)
+ Название участка (обязательно для заполения)
+ Информация (обязательно для заполения)
+ Номер телефона
+ Координата X
+ Координата Y

Ссылка:
{site}/user/create/spot

### <a name="info_user_create_deputat"></a> Deputat

Страница для создания улицы

Имеет поля: 
+ Область 
+ Район (обязательно для заполения)
+ Фамилия (обязательно для заполения)
+ Имя (обязательно для заполения)
+ Отчество (обязательно для заполения)
+ Название района (обязательно для заполения)
+ Биография (обязательно для заполения)

Ссылка:
{site}/user/create/deputat

### **Update**

В разработке

### **Logs**

В разработке

## Validate (В разработке)

???

# <a name="info_api"></a> API

Возвращает JSON в формате:

```javascript
{
    "success": ,
    "message": ,
    "data": 
}
```

## <a name="info_api_area"></a> Area

### <a name="info_api_area_get_all"></a> Get All

Возвращает весь список областей

Пример {site}/api/areas:

```javascript
{
    "success": true,
    "message": "Areas retrieved successfully.",
    "data": [
        {
            "id": 1,
            "name": "Test_Area_Name_1"
        },
        {
            "id": 2,
            "name": "Test_Area_Name_2"
        },
        {
            "id": 3,
            "name": "Test_Area_Name_3"
        }
    ]
}
```
Метод запроса GET {site}/api/areas

### <a name="info_api_area_get_one"></a> Get One

Возвращает область по {id}

Пример {site}/api/areas/1:

```javascript
{
    "success": true,
    "message": "Area retrieved successfully.",
    "data": {
        "id": 1,
        "name": "Test_Area_Name_1"
    }
}
```
{id} - id области которое нужно вернуть

Метод запроса GET {site}/api/areas/{id}

### <a name="info_api_area_create"></a> Create

Возвращает созданную область

Пример {site}/api/areas?area_name=Test_Area_Name_3:

```javascript
{
    "success": true,
    "message": "Area created successfully.",
    "data": {
        "id": 3,
        "name": "Test_Area_Name_3"
    }
}
```
Параметры запроса:
+ area_name (обязательный параметр)

Метод запроса POST {site}/api/areas

### <a name="info_api_area_update"></a> Update

Возвращает измененную область

Пример {site}/api/areas/1?area_name=Update_Area_Name_3:

```javascript
{
    "success": true,
    "message": "Area updated successfully.",
    "data": {
        "id": 1,
        "name": "Update_Area_Name_3"
    }
}
```
Параметры запроса:
+ area_name (обязательный параметр)

Метод запроса PUT {site}/api/areas/{id}

### <a name="info_api_area_delete"></a> Delete

Возвращает сообщение о успешности действия

Пример {site}/api/areas/1:

```javascript
{
    "success": true,
    "message": "Area deleted successfully.",
    "data": []
}
```
{id} - id области которую нужно удалить

Метод запроса DELETE {site}/api/areas/{id}

## <a name="info_api_district"></a> District

### <a name="info_api_district_get_all"></a> Get All

Возвращает весь список районов

Пример {site}/api/districts:

```javascript
{
    "success": true,
    "message": "Districts retrieved successfully.",
    "data": [
        {
            "id": 1,
            "name": "District_Name_Test_1",
            "area_id": 1
        },
        {
            "id": 2,
            "name": "District_Name_Test_2",
            "area_id": 1
        },
        {
            "id": 3,
            "name": "District_Name_Test_3",
            "area_id": 2
        }
    ]
}
```
Метод запроса GET {site}/api/districts

### <a name="info_api_district_get_one"></a> Get One

Возвращает район по {id}

Пример {site}/api/districts/1:

```javascript
{
    "success": true,
    "message": "District retrieved successfully.",
    "data": {
        "id": 1,
        "name": "District_Name_Test_1",
        "area_id": 1
    }
}
```
{id} - id района которого нужно вернуть

Метод запроса GET {site}/api/districts/{id}

### <a name="info_api_district_get_by_field"></a> Get By field

Возвращает весь список районов с полем {field} равным {id}

Пример {site}/api/districts/area_id/1:

```javascript
{
    "success": true,
    "message": "Districts retrieved successfully.",
    "data": [
        {
            "id": 1,
            "name": "District_Name_Test_1",
            "area_id": 1
        },
        {
            "id": 2,
            "name": "District_Name_Test_2",
            "area_id": 1
        }
    ]
}
```
{field} - поле таблицы district

{id} - id поля {field} по которому ведется поиск

Доступные поля district:
+ area_id

Метод запроса GET {site}/api/districts/{field}/{id}

### <a name="info_api_district_create"></a> Create

Возвращает созданный район

Пример {site}/api/districts?district_name=Create_District_Name_1&area_id=1:

```javascript
{
    "success": true,
    "message": "District created successfully.",
    "data": {
        "id": 2,
        "name": "Create_District_Name_1",
        "area_id": "1"
    }
}
```
Параметры запроса:
+ district_name (обязательный параметр)
+ area_id (обязательный параметр)

Метод запроса POST {site}/api/districts

### <a name="info_api_district_delete"></a> Delete

Возвращает сообщение о завершении

Пример {site}/api/districts/1:

```javascript
{
    "success": true,
    "message": "District deleted successfully.",
    "data": []
}
```
{id} - id области которую нужно удалить

Метод запроса DELETE {site}/api/districts/{id}

## <a name="info_api_city"></a> City

### <a name="info_api_city_get_all"></a> Get All

Возвращает весь список городов

Пример {site}/api/cities:

```javascript
{
    "success": true,
    "message": "Cities retrieved successfully.",
    "data": [
        {
            "id": 1,
            "name": "City_Name_Test_1",
            "type": "City_Name_Type_1",
            "category": "City_Name_Category_1",
            "district_id": 1,
            "spot_id": null
        },
        {
            "id": 2,
            "name": "City_Name_Test_2",
            "type": "City_Name_Type_2",
            "category": "City_Name_Category_2",
            "district_id": 1,
            "spot_id": 1
        },
                {
            "id": 3,
            "name": "City_Name_Test_3",
            "type": "City_Name_Type_3",
            "category": "City_Name_Category_3",
            "district_id": 2,
            "spot_id": null
        }
    ]
}
```
Метод запроса GET {site}/api/cities

### <a name="info_api_city_get_one"></a> Get One

Возвращает город по {id}

Пример {site}/api/cities/1:

```javascript
{
    "success": true,
    "message": "City retrieved successfully.",
    "data": {
        "id": 1,
        "name": "City_Name_Test_1",
        "type": "City_Name_Type_1",
        "category": "City_Name_Category_1",
        "district_id": 1,
        "spot_id": null
    }
}
```
{id} - id города которого нужно вернуть

Метод запроса GET {site}/api/cities/{id}

### <a name="info_api_city_get_by_field"></a> Get By field

Возвращает весь список городов с полем {field} равным {id}

Пример {site}/api/cities/district_id/1:

```javascript
{
    "success": true,
    "message": "Cities retrieved successfully.",
    "data": [
        {
            "id": 1,
            "name": "City_Name_Test_1",
            "type": "City_Name_Type_1",
            "category": "City_Name_Category_1",
            "district_id": 1,
            "spot_id": null
        },
        {
            "id": 2,
            "name": "City_Name_Test_2",
            "type": "City_Name_Type_2",
            "category": "City_Name_Category_2",
            "district_id": 1,
            "spot_id": 1
        }
    ]
}
```
{field} - поле таблицы district

{id} - id поля {field} по которому ведется поиск

Доступные поля city:
+ district_id
+ spot_id

Метод запроса GET {site}/api/cities/{field}/{id}

### <a name="info_api_city_create"></a> Create

Возвращает созданный город

Пример {site}/api/cities?city_name=Name&city_type=Type&city_category=Category&district_id=1:

```javascript
{
    "success": true,
    "message": "City created successfully.",
    "data": {
        "id": 1,
        "name": "Name",
        "type": "Type",
        "category": "Category",
        "district_id": "1",
        "spot_id": null
    }
}
```
Параметры запроса:
+ city_name (обязательный параметр)
+ city_type
+ city_category
+ district_id (обязательный параметр)

Метод запроса POST {site}/api/cities

### <a name="info_api_city_delete"></a> Delete

Возвращает сообщение о завершении

Пример {site}/api/cities/1:

```javascript
{
    "success": true,
    "message": "City deleted successfully.",
    "data": []
}
```
{id} - id города который нужно удалить

Метод запроса DELETE {site}/api/cities/{id}

### <a name="info_api_city_bind"></a> Bind

Привязывает города к участку

Пример {site}/api/cities/bind?spot_id=1&cities_id[]=1&cities_id[]=2:

```javascript
{
    "success": true,
    "message": "City bind successfully.",
    "data": []
}
```
Параметры запроса:
+ cities_id[] (обязательный параметр)
+ spot_id (обязательный параметр)

Метод запроса POST {site}/api/cities/bind

### <a name="info_api_city_unbind"></a> Unbind

Отвязывает города от участка

Пример {site}/api/cities/bind?cities_id[]=1&cities_id[]=2:

```javascript
{
    "success": true,
    "message": "City unbind successfully.",
    "data": []
}
```
Параметры запроса:
+ cities_id[] (обязательный параметр)

Метод запроса POST {site}/api/cities/unbind
