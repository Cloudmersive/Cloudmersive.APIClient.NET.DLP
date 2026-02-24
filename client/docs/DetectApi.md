# Cloudmersive.APIClient.NET.DLP.Api.DetectApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**DetectDocument**](DetectApi.md#detectdocument) | **POST** /dlp/detect/document | Detect User Data in Document Image |
| [**DetectDocumentAdvanced**](DetectApi.md#detectdocumentadvanced) | **POST** /dlp/detect/document/advanced | Detect User Data in Document Image (Advanced) |
| [**DetectText**](DetectApi.md#detecttext) | **POST** /dlp/detect/text | Detect User Data in Input Text |
| [**DetectTextAdvanced**](DetectApi.md#detecttextadvanced) | **POST** /dlp/detect/text/advanced | Detect User Data in Input Text (Advanced) |

<a id="detectdocument"></a>
# **DetectDocument**
> DlpDetectionResponse DetectDocument (DlpDocumentDetectionRequest body = null)

Detect User Data in Document Image

Detects configurable types of user data in a document (PDF, DOC, DOCX, XLS, XLSX, PPT, PPTX, HTML, EML, MSG, PNG, JPG, WEBP) using Advanced AI.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Cloudmersive.APIClient.NET.DLP.Api;
using Cloudmersive.APIClient.NET.DLP.Client;
using Cloudmersive.APIClient.NET.DLP.Model;

namespace Example
{
    public class DetectDocumentExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "http://localhost";
            // Configure API key authorization: Apikey
            config.AddApiKey("Apikey", "YOUR_API_KEY");
            // Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
            // config.AddApiKeyPrefix("Apikey", "Bearer");

            var apiInstance = new DetectApi(config);
            var body = new DlpDocumentDetectionRequest(); // DlpDocumentDetectionRequest | Input request (optional) 

            try
            {
                // Detect User Data in Document Image
                DlpDetectionResponse result = apiInstance.DetectDocument(body);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling DetectApi.DetectDocument: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the DetectDocumentWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Detect User Data in Document Image
    ApiResponse<DlpDetectionResponse> response = apiInstance.DetectDocumentWithHttpInfo(body);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling DetectApi.DetectDocumentWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **body** | [**DlpDocumentDetectionRequest**](DlpDocumentDetectionRequest.md) | Input request | [optional]  |

### Return type

[**DlpDetectionResponse**](DlpDetectionResponse.md)

### Authorization

[Apikey](../README.md#Apikey)

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/*+json
 - **Accept**: text/plain, application/json, text/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="detectdocumentadvanced"></a>
# **DetectDocumentAdvanced**
> DlpAdvancedDetectionResponse DetectDocumentAdvanced (DlpAdvancedDocumentDetectionRequest body = null)

Detect User Data in Document Image (Advanced)

Detects 29 configurable types of user data including health-related PHI in a document (PDF, DOC, DOCX, XLS, XLSX, PPT, PPTX, HTML, EML, MSG, PNG, JPG, WEBP) using Advanced AI.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Cloudmersive.APIClient.NET.DLP.Api;
using Cloudmersive.APIClient.NET.DLP.Client;
using Cloudmersive.APIClient.NET.DLP.Model;

namespace Example
{
    public class DetectDocumentAdvancedExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "http://localhost";
            // Configure API key authorization: Apikey
            config.AddApiKey("Apikey", "YOUR_API_KEY");
            // Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
            // config.AddApiKeyPrefix("Apikey", "Bearer");

            var apiInstance = new DetectApi(config);
            var body = new DlpAdvancedDocumentDetectionRequest(); // DlpAdvancedDocumentDetectionRequest | Input request (optional) 

            try
            {
                // Detect User Data in Document Image (Advanced)
                DlpAdvancedDetectionResponse result = apiInstance.DetectDocumentAdvanced(body);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling DetectApi.DetectDocumentAdvanced: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the DetectDocumentAdvancedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Detect User Data in Document Image (Advanced)
    ApiResponse<DlpAdvancedDetectionResponse> response = apiInstance.DetectDocumentAdvancedWithHttpInfo(body);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling DetectApi.DetectDocumentAdvancedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **body** | [**DlpAdvancedDocumentDetectionRequest**](DlpAdvancedDocumentDetectionRequest.md) | Input request | [optional]  |

### Return type

[**DlpAdvancedDetectionResponse**](DlpAdvancedDetectionResponse.md)

### Authorization

[Apikey](../README.md#Apikey)

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/*+json
 - **Accept**: text/plain, application/json, text/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="detecttext"></a>
# **DetectText**
> DlpDetectionResponse DetectText (DlpDetectionRequest body = null)

Detect User Data in Input Text

Detects configurable types of user data in an input text string using Advanced AI.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Cloudmersive.APIClient.NET.DLP.Api;
using Cloudmersive.APIClient.NET.DLP.Client;
using Cloudmersive.APIClient.NET.DLP.Model;

namespace Example
{
    public class DetectTextExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "http://localhost";
            // Configure API key authorization: Apikey
            config.AddApiKey("Apikey", "YOUR_API_KEY");
            // Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
            // config.AddApiKeyPrefix("Apikey", "Bearer");

            var apiInstance = new DetectApi(config);
            var body = new DlpDetectionRequest(); // DlpDetectionRequest | Input request (optional) 

            try
            {
                // Detect User Data in Input Text
                DlpDetectionResponse result = apiInstance.DetectText(body);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling DetectApi.DetectText: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the DetectTextWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Detect User Data in Input Text
    ApiResponse<DlpDetectionResponse> response = apiInstance.DetectTextWithHttpInfo(body);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling DetectApi.DetectTextWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **body** | [**DlpDetectionRequest**](DlpDetectionRequest.md) | Input request | [optional]  |

### Return type

[**DlpDetectionResponse**](DlpDetectionResponse.md)

### Authorization

[Apikey](../README.md#Apikey)

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/*+json
 - **Accept**: text/plain, application/json, text/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="detecttextadvanced"></a>
# **DetectTextAdvanced**
> DlpAdvancedDetectionResponse DetectTextAdvanced (DlpAdvancedDetectionRequest body = null)

Detect User Data in Input Text (Advanced)

Detects 29 configurable types of user data including health-related PHI in an input text string using Advanced AI.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Cloudmersive.APIClient.NET.DLP.Api;
using Cloudmersive.APIClient.NET.DLP.Client;
using Cloudmersive.APIClient.NET.DLP.Model;

namespace Example
{
    public class DetectTextAdvancedExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "http://localhost";
            // Configure API key authorization: Apikey
            config.AddApiKey("Apikey", "YOUR_API_KEY");
            // Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
            // config.AddApiKeyPrefix("Apikey", "Bearer");

            var apiInstance = new DetectApi(config);
            var body = new DlpAdvancedDetectionRequest(); // DlpAdvancedDetectionRequest | Input request (optional) 

            try
            {
                // Detect User Data in Input Text (Advanced)
                DlpAdvancedDetectionResponse result = apiInstance.DetectTextAdvanced(body);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling DetectApi.DetectTextAdvanced: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the DetectTextAdvancedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Detect User Data in Input Text (Advanced)
    ApiResponse<DlpAdvancedDetectionResponse> response = apiInstance.DetectTextAdvancedWithHttpInfo(body);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling DetectApi.DetectTextAdvancedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **body** | [**DlpAdvancedDetectionRequest**](DlpAdvancedDetectionRequest.md) | Input request | [optional]  |

### Return type

[**DlpAdvancedDetectionResponse**](DlpAdvancedDetectionResponse.md)

### Authorization

[Apikey](../README.md#Apikey)

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/*+json
 - **Accept**: text/plain, application/json, text/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

