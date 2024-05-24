# Swagger\Client\ContactsApi

All URIs are relative to *https://wappi.pro*

Method | HTTP request | Description
------------- | ------------- | -------------
[**apiSyncContactBlockPost**](ContactsApi.md#apisynccontactblockpost) | **POST** /api/sync/contact/block | Заблокировать контакт
[**apiSyncContactGetGet**](ContactsApi.md#apisynccontactgetget) | **GET** /api/sync/contact/get | Получить информацию о контакте
[**apiSyncContactRegisteredCheckPost**](ContactsApi.md#apisynccontactregisteredcheckpost) | **POST** /api/sync/contact/registered/check | Проверка зарегестрирован ли контакт
[**apiSyncContactUnblockPost**](ContactsApi.md#apisynccontactunblockpost) | **POST** /api/sync/contact/unblock | Разблокировать контакт
[**apiSyncContactsGetGet**](ContactsApi.md#apisynccontactsgetget) | **GET** /api/sync/contacts/get | Получить список контактов

# **apiSyncContactBlockPost**
> \Swagger\Client\Model\InlineResponse2002 apiSyncContactBlockPost($profile_id, $contact)

Заблокировать контакт

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ContactsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$profile_id = "profile_id_example"; // string | Profile ID
$contact = "contact_example"; // string | Контакт. Для ввода доступны форматы:   ID контакта.*Пример: * ** 13475634251 @c.us ** ;   Номер телефона.*Пример: * ** 79002224477 ** .Номер должен начинаться с кода страны. Для России и Казахстана это всегда 7, затем 10 цифр.Сообщения на номера телефона с 8 не будут доставлены.

try {
    $result = $apiInstance->apiSyncContactBlockPost($profile_id, $contact);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ContactsApi->apiSyncContactBlockPost: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **profile_id** | **string**| Profile ID |
 **contact** | **string**| Контакт. Для ввода доступны форматы:   ID контакта.*Пример: * ** 13475634251 @c.us ** ;   Номер телефона.*Пример: * ** 79002224477 ** .Номер должен начинаться с кода страны. Для России и Казахстана это всегда 7, затем 10 цифр.Сообщения на номера телефона с 8 не будут доставлены. |

### Return type

[**\Swagger\Client\Model\InlineResponse2002**](../Model/InlineResponse2002.md)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **apiSyncContactGetGet**
> \Swagger\Client\Model\InlineResponse2005 apiSyncContactGetGet($profile_id, $contact, $profile_pic)

Получить информацию о контакте

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ContactsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$profile_id = "profile_id_example"; // string | Profile ID
$contact = "contact_example"; // string | Контакт. Для ввода доступны форматы:   ID контакта.*Пример: * ** 13475634251 @c.us ** ;   Номер телефона.*Пример: * ** 79002224477 ** .Номер должен начинаться с кода страны. Для России и Казахстана это всегда 7, затем 10 цифр.Сообщения на номера телефона с 8 не будут доставлены.
$profile_pic = "profile_pic_example"; // string | Получить картинку профиля, может принимать значения base64 или url

try {
    $result = $apiInstance->apiSyncContactGetGet($profile_id, $contact, $profile_pic);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ContactsApi->apiSyncContactGetGet: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **profile_id** | **string**| Profile ID |
 **contact** | **string**| Контакт. Для ввода доступны форматы:   ID контакта.*Пример: * ** 13475634251 @c.us ** ;   Номер телефона.*Пример: * ** 79002224477 ** .Номер должен начинаться с кода страны. Для России и Казахстана это всегда 7, затем 10 цифр.Сообщения на номера телефона с 8 не будут доставлены. |
 **profile_pic** | **string**| Получить картинку профиля, может принимать значения base64 или url | [optional]

### Return type

[**\Swagger\Client\Model\InlineResponse2005**](../Model/InlineResponse2005.md)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **apiSyncContactRegisteredCheckPost**
> \Swagger\Client\Model\InlineResponse2009 apiSyncContactRegisteredCheckPost($profile_id, $contact)

Проверка зарегестрирован ли контакт

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ContactsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$profile_id = "profile_id_example"; // string | Profile ID
$contact = "contact_example"; // string | Контакт. Для ввода доступны форматы:   ID контакта.*Пример: * ** 13475634251 @c.us ** ;   Номер телефона.*Пример: * ** 79002224477 ** .Номер должен начинаться с кода страны. Для России и Казахстана это всегда 7, затем 10 цифр.Сообщения на номера телефона с 8 не будут доставлены.

try {
    $result = $apiInstance->apiSyncContactRegisteredCheckPost($profile_id, $contact);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ContactsApi->apiSyncContactRegisteredCheckPost: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **profile_id** | **string**| Profile ID |
 **contact** | **string**| Контакт. Для ввода доступны форматы:   ID контакта.*Пример: * ** 13475634251 @c.us ** ;   Номер телефона.*Пример: * ** 79002224477 ** .Номер должен начинаться с кода страны. Для России и Казахстана это всегда 7, затем 10 цифр.Сообщения на номера телефона с 8 не будут доставлены. |

### Return type

[**\Swagger\Client\Model\InlineResponse2009**](../Model/InlineResponse2009.md)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **apiSyncContactUnblockPost**
> \Swagger\Client\Model\InlineResponse2002 apiSyncContactUnblockPost($profile_id, $contact)

Разблокировать контакт

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ContactsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$profile_id = "profile_id_example"; // string | Profile ID
$contact = "contact_example"; // string | Контакт. Для ввода доступны форматы:   ID контакта.*Пример: * ** 13475634251 @c.us ** ;   Номер телефона.*Пример: * ** 79002224477 ** .Номер должен начинаться с кода страны. Для России и Казахстана это всегда 7, затем 10 цифр.Сообщения на номера телефона с 8 не будут доставлены.

try {
    $result = $apiInstance->apiSyncContactUnblockPost($profile_id, $contact);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ContactsApi->apiSyncContactUnblockPost: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **profile_id** | **string**| Profile ID |
 **contact** | **string**| Контакт. Для ввода доступны форматы:   ID контакта.*Пример: * ** 13475634251 @c.us ** ;   Номер телефона.*Пример: * ** 79002224477 ** .Номер должен начинаться с кода страны. Для России и Казахстана это всегда 7, затем 10 цифр.Сообщения на номера телефона с 8 не будут доставлены. |

### Return type

[**\Swagger\Client\Model\InlineResponse2002**](../Model/InlineResponse2002.md)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **apiSyncContactsGetGet**
> \Swagger\Client\Model\InlineResponse2004 apiSyncContactsGetGet($profile_id)

Получить список контактов

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ContactsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$profile_id = "profile_id_example"; // string | Profile ID

try {
    $result = $apiInstance->apiSyncContactsGetGet($profile_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ContactsApi->apiSyncContactsGetGet: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **profile_id** | **string**| Profile ID |

### Return type

[**\Swagger\Client\Model\InlineResponse2004**](../Model/InlineResponse2004.md)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

