# Swagger\Client\WebhookApi

All URIs are relative to *https://wappi.pro*

Method | HTTP request | Description
------------- | ------------- | -------------
[**apiWebhookUrlDeletePost**](WebhookApi.md#apiwebhookurldeletepost) | **POST** /api/webhook/url/delete | Удалить ссылку на webhook
[**apiWebhookUrlGetGet**](WebhookApi.md#apiwebhookurlgetget) | **GET** /api/webhook/url/get | Получить ссылку на webhook
[**apiWebhookUrlSetPost**](WebhookApi.md#apiwebhookurlsetpost) | **POST** /api/webhook/url/set | Установить ссылку на webhook для уведомлений

# **apiWebhookUrlDeletePost**
> \Swagger\Client\Model\InlineResponse20016 apiWebhookUrlDeletePost($profile_id)

Удалить ссылку на webhook

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\WebhookApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$profile_id = "profile_id_example"; // string | Profile ID

try {
    $result = $apiInstance->apiWebhookUrlDeletePost($profile_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling WebhookApi->apiWebhookUrlDeletePost: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **profile_id** | **string**| Profile ID |

### Return type

[**\Swagger\Client\Model\InlineResponse20016**](../Model/InlineResponse20016.md)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **apiWebhookUrlGetGet**
> \Swagger\Client\Model\InlineResponse20014 apiWebhookUrlGetGet($profile_id)

Получить ссылку на webhook

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\WebhookApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$profile_id = "profile_id_example"; // string | Profile ID

try {
    $result = $apiInstance->apiWebhookUrlGetGet($profile_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling WebhookApi->apiWebhookUrlGetGet: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **profile_id** | **string**| Profile ID |

### Return type

[**\Swagger\Client\Model\InlineResponse20014**](../Model/InlineResponse20014.md)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **apiWebhookUrlSetPost**
> \Swagger\Client\Model\InlineResponse20015 apiWebhookUrlSetPost($profile_id, $url)

Установить ссылку на webhook для уведомлений

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\WebhookApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$profile_id = "profile_id_example"; // string | Profile ID
$url = "url_example"; // string | <your url>

try {
    $result = $apiInstance->apiWebhookUrlSetPost($profile_id, $url);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling WebhookApi->apiWebhookUrlSetPost: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **profile_id** | **string**| Profile ID |
 **url** | **string**| &lt;your url&gt; |

### Return type

[**\Swagger\Client\Model\InlineResponse20015**](../Model/InlineResponse20015.md)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

