# Cloudmersive.APIClient.NET.DLP.Model.DlpAdvancedRedactionRequest
Request object for advanced DLP text redaction with 34 PII detection types including health-related data and configurable redaction mode.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**InputText** | **string** | Text to scan for PII and redact sensitive data from. | [optional] 
**AllowEmailAddress** | **bool** | Set to true to allow email addresses in the input text and not redact them. | [optional] 
**AllowPhoneNumber** | **bool** | Set to true to allow phone numbers in the input text and not redact them. | [optional] 
**AllowStreetAddress** | **bool** | Set to true to allow street addresses in the input text and not redact them. | [optional] 
**AllowPersonName** | **bool** | Set to true to allow person names in the input text and not redact them. | [optional] 
**AllowBirthDate** | **bool** | Set to true to allow birth dates in the input text and not redact them. | [optional] 
**AllowPassportNumber** | **bool** | Set to true to allow passport numbers in the input text and not redact them. | [optional] 
**AllowDriversLicense** | **bool** | Set to true to allow drivers license numbers in the input text and not redact them. | [optional] 
**AllowSocialSecurityNumber** | **bool** | Set to true to allow social security numbers in the input text and not redact them. | [optional] 
**AllowTaxpayerID** | **bool** | Set to true to allow taxpayer IDs in the input text and not redact them. | [optional] 
**AllowCreditCardNumber** | **bool** | Set to true to allow credit card numbers in the input text and not redact them. | [optional] 
**AllowCreditCardExpirationDate** | **bool** | Set to true to allow credit card expiration dates in the input text and not redact them. | [optional] 
**AllowCreditCardVerificationCode** | **bool** | Set to true to allow credit card verification codes in the input text and not redact them. | [optional] 
**AllowBankAccountNumber** | **bool** | Set to true to allow bank account numbers in the input text and not redact them. | [optional] 
**AllowIBAN** | **bool** | Set to true to allow IBANs in the input text and not redact them. | [optional] 
**AllowHealthInsuranceNumber** | **bool** | Set to true to allow health insurance numbers in the input text and not redact them. | [optional] 
**AllowBearerToken** | **bool** | Set to true to allow bearer tokens in the input text and not redact them. | [optional] 
**AllowHttpCookie** | **bool** | Set to true to allow HTTP cookies in the input text and not redact them. | [optional] 
**AllowPrivateKeys** | **bool** | Set to true to allow private keys in the input text and not redact them. | [optional] 
**AllowCredentials** | **bool** | Set to true to allow credentials (usernames/passwords) in the input text and not redact them. | [optional] 
**AllowDeepWebUrls** | **bool** | Set to true to allow deep web URLs (.onion) in the input text and not redact them. | [optional] 
**AllowSourceCode** | **bool** | Set to true to allow source code in the input text and not redact it. | [optional] 
**AllowIpAddress** | **bool** | Set to true to allow IP addresses in the input text and not redact them. | [optional] 
**AllowMacAddress** | **bool** | Set to true to allow MAC addresses in the input text and not redact them. | [optional] 
**AllowHealthInsuranceMemberID** | **bool** | Set to true to allow health insurance member IDs in the input text and not redact them. | [optional] 
**AllowHealthInjuryOrDisease** | **bool** | Set to true to allow references to injuries or diseases in the input text and not redact them. | [optional] 
**AllowHealthTypeOfTreatment** | **bool** | Set to true to allow references to types of medical treatment in the input text and not redact them. | [optional] 
**AllowHealthDateAndTimeOfTreatment** | **bool** | Set to true to allow dates and times of medical treatment in the input text and not redact them. | [optional] 
**AllowHealthPlanBeneficiaryNumber** | **bool** | Set to true to allow health plan beneficiary numbers in the input text and not redact them. | [optional] 
**AllowHealthPaymentsMadeForTreatment** | **bool** | Set to true to allow payments made for medical treatment in the input text and not redact them. | [optional] 
**AllowVehicleID** | **bool** | Set to true to allow vehicle identifiers (e.g. license plates, VINs) in the input text and not redact them. | [optional] 
**AllowDeviceID** | **bool** | Set to true to allow device identifiers (e.g. serial numbers, IMEIs, MAC-level device IDs) in the input text and not redact them. | [optional] 
**AllowNamesOfRelatives** | **bool** | Set to true to allow names of relatives in the input text and not redact them. | [optional] 
**AllowHealthUniversalRecordLocator** | **bool** | Set to true to allow health universal record locators (URLs) in the input text and not redact them. | [optional] 
**AllowBiometrics** | **bool** | Set to true to allow biometric data references (e.g. fingerprints, retinal scans, voiceprints) in the input text and not redact them. | [optional] 
**RedactionMode** | **string** | Redaction mode: \&quot;Delete\&quot; to remove PII entirely, or \&quot;ReplaceWithAsterisk\&quot; to replace PII characters with asterisks (*). | [optional] 
**ProvideAnalysisRationale** | **bool** | Set to true to include a natural language rationale explaining why each detection conclusion was formed. | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

