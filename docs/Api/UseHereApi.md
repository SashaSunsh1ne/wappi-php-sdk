# Swagger\Client\UseHereApi

All URIs are relative to *https://wappi.pro*

Method | HTTP request | Description
------------- | ------------- | -------------
[**apiSyncUseHerePost**](UseHereApi.md#apisyncuseherepost) | **POST** /api/sync/use/here | Принудительное использование браузера у нас, если залогинен в другом браузере

# **apiSyncUseHerePost**
> \Swagger\Client\Model\InlineResponse2002 apiSyncUseHerePost($profile_id)

Принудительное использование браузера у нас, если залогинен в другом браузере

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\UseHereApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$profile_id = "profile_id_example"; // string | Profile ID

try {
    $result = $apiInstance->apiSyncUseHerePost($profile_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UseHereApi->apiSyncUseHerePost: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **profile_id** | **string**| Profile ID |

### Return type

[**\Swagger\Client\Model\InlineResponse2002**](../Model/InlineResponse2002.md)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

