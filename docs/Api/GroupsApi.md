# Swagger\Client\GroupsApi

All URIs are relative to *https://wappi.pro*

Method | HTTP request | Description
------------- | ------------- | -------------
[**apiSyncGroupAdminDemotePost**](GroupsApi.md#apisyncgroupadmindemotepost) | **POST** /api/sync/group/admin/demote | Убрать права администратора группы для контакта
[**apiSyncGroupAdminPromovePost**](GroupsApi.md#apisyncgroupadminpromovepost) | **POST** /api/sync/group/admin/promove | Добавить права администратора группы контакту
[**apiSyncGroupAdminsGetGet**](GroupsApi.md#apisyncgroupadminsgetget) | **GET** /api/sync/group/admins/get | Получить список администраторов из группы
[**apiSyncGroupCreatePost**](GroupsApi.md#apisyncgroupcreatepost) | **POST** /api/sync/group/create | Создать новую группу
[**apiSyncGroupLeavePost**](GroupsApi.md#apisyncgroupleavepost) | **POST** /api/sync/group/leave | Покинуть группу
[**apiSyncGroupParticipantAddPost**](GroupsApi.md#apisyncgroupparticipantaddpost) | **POST** /api/sync/group/participant/add | Добавить контакт в группу
[**apiSyncGroupParticipantRemovePost**](GroupsApi.md#apisyncgroupparticipantremovepost) | **POST** /api/sync/group/participant/remove | Удалить контакт из группы
[**apiSyncGroupParticipantsGetGet**](GroupsApi.md#apisyncgroupparticipantsgetget) | **GET** /api/sync/group/participants/get | Получить контакты из группы

# **apiSyncGroupAdminDemotePost**
> \Swagger\Client\Model\InlineResponse2002 apiSyncGroupAdminDemotePost($profile_id, $chat_id, $contact)

Убрать права администратора группы для контакта

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\GroupsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$profile_id = "profile_id_example"; // string | Profile ID
$chat_id = "chat_id_example"; // string | Chat ID - ID чата группы из списка сообщений. *Пример:* **13475634251-1567456345@g.us** для группы.
$contact = "contact_example"; // string | Контакт. Для ввода доступны форматы:   ID контакта.*Пример: * ** 13475634251 @c.us ** ;   Номер телефона.*Пример: * ** 79002224477 ** .Номер должен начинаться с кода страны. Для России и Казахстана это всегда 7, затем 10 цифр.Сообщения на номера телефона с 8 не будут доставлены.

try {
    $result = $apiInstance->apiSyncGroupAdminDemotePost($profile_id, $chat_id, $contact);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling GroupsApi->apiSyncGroupAdminDemotePost: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **profile_id** | **string**| Profile ID |
 **chat_id** | **string**| Chat ID - ID чата группы из списка сообщений. *Пример:* **13475634251-1567456345@g.us** для группы. |
 **contact** | **string**| Контакт. Для ввода доступны форматы:   ID контакта.*Пример: * ** 13475634251 @c.us ** ;   Номер телефона.*Пример: * ** 79002224477 ** .Номер должен начинаться с кода страны. Для России и Казахстана это всегда 7, затем 10 цифр.Сообщения на номера телефона с 8 не будут доставлены. |

### Return type

[**\Swagger\Client\Model\InlineResponse2002**](../Model/InlineResponse2002.md)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **apiSyncGroupAdminPromovePost**
> \Swagger\Client\Model\InlineResponse2002 apiSyncGroupAdminPromovePost($profile_id, $chat_id, $contact)

Добавить права администратора группы контакту

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\GroupsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$profile_id = "profile_id_example"; // string | Profile ID
$chat_id = "chat_id_example"; // string | Chat ID - ID чата группы из списка сообщений. *Пример:* **13475634251-1567456345@g.us** для группы.
$contact = "contact_example"; // string | Контакт. Для ввода доступны форматы:   ID контакта.*Пример: * ** 13475634251 @c.us ** ;   Номер телефона.*Пример: * ** 79002224477 ** .Номер должен начинаться с кода страны. Для России и Казахстана это всегда 7, затем 10 цифр.Сообщения на номера телефона с 8 не будут доставлены.

try {
    $result = $apiInstance->apiSyncGroupAdminPromovePost($profile_id, $chat_id, $contact);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling GroupsApi->apiSyncGroupAdminPromovePost: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **profile_id** | **string**| Profile ID |
 **chat_id** | **string**| Chat ID - ID чата группы из списка сообщений. *Пример:* **13475634251-1567456345@g.us** для группы. |
 **contact** | **string**| Контакт. Для ввода доступны форматы:   ID контакта.*Пример: * ** 13475634251 @c.us ** ;   Номер телефона.*Пример: * ** 79002224477 ** .Номер должен начинаться с кода страны. Для России и Казахстана это всегда 7, затем 10 цифр.Сообщения на номера телефона с 8 не будут доставлены. |

### Return type

[**\Swagger\Client\Model\InlineResponse2002**](../Model/InlineResponse2002.md)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **apiSyncGroupAdminsGetGet**
> \Swagger\Client\Model\InlineResponse20013 apiSyncGroupAdminsGetGet($profile_id, $chat_id)

Получить список администраторов из группы

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\GroupsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$profile_id = "profile_id_example"; // string | Profile ID
$chat_id = "chat_id_example"; // string | Chat ID - ID чата группы из списка сообщений. *Пример:* **13475634251-1567456345@g.us** для группы.

try {
    $result = $apiInstance->apiSyncGroupAdminsGetGet($profile_id, $chat_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling GroupsApi->apiSyncGroupAdminsGetGet: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **profile_id** | **string**| Profile ID |
 **chat_id** | **string**| Chat ID - ID чата группы из списка сообщений. *Пример:* **13475634251-1567456345@g.us** для группы. |

### Return type

[**\Swagger\Client\Model\InlineResponse20013**](../Model/InlineResponse20013.md)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **apiSyncGroupCreatePost**
> \Swagger\Client\Model\InlineResponse20012 apiSyncGroupCreatePost($body, $profile_id, $name)

Создать новую группу

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\GroupsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \stdClass; // object | Добавление массива контактов. Для ввода доступны форматы:

 ID контакта.*Пример: * ** 13475634251 @c.us ** ;

 Номер телефона.*Пример: * ** 79002224477 ** . Номер должен начинаться с кода страны. Для России и Казахстана это всегда 7, затем 10 цифр.Сообщения на номера телефона с 8 не будут доставлены.

 *Пример массива: * 

 
$profile_id = "profile_id_example"; // string | Profile ID
$name = "name_example"; // string | Название группы

try {
    $result = $apiInstance->apiSyncGroupCreatePost($body, $profile_id, $name);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling GroupsApi->apiSyncGroupCreatePost: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**object**](../Model/object.md)| Добавление массива контактов. Для ввода доступны форматы:

 ID контакта.*Пример: * ** 13475634251 @c.us ** ;

 Номер телефона.*Пример: * ** 79002224477 ** . Номер должен начинаться с кода страны. Для России и Казахстана это всегда 7, затем 10 цифр.Сообщения на номера телефона с 8 не будут доставлены.

 *Пример массива: * 

  |
 **profile_id** | **string**| Profile ID |
 **name** | **string**| Название группы |

### Return type

[**\Swagger\Client\Model\InlineResponse20012**](../Model/InlineResponse20012.md)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **apiSyncGroupLeavePost**
> \Swagger\Client\Model\InlineResponse2002 apiSyncGroupLeavePost($profile_id, $chat_id)

Покинуть группу

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\GroupsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$profile_id = "profile_id_example"; // string | Profile ID
$chat_id = "chat_id_example"; // string | Chat ID - ID чата группы из списка сообщений. *Пример:* **13475634251-1567456345@g.us** для группы.

try {
    $result = $apiInstance->apiSyncGroupLeavePost($profile_id, $chat_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling GroupsApi->apiSyncGroupLeavePost: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **profile_id** | **string**| Profile ID |
 **chat_id** | **string**| Chat ID - ID чата группы из списка сообщений. *Пример:* **13475634251-1567456345@g.us** для группы. |

### Return type

[**\Swagger\Client\Model\InlineResponse2002**](../Model/InlineResponse2002.md)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **apiSyncGroupParticipantAddPost**
> \Swagger\Client\Model\InlineResponse2002 apiSyncGroupParticipantAddPost($profile_id, $chat_id, $contact)

Добавить контакт в группу

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\GroupsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$profile_id = "profile_id_example"; // string | Profile ID
$chat_id = "chat_id_example"; // string | Chat ID - ID чата группы из списка сообщений. *Пример:* **13475634251-1567456345@g.us** для группы.
$contact = "contact_example"; // string | Контакт. Для ввода доступны форматы:   ID контакта.*Пример: * ** 13475634251 @c.us ** ;   Номер телефона.*Пример: * ** 79002224477 ** .Номер должен начинаться с кода страны. Для России и Казахстана это всегда 7, затем 10 цифр.Сообщения на номера телефона с 8 не будут доставлены.

try {
    $result = $apiInstance->apiSyncGroupParticipantAddPost($profile_id, $chat_id, $contact);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling GroupsApi->apiSyncGroupParticipantAddPost: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **profile_id** | **string**| Profile ID |
 **chat_id** | **string**| Chat ID - ID чата группы из списка сообщений. *Пример:* **13475634251-1567456345@g.us** для группы. |
 **contact** | **string**| Контакт. Для ввода доступны форматы:   ID контакта.*Пример: * ** 13475634251 @c.us ** ;   Номер телефона.*Пример: * ** 79002224477 ** .Номер должен начинаться с кода страны. Для России и Казахстана это всегда 7, затем 10 цифр.Сообщения на номера телефона с 8 не будут доставлены. |

### Return type

[**\Swagger\Client\Model\InlineResponse2002**](../Model/InlineResponse2002.md)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **apiSyncGroupParticipantRemovePost**
> \Swagger\Client\Model\InlineResponse2002 apiSyncGroupParticipantRemovePost($profile_id, $chat_id, $contact)

Удалить контакт из группы

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\GroupsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$profile_id = "profile_id_example"; // string | Profile ID
$chat_id = "chat_id_example"; // string | Chat ID - ID чата группы из списка сообщений. *Пример:* **13475634251-1567456345@g.us** для группы.
$contact = "contact_example"; // string | Контакт. Для ввода доступны форматы:   ID контакта.*Пример: * ** 13475634251 @c.us ** ;   Номер телефона.*Пример: * ** 79002224477 ** .Номер должен начинаться с кода страны. Для России и Казахстана это всегда 7, затем 10 цифр.Сообщения на номера телефона с 8 не будут доставлены.

try {
    $result = $apiInstance->apiSyncGroupParticipantRemovePost($profile_id, $chat_id, $contact);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling GroupsApi->apiSyncGroupParticipantRemovePost: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **profile_id** | **string**| Profile ID |
 **chat_id** | **string**| Chat ID - ID чата группы из списка сообщений. *Пример:* **13475634251-1567456345@g.us** для группы. |
 **contact** | **string**| Контакт. Для ввода доступны форматы:   ID контакта.*Пример: * ** 13475634251 @c.us ** ;   Номер телефона.*Пример: * ** 79002224477 ** .Номер должен начинаться с кода страны. Для России и Казахстана это всегда 7, затем 10 цифр.Сообщения на номера телефона с 8 не будут доставлены. |

### Return type

[**\Swagger\Client\Model\InlineResponse2002**](../Model/InlineResponse2002.md)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **apiSyncGroupParticipantsGetGet**
> \Swagger\Client\Model\InlineResponse2004 apiSyncGroupParticipantsGetGet($profile_id, $chat_id)

Получить контакты из группы

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\GroupsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$profile_id = "profile_id_example"; // string | Profile ID
$chat_id = "chat_id_example"; // string | Chat ID - ID чата группы из списка сообщений. *Пример:* **13475634251-1567456345@g.us** для группы.

try {
    $result = $apiInstance->apiSyncGroupParticipantsGetGet($profile_id, $chat_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling GroupsApi->apiSyncGroupParticipantsGetGet: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **profile_id** | **string**| Profile ID |
 **chat_id** | **string**| Chat ID - ID чата группы из списка сообщений. *Пример:* **13475634251-1567456345@g.us** для группы. |

### Return type

[**\Swagger\Client\Model\InlineResponse2004**](../Model/InlineResponse2004.md)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

