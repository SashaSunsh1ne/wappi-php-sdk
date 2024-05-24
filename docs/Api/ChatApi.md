# Swagger\Client\ChatApi

All URIs are relative to *https://wappi.pro*

Method | HTTP request | Description
------------- | ------------- | -------------
[**apiSyncChatDeletePost**](ChatApi.md#apisyncchatdeletepost) | **POST** /api/sync/chat/delete | Удалить чат
[**apiSyncChatSeenSendPost**](ChatApi.md#apisyncchatseensendpost) | **POST** /api/sync/chat/seen/send | Отметить сообщения прочитанными в чате
[**apiSyncChatsGetGet**](ChatApi.md#apisyncchatsgetget) | **GET** /api/sync/chats/get | Получить список чатов

# **apiSyncChatDeletePost**
> \Swagger\Client\Model\InlineResponse2002 apiSyncChatDeletePost($profile_id, $chat_id)

Удалить чат

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ChatApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$profile_id = "profile_id_example"; // string | Profile ID
$chat_id = "chat_id_example"; // string | Chat ID - ID чата из списка сообщений. *Примеры:* **13475634251@c.us** для личных сообщений и **13475634251-1567456345@g.us** для группы.

try {
    $result = $apiInstance->apiSyncChatDeletePost($profile_id, $chat_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ChatApi->apiSyncChatDeletePost: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **profile_id** | **string**| Profile ID |
 **chat_id** | **string**| Chat ID - ID чата из списка сообщений. *Примеры:* **13475634251@c.us** для личных сообщений и **13475634251-1567456345@g.us** для группы. |

### Return type

[**\Swagger\Client\Model\InlineResponse2002**](../Model/InlineResponse2002.md)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **apiSyncChatSeenSendPost**
> \Swagger\Client\Model\InlineResponse2002 apiSyncChatSeenSendPost($profile_id, $chat_id)

Отметить сообщения прочитанными в чате

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ChatApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$profile_id = "profile_id_example"; // string | Profile ID
$chat_id = "chat_id_example"; // string | Chat ID - ID чата из списка сообщений. *Примеры:* **13475634251@c.us** для личных сообщений и **13475634251-1567456345@g.us** для группы.

try {
    $result = $apiInstance->apiSyncChatSeenSendPost($profile_id, $chat_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ChatApi->apiSyncChatSeenSendPost: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **profile_id** | **string**| Profile ID |
 **chat_id** | **string**| Chat ID - ID чата из списка сообщений. *Примеры:* **13475634251@c.us** для личных сообщений и **13475634251-1567456345@g.us** для группы. |

### Return type

[**\Swagger\Client\Model\InlineResponse2002**](../Model/InlineResponse2002.md)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **apiSyncChatsGetGet**
> \Swagger\Client\Model\InlineResponse2006 apiSyncChatsGetGet($profile_id)

Получить список чатов

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\ChatApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$profile_id = "profile_id_example"; // string | Profile ID

try {
    $result = $apiInstance->apiSyncChatsGetGet($profile_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ChatApi->apiSyncChatsGetGet: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **profile_id** | **string**| Profile ID |

### Return type

[**\Swagger\Client\Model\InlineResponse2006**](../Model/InlineResponse2006.md)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

