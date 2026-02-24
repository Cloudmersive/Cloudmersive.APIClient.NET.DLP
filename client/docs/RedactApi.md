# Cloudmersive.APIClient.NET.DLP.Api.RedactApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**RedactDocument**](RedactApi.md#redactdocument) | **POST** /dlp/redact/document | Redact User Data in Document |
| [**RedactDocumentAdvanced**](RedactApi.md#redactdocumentadvanced) | **POST** /dlp/redact/document/advanced | Redact User Data in Document (Advanced) |
| [**RedactText**](RedactApi.md#redacttext) | **POST** /dlp/redact/text | Redact User Data in Input Text |
| [**RedactTextAdvanced**](RedactApi.md#redacttextadvanced) | **POST** /dlp/redact/text/advanced | Redact User Data in Input Text (Advanced) |

<a id="redactdocument"></a>
# **RedactDocument**
> DlpDocumentRedactionResponse RedactDocument (DlpDocumentRedactionRequest body = null)

Redact User Data in Document

Detects and redacts configurable types of user data in a document (PDF, DOC, DOCX, XLS, XLSX, PPT, PPTX, HTML, EML, MSG, PNG, JPG, WEBP) using Advanced AI. Rasterizes document pages, detects PII regions using a grid-overlay approach, blurs those regions, and returns a rasterized PDF.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Cloudmersive.APIClient.NET.DLP.Api;
using Cloudmersive.APIClient.NET.DLP.Client;
using Cloudmersive.APIClient.NET.DLP.Model;

namespace Example
{
    public class RedactDocumentExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "http://localhost";
            // Configure API key authorization: Apikey
            config.AddApiKey("Apikey", "YOUR_API_KEY");
            // Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
            // config.AddApiKeyPrefix("Apikey", "Bearer");

            var apiInstance = new RedactApi(config);
            var body = new DlpDocumentRedactionRequest(); // DlpDocumentRedactionRequest | Input request (optional) 

            try
            {
                // Redact User Data in Document
                DlpDocumentRedactionResponse result = apiInstance.RedactDocument(body);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling RedactApi.RedactDocument: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the RedactDocumentWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Redact User Data in Document
    ApiResponse<DlpDocumentRedactionResponse> response = apiInstance.RedactDocumentWithHttpInfo(body);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling RedactApi.RedactDocumentWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **body** | [**DlpDocumentRedactionRequest**](DlpDocumentRedactionRequest.md) | Input request | [optional]  |

### Return type

[**DlpDocumentRedactionResponse**](DlpDocumentRedactionResponse.md)

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

<a id="redactdocumentadvanced"></a>
# **RedactDocumentAdvanced**
> DlpAdvancedDocumentRedactionResponse RedactDocumentAdvanced (DlpAdvancedDocumentRedactionRequest body = null)

Redact User Data in Document (Advanced)

Detects and redacts 35 configurable types of user data including health-related PHI in a document (PDF, DOC, DOCX, XLS, XLSX, PPT, PPTX, HTML, EML, MSG, PNG, JPG, WEBP) using Advanced AI. Rasterizes document pages, detects PII regions using a row-overlay approach, redacts those regions, and returns a rasterized PDF.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Cloudmersive.APIClient.NET.DLP.Api;
using Cloudmersive.APIClient.NET.DLP.Client;
using Cloudmersive.APIClient.NET.DLP.Model;

namespace Example
{
    public class RedactDocumentAdvancedExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "http://localhost";
            // Configure API key authorization: Apikey
            config.AddApiKey("Apikey", "YOUR_API_KEY");
            // Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
            // config.AddApiKeyPrefix("Apikey", "Bearer");

            var apiInstance = new RedactApi(config);
            var body = new DlpAdvancedDocumentRedactionRequest(); // DlpAdvancedDocumentRedactionRequest | Input request (optional) 

            try
            {
                // Redact User Data in Document (Advanced)
                DlpAdvancedDocumentRedactionResponse result = apiInstance.RedactDocumentAdvanced(body);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling RedactApi.RedactDocumentAdvanced: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the RedactDocumentAdvancedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Redact User Data in Document (Advanced)
    ApiResponse<DlpAdvancedDocumentRedactionResponse> response = apiInstance.RedactDocumentAdvancedWithHttpInfo(body);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling RedactApi.RedactDocumentAdvancedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **body** | [**DlpAdvancedDocumentRedactionRequest**](DlpAdvancedDocumentRedactionRequest.md) | Input request | [optional]  |

### Return type

[**DlpAdvancedDocumentRedactionResponse**](DlpAdvancedDocumentRedactionResponse.md)

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

<a id="redacttext"></a>
# **RedactText**
> DlpRedactionResponse RedactText (DlpRedactionRequest body = null)

Redact User Data in Input Text

Detects and redacts configurable types of user data in an input text string using Advanced AI. First detects PII, then redacts disallowed types by either deleting them or replacing them with asterisks.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Cloudmersive.APIClient.NET.DLP.Api;
using Cloudmersive.APIClient.NET.DLP.Client;
using Cloudmersive.APIClient.NET.DLP.Model;

namespace Example
{
    public class RedactTextExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "http://localhost";
            // Configure API key authorization: Apikey
            config.AddApiKey("Apikey", "YOUR_API_KEY");
            // Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
            // config.AddApiKeyPrefix("Apikey", "Bearer");

            var apiInstance = new RedactApi(config);
            var body = new DlpRedactionRequest(); // DlpRedactionRequest | Input request (optional) 

            try
            {
                // Redact User Data in Input Text
                DlpRedactionResponse result = apiInstance.RedactText(body);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling RedactApi.RedactText: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the RedactTextWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Redact User Data in Input Text
    ApiResponse<DlpRedactionResponse> response = apiInstance.RedactTextWithHttpInfo(body);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling RedactApi.RedactTextWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **body** | [**DlpRedactionRequest**](DlpRedactionRequest.md) | Input request | [optional]  |

### Return type

[**DlpRedactionResponse**](DlpRedactionResponse.md)

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

<a id="redacttextadvanced"></a>
# **RedactTextAdvanced**
> DlpAdvancedRedactionResponse RedactTextAdvanced (DlpAdvancedRedactionRequest body = null)

Redact User Data in Input Text (Advanced)

Detects and redacts 34 configurable types of user data including health-related PHI in an input text string using Advanced AI. First detects PII, then redacts disallowed types by either deleting them or replacing them with asterisks.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Cloudmersive.APIClient.NET.DLP.Api;
using Cloudmersive.APIClient.NET.DLP.Client;
using Cloudmersive.APIClient.NET.DLP.Model;

namespace Example
{
    public class RedactTextAdvancedExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "http://localhost";
            // Configure API key authorization: Apikey
            config.AddApiKey("Apikey", "YOUR_API_KEY");
            // Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
            // config.AddApiKeyPrefix("Apikey", "Bearer");

            var apiInstance = new RedactApi(config);
            var body = new DlpAdvancedRedactionRequest(); // DlpAdvancedRedactionRequest | Input request (optional) 

            try
            {
                // Redact User Data in Input Text (Advanced)
                DlpAdvancedRedactionResponse result = apiInstance.RedactTextAdvanced(body);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling RedactApi.RedactTextAdvanced: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the RedactTextAdvancedWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Redact User Data in Input Text (Advanced)
    ApiResponse<DlpAdvancedRedactionResponse> response = apiInstance.RedactTextAdvancedWithHttpInfo(body);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling RedactApi.RedactTextAdvancedWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **body** | [**DlpAdvancedRedactionRequest**](DlpAdvancedRedactionRequest.md) | Input request | [optional]  |

### Return type

[**DlpAdvancedRedactionResponse**](DlpAdvancedRedactionResponse.md)

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

