# Cloudmersive.APIClient.NET.DLP.Model.DlpBatchJobStatusResult
Result of performing a DLP batch job operation

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Successful** | **bool** | True if the operation to check the status of the job was successful, false otherwise | [optional] 
**AsyncJobStatus** | **string** | Returns the job status of the Async Job, if applicable.  Possible states are STARTED and COMPLETED | [optional] 
**AsyncJobID** | **string** | Job ID | [optional] 
**DetectAudioResult** | [**DlpAudioDetectionResponse**](DlpAudioDetectionResponse.md) |  | [optional] 
**DetectAudioAdvancedResult** | [**DlpAdvancedAudioDetectionResponse**](DlpAdvancedAudioDetectionResponse.md) |  | [optional] 
**RedactAudioResult** | [**DlpAudioRedactionResponse**](DlpAudioRedactionResponse.md) |  | [optional] 
**RedactAudioAdvancedResult** | [**DlpAdvancedAudioRedactionResponse**](DlpAdvancedAudioRedactionResponse.md) |  | [optional] 
**ErrorMessage** | **string** | Error message (if any) | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

