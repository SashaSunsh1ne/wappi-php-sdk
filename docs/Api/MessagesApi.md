# Swagger\Client\MessagesApi

All URIs are relative to *https://wappi.pro*

Method | HTTP request | Description
------------- | ------------- | -------------
[**apiSyncMessageDeletePost**](MessagesApi.md#apisyncmessagedeletepost) | **POST** /api/sync/message/delete | Удалить сообщение
[**apiSyncMessageFileSendPost**](MessagesApi.md#apisyncmessagefilesendpost) | **POST** /api/sync/message/file/send | Отправить файл
[**apiSyncMessageReplyPost**](MessagesApi.md#apisyncmessagereplypost) | **POST** /api/sync/message/reply | Ответить на сообщение
[**apiSyncMessageSendPost**](MessagesApi.md#apisyncmessagesendpost) | **POST** /api/sync/message/send | Отправить сообщение
[**apiSyncMessagesGetGet**](MessagesApi.md#apisyncmessagesgetget) | **GET** /api/sync/messages/get | Получить сообщения
[**apiSyncMessagesUnreadGetGet**](MessagesApi.md#apisyncmessagesunreadgetget) | **GET** /api/sync/messages/unread/get | Получить непрочитанные сообщения

# **apiSyncMessageDeletePost**
> \Swagger\Client\Model\InlineResponse2002 apiSyncMessageDeletePost($profile_id, $message_id)

Удалить сообщение

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\MessagesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$profile_id = "profile_id_example"; // string | Profile ID
$message_id = "message_id_example"; // string | ID сообщения в формате **false_9001112233@c.us_4EB1F19C471F4A61CC5A**

try {
    $result = $apiInstance->apiSyncMessageDeletePost($profile_id, $message_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling MessagesApi->apiSyncMessageDeletePost: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **profile_id** | **string**| Profile ID |
 **message_id** | **string**| ID сообщения в формате **false_9001112233@c.us_4EB1F19C471F4A61CC5A** |

### Return type

[**\Swagger\Client\Model\InlineResponse2002**](../Model/InlineResponse2002.md)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **apiSyncMessageFileSendPost**
> \Swagger\Client\Model\InlineResponse2001 apiSyncMessageFileSendPost($profile_id, $recipient, $file, $create, $file_type, $caption)

Отправить файл

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\MessagesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$profile_id = "profile_id_example"; // string | Profile ID
$recipient = "recipient_example"; // string | Получатель. Для ввода доступны форматы:   Chat ID - ID чата из списка сообщений.*Примеры: * ** 13475634251 @c.us ** для личных сообщений и ** 13475634251 - 1567456345 @g.us ** для группы;   Номер телефона.*Пример: * ** 79002224477 ** .Номер должен начинаться с кода страны.Для России и Казахстана это всегда 7, затем 10 цифр.Сообщения на номера телефона с 8 не будут доставлены.
$file = "file_example"; // string | 
$create = true; // bool | Создать новый чат, если его нет.
$file_type = "file"; // string | Тип файла.
$caption = ""; // string | Подпись к файлу.

try {
    $result = $apiInstance->apiSyncMessageFileSendPost($profile_id, $recipient, $file, $create, $file_type, $caption);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling MessagesApi->apiSyncMessageFileSendPost: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **profile_id** | **string**| Profile ID |
 **recipient** | **string**| Получатель. Для ввода доступны форматы:   Chat ID - ID чата из списка сообщений.*Примеры: * ** 13475634251 @c.us ** для личных сообщений и ** 13475634251 - 1567456345 @g.us ** для группы;   Номер телефона.*Пример: * ** 79002224477 ** .Номер должен начинаться с кода страны.Для России и Казахстана это всегда 7, затем 10 цифр.Сообщения на номера телефона с 8 не будут доставлены. |
 **file** | **string****string**|  | [optional]
 **create** | **bool**| Создать новый чат, если его нет. | [optional] [default to true]
 **file_type** | **string**| Тип файла. | [optional] [default to file]
 **caption** | **string**| Подпись к файлу. | [optional]

### Return type

[**\Swagger\Client\Model\InlineResponse2001**](../Model/InlineResponse2001.md)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **apiSyncMessageReplyPost**
> \Swagger\Client\Model\InlineResponse2001 apiSyncMessageReplyPost($profile_id, $message_id)

Ответить на сообщение

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\MessagesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$profile_id = "profile_id_example"; // string | Profile ID
$message_id = "message_id_example"; // string | ID сообщения в формате **false_9001112233@c.us_4EB1F19C471F4A61CC5A**

try {
    $result = $apiInstance->apiSyncMessageReplyPost($profile_id, $message_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling MessagesApi->apiSyncMessageReplyPost: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **profile_id** | **string**| Profile ID |
 **message_id** | **string**| ID сообщения в формате **false_9001112233@c.us_4EB1F19C471F4A61CC5A** |

### Return type

[**\Swagger\Client\Model\InlineResponse2001**](../Model/InlineResponse2001.md)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/x-www-form-urlencoded
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **apiSyncMessageSendPost**
> \Swagger\Client\Model\InlineResponse2001 apiSyncMessageSendPost($body, $profile_id, $recipient, $create)

Отправить сообщение

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\MessagesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = "body_example"; // string | Текст сообщения - любая строка, включая emoji.
$profile_id = "profile_id_example"; // string | Profile ID
$recipient = "recipient_example"; // string | Получатель. Для ввода доступны форматы:   Chat ID - ID чата из списка сообщений.*Примеры: * ** 13475634251 @c.us ** для личных сообщений и ** 13475634251 - 1567456345 @g.us ** для группы;   Номер телефона.*Пример: * ** 79002224477 ** .Номер должен начинаться с кода страны.Для России и Казахстана это всегда 7, затем 10 цифр.Сообщения на номера телефона с 8 не будут доставлены.
$create = true; // bool | Создавать новый чат, если его нет.

try {
    $result = $apiInstance->apiSyncMessageSendPost($body, $profile_id, $recipient, $create);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling MessagesApi->apiSyncMessageSendPost: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**string**](../Model/string.md)| Текст сообщения - любая строка, включая emoji. |
 **profile_id** | **string**| Profile ID |
 **recipient** | **string**| Получатель. Для ввода доступны форматы:   Chat ID - ID чата из списка сообщений.*Примеры: * ** 13475634251 @c.us ** для личных сообщений и ** 13475634251 - 1567456345 @g.us ** для группы;   Номер телефона.*Пример: * ** 79002224477 ** .Номер должен начинаться с кода страны.Для России и Казахстана это всегда 7, затем 10 цифр.Сообщения на номера телефона с 8 не будут доставлены. |
 **create** | **bool**| Создавать новый чат, если его нет. | [optional] [default to true]

### Return type

[**\Swagger\Client\Model\InlineResponse2001**](../Model/InlineResponse2001.md)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: text/plain
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **apiSyncMessagesGetGet**
> \Swagger\Client\Model\InlineResponse2007 apiSyncMessagesGetGet($profile_id, $chat_id, $include_me, $filters, $include_notifications, $load_all_msg)

Получить сообщения

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\MessagesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$profile_id = "profile_id_example"; // string | Profile ID
$chat_id = "chat_id_example"; // string | Chat ID - ID чата из списка сообщений. *Примеры:* **13475634251@c.us** для личных сообщений и **13475634251-1567456345@g.us** для группы.
$include_me = false; // bool | Включать собственные сообщения.
$filters = "all"; // string | Все сообщения или только непрочитанные.
$include_notifications = false; // bool | Включать notifications.
$load_all_msg = false; // bool | Загружать все сообщения (ВНИМАНИЕ: работает только в асинхронном режиме).

try {
    $result = $apiInstance->apiSyncMessagesGetGet($profile_id, $chat_id, $include_me, $filters, $include_notifications, $load_all_msg);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling MessagesApi->apiSyncMessagesGetGet: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **profile_id** | **string**| Profile ID |
 **chat_id** | **string**| Chat ID - ID чата из списка сообщений. *Примеры:* **13475634251@c.us** для личных сообщений и **13475634251-1567456345@g.us** для группы. |
 **include_me** | **bool**| Включать собственные сообщения. | [optional] [default to false]
 **filters** | **string**| Все сообщения или только непрочитанные. | [optional] [default to all]
 **include_notifications** | **bool**| Включать notifications. | [optional] [default to false]
 **load_all_msg** | **bool**| Загружать все сообщения (ВНИМАНИЕ: работает только в асинхронном режиме). | [optional] [default to false]

### Return type

[**\Swagger\Client\Model\InlineResponse2007**](../Model/InlineResponse2007.md)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **apiSyncMessagesUnreadGetGet**
> \Swagger\Client\Model\InlineResponse2008 apiSyncMessagesUnreadGetGet($profile_id)

Получить непрочитанные сообщения

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\MessagesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$profile_id = "profile_id_example"; // string | Profile ID

try {
    $result = $apiInstance->apiSyncMessagesUnreadGetGet($profile_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling MessagesApi->apiSyncMessagesUnreadGetGet: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **profile_id** | **string**| Profile ID |

### Return type

[**\Swagger\Client\Model\InlineResponse2008**](../Model/InlineResponse2008.md)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

