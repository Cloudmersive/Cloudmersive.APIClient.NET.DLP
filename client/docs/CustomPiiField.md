# Cloudmersive.APIClient.NET.DLP.Model.CustomPiiField
Caller-defined custom PII field. The redaction LLM will look for content matching  the description and redact it as a semantic tag derived from the title  (e.g. title \"internal participant code\" → tag [INTERNAL-PARTICIPANT-CODE]).

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Title** | **string** | Short title for the custom field, also used to derive the semantic tag (uppercased, spaces/underscores replaced with hyphens). | [optional] 
**Description** | **string** | Description of what this field looks like, used to instruct the redaction LLM. Be specific so the LLM can locate matches. | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

