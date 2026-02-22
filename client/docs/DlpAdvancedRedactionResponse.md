# Cloudmersive.APIClient.NET.DLP.Model.DlpAdvancedRedactionResponse
Response object for advanced DLP text redaction with 34 PII detection results, redacted text, and optional rationale.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**RedactedText** | **string** | The redacted text with PII removed or replaced, or the original text if no disallowed PII was found. | [optional] 
**CleanResult** | **bool** | True if no disallowed PII or sensitive data types were detected; false if any disallowed type was found and redacted. | [optional] 
**ContainsEmailAddress** | **bool** | True if the input contains email addresses. | [optional] 
**ContainsPhoneNumber** | **bool** | True if the input contains phone numbers. | [optional] 
**ContainsStreetAddress** | **bool** | True if the input contains street addresses. | [optional] 
**ContainsPersonName** | **bool** | True if the input contains person names. | [optional] 
**ContainsBirthDate** | **bool** | True if the input contains birth dates. | [optional] 
**ContainsPassportNumber** | **bool** | True if the input contains passport numbers. | [optional] 
**ContainsDriversLicense** | **bool** | True if the input contains drivers license numbers. | [optional] 
**ContainsSocialSecurityNumber** | **bool** | True if the input contains social security numbers. | [optional] 
**ContainsTaxpayerID** | **bool** | True if the input contains taxpayer IDs. | [optional] 
**ContainsCreditCardNumber** | **bool** | True if the input contains credit card numbers. | [optional] 
**ContainsCreditCardExpirationDate** | **bool** | True if the input contains credit card expiration dates. | [optional] 
**ContainsCreditCardVerificationCode** | **bool** | True if the input contains credit card verification codes. | [optional] 
**ContainsBankAccountNumber** | **bool** | True if the input contains bank account numbers. | [optional] 
**ContainsIBAN** | **bool** | True if the input contains IBANs. | [optional] 
**ContainsHealthInsuranceNumber** | **bool** | True if the input contains health insurance numbers. | [optional] 
**ContainsBearerToken** | **bool** | True if the input contains bearer tokens. | [optional] 
**ContainsHttpCookie** | **bool** | True if the input contains HTTP cookies. | [optional] 
**ContainsPrivateKeys** | **bool** | True if the input contains private keys. | [optional] 
**ContainsCredentials** | **bool** | True if the input contains credentials (usernames/passwords). | [optional] 
**ContainsDeepWebUrls** | **bool** | True if the input contains deep web URLs (.onion). | [optional] 
**ContainsSourceCode** | **bool** | True if the input contains source code. | [optional] 
**ContainsIpAddress** | **bool** | True if the input contains IP addresses. | [optional] 
**ContainsMacAddress** | **bool** | True if the input contains MAC addresses. | [optional] 
**ContainsHealthInsuranceMemberID** | **bool** | True if the input contains health insurance member IDs. | [optional] 
**ContainsHealthInjuryOrDisease** | **bool** | True if the input contains references to injuries or diseases. | [optional] 
**ContainsHealthTypeOfTreatment** | **bool** | True if the input contains references to types of medical treatment. | [optional] 
**ContainsHealthDateAndTimeOfTreatment** | **bool** | True if the input contains dates and times of medical treatment. | [optional] 
**ContainsHealthPlanBeneficiaryNumber** | **bool** | True if the input contains health plan beneficiary numbers. | [optional] 
**ContainsHealthPaymentsMadeForTreatment** | **bool** | True if the input contains payments made for medical treatment. | [optional] 
**ContainsVehicleID** | **bool** | True if the input contains vehicle identifiers (e.g. license plates, VINs). | [optional] 
**ContainsDeviceID** | **bool** | True if the input contains device identifiers (e.g. serial numbers, IMEIs, MAC-level device IDs). | [optional] 
**ContainsNamesOfRelatives** | **bool** | True if the input contains names of relatives. | [optional] 
**ContainsHealthUniversalRecordLocator** | **bool** | True if the input contains health universal record locators (URLs). | [optional] 
**ContainsBiometrics** | **bool** | True if the input contains biometric data references (e.g. fingerprints, retinal scans, voiceprints). | [optional] 
**AnalysisRationale** | **string** | Rationale for why the conclusion was formed. Only populated when ProvideAnalysisRationale is set to true in the request. | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

