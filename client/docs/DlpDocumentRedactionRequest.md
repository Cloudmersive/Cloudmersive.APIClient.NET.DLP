# Cloudmersive.APIClient.NET.DLP.Model.DlpDocumentRedactionRequest
Request object for DLP document redaction with 23 PII detection types.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**InputFile** | **byte[]** | Document file bytes (PDF, DOCX, PNG, or JPG) to scan for PII and redact. | [optional] 
**FileName** | **string** | Optional. Name of the input file including extension, used for format detection. If not provided, format is detected from file contents. | [optional] 
**RecognitionMode** | **string** | Optional. Recognition mode for image processing. Options: null (default), \&quot;Fast\&quot;, \&quot;FastPlus\&quot;, \&quot;FastMini\&quot;. | [optional] 
**RedactionMode** | **string** | Redaction mode for PII regions. Options: \&quot;BlackOut\&quot; (default) draws black rectangles over PII rows, \&quot;Blur\&quot; applies Gaussian blur to PII rows, \&quot;BlackOutEntirePage\&quot; blacks out entire dirty pages, \&quot;BlurEntirePage\&quot; blurs entire dirty pages. | [optional] 
**AllowEmailAddress** | **bool** | Set to true to allow email addresses in the document and not redact them. | [optional] 
**AllowPhoneNumber** | **bool** | Set to true to allow phone numbers in the document and not redact them. | [optional] 
**AllowStreetAddress** | **bool** | Set to true to allow street addresses in the document and not redact them. | [optional] 
**AllowPersonName** | **bool** | Set to true to allow person names in the document and not redact them. | [optional] 
**AllowBirthDate** | **bool** | Set to true to allow birth dates in the document and not redact them. | [optional] 
**AllowPassportNumber** | **bool** | Set to true to allow passport numbers in the document and not redact them. | [optional] 
**AllowDriversLicense** | **bool** | Set to true to allow drivers license numbers in the document and not redact them. | [optional] 
**AllowSocialSecurityNumber** | **bool** | Set to true to allow social security numbers in the document and not redact them. | [optional] 
**AllowTaxpayerID** | **bool** | Set to true to allow taxpayer IDs in the document and not redact them. | [optional] 
**AllowCreditCardNumber** | **bool** | Set to true to allow credit card numbers in the document and not redact them. | [optional] 
**AllowCreditCardExpirationDate** | **bool** | Set to true to allow credit card expiration dates in the document and not redact them. | [optional] 
**AllowCreditCardVerificationCode** | **bool** | Set to true to allow credit card verification codes in the document and not redact them. | [optional] 
**AllowBankAccountNumber** | **bool** | Set to true to allow bank account numbers in the document and not redact them. | [optional] 
**AllowIBAN** | **bool** | Set to true to allow IBANs in the document and not redact them. | [optional] 
**AllowHealthInsuranceNumber** | **bool** | Set to true to allow health insurance numbers in the document and not redact them. | [optional] 
**AllowBearerToken** | **bool** | Set to true to allow bearer tokens in the document and not redact them. | [optional] 
**AllowHttpCookie** | **bool** | Set to true to allow HTTP cookies in the document and not redact them. | [optional] 
**AllowPrivateKeys** | **bool** | Set to true to allow private keys in the document and not redact them. | [optional] 
**AllowCredentials** | **bool** | Set to true to allow credentials (usernames/passwords) in the document and not redact them. | [optional] 
**AllowDeepWebUrls** | **bool** | Set to true to allow deep web URLs (.onion) in the document and not redact them. | [optional] 
**AllowSourceCode** | **bool** | Set to true to allow source code in the document and not redact it. | [optional] 
**AllowIpAddress** | **bool** | Set to true to allow IP addresses in the document and not redact them. | [optional] 
**AllowMacAddress** | **bool** | Set to true to allow MAC addresses in the document and not redact them. | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

