# Swagger\Client\TasksApi

All URIs are relative to *https://wappi.pro*

Method | HTTP request | Description
------------- | ------------- | -------------
[**apiTasksClearPendingPost**](TasksApi.md#apitasksclearpendingpost) | **POST** /api/tasks/clear/pending | Удалить из очереди ожидающие выполнения асинхронные задачи
[**apiTasksGetGet**](TasksApi.md#apitasksgetget) | **GET** /api/tasks/get | Получить список асинхронных задач

# **apiTasksClearPendingPost**
> \Swagger\Client\Model\InlineResponse20011 apiTasksClearPendingPost($profile_id)

Удалить из очереди ожидающие выполнения асинхронные задачи

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\TasksApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$profile_id = "profile_id_example"; // string | Profile ID

try {
    $result = $apiInstance->apiTasksClearPendingPost($profile_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling TasksApi->apiTasksClearPendingPost: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **profile_id** | **string**| Profile ID |

### Return type

[**\Swagger\Client\Model\InlineResponse20011**](../Model/InlineResponse20011.md)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **apiTasksGetGet**
> \Swagger\Client\Model\InlineResponse20010 apiTasksGetGet($profile_id, $limit, $task_id)

Получить список асинхронных задач

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
// Configure API key authorization: api_key
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

$apiInstance = new Swagger\Client\Api\TasksApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$profile_id = "profile_id_example"; // string | Profile ID
$limit = 56; // int | limit
$task_id = "task_id_example"; // string | Task ID

try {
    $result = $apiInstance->apiTasksGetGet($profile_id, $limit, $task_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling TasksApi->apiTasksGetGet: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **profile_id** | **string**| Profile ID |
 **limit** | **int**| limit | [optional]
 **task_id** | **string**| Task ID | [optional]

### Return type

[**\Swagger\Client\Model\InlineResponse20010**](../Model/InlineResponse20010.md)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

