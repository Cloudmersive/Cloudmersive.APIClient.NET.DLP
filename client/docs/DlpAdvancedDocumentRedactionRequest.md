# Cloudmersive.APIClient.NET.DLP.Model.DlpAdvancedDocumentRedactionRequest
Request object for advanced DLP document redaction with 35 PII detection types including health-related data.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**InputFile** | **byte[]** | Document file bytes (PDF, DOC, DOCX, XLS, XLSX, PPT, PPTX, HTML, EML, MSG, PNG, JPG, or WEBP) to scan for PII and redact. | [optional] 
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
**AllowHealthInsuranceMemberID** | **bool** | Set to true to allow health insurance member IDs in the document and not redact them. | [optional] 
**AllowHealthInjuryOrDisease** | **bool** | Set to true to allow references to injuries or diseases in the document and not redact them. | [optional] 
**AllowHealthTypeOfTreatment** | **bool** | Set to true to allow references to types of medical treatment in the document and not redact them. | [optional] 
**AllowHealthDateAndTimeOfTreatment** | **bool** | Set to true to allow dates and times of medical treatment in the document and not redact them. | [optional] 
**AllowHealthPlanBeneficiaryNumber** | **bool** | Set to true to allow health plan beneficiary numbers in the document and not redact them. | [optional] 
**AllowHealthPaymentsMadeForTreatment** | **bool** | Set to true to allow payments made for medical treatment in the document and not redact them. | [optional] 
**AllowFaces** | **bool** | Set to true to allow identifiable human faces in the document and not redact them. | [optional] 
**AllowVehicleID** | **bool** | Set to true to allow vehicle identifiers (e.g. license plates, VINs) in the document and not redact them. | [optional] 
**AllowDeviceID** | **bool** | Set to true to allow device identifiers (e.g. serial numbers, IMEIs, MAC-level device IDs) in the document and not redact them. | [optional] 
**AllowNamesOfRelatives** | **bool** | Set to true to allow names of relatives in the document and not redact them. | [optional] 
**AllowHealthUniversalRecordLocator** | **bool** | Set to true to allow health universal record locators (URLs) in the document and not redact them. | [optional] 
**AllowBiometrics** | **bool** | Set to true to allow biometric data references (e.g. fingerprints, retinal scans, voiceprints) in the document and not redact them. | [optional] 
**ProvideAnalysisRationale** | **bool** | Set to true to include a natural language rationale explaining why each detection conclusion was formed. | [optional] 
**CustomPolicyID** | **string** | Apply a Custom Policy for DLP Enforcement by providing the ID; to create a Custom Policy,  navigate to the Cloudmersive Management Portal and select Custom Policies.  Requires Managed Instance or Private Cloud | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

