# Cloudmersive.APIClient.NET.DLP.Model.DlpAdvancedAudioDetectionResponse
Response object for advanced DLP audio detection with 34 PII detection types, transcript, timestamps, and optional rationale.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**CleanResult** | **bool** | True if no disallowed PII or sensitive data types were detected; false if any disallowed type was found. | [optional] 
**Transcript** | **string** | Full transcript of the audio file. | [optional] 
**Timestamps** | [**List&lt;AudioTimestamp&gt;**](AudioTimestamp.md) | Token-level timestamps from speech recognition. | [optional] 
**ContainsEmailAddress** | **bool** | True if the audio transcript contains email addresses. | [optional] 
**ContainsPhoneNumber** | **bool** | True if the audio transcript contains phone numbers. | [optional] 
**ContainsStreetAddress** | **bool** | True if the audio transcript contains street addresses. | [optional] 
**ContainsCity** | **bool** | True if the audio transcript contains standalone city names (e.g. \&quot;San Francisco\&quot;) outside of a full street address. | [optional] 
**ContainsPersonName** | **bool** | True if the audio transcript contains person names. | [optional] 
**ContainsBirthDate** | **bool** | True if the audio transcript contains birth dates. | [optional] 
**ContainsPassportNumber** | **bool** | True if the audio transcript contains passport numbers. | [optional] 
**ContainsDriversLicense** | **bool** | True if the audio transcript contains drivers license numbers. | [optional] 
**ContainsSocialSecurityNumber** | **bool** | True if the audio transcript contains social security numbers. | [optional] 
**ContainsTaxpayerID** | **bool** | True if the audio transcript contains taxpayer IDs. | [optional] 
**ContainsCreditCardNumber** | **bool** | True if the audio transcript contains credit card numbers. | [optional] 
**ContainsCreditCardExpirationDate** | **bool** | True if the audio transcript contains credit card expiration dates. | [optional] 
**ContainsCreditCardVerificationCode** | **bool** | True if the audio transcript contains credit card verification codes. | [optional] 
**ContainsBankAccountNumber** | **bool** | True if the audio transcript contains bank account numbers. | [optional] 
**ContainsIBAN** | **bool** | True if the audio transcript contains IBANs. | [optional] 
**ContainsHealthInsuranceNumber** | **bool** | True if the audio transcript contains health insurance numbers. | [optional] 
**ContainsBearerToken** | **bool** | True if the audio transcript contains bearer tokens. | [optional] 
**ContainsHttpCookie** | **bool** | True if the audio transcript contains HTTP cookies. | [optional] 
**ContainsPrivateKeys** | **bool** | True if the audio transcript contains private keys. | [optional] 
**ContainsCredentials** | **bool** | True if the audio transcript contains credentials (usernames/passwords). | [optional] 
**ContainsDeepWebUrls** | **bool** | True if the audio transcript contains deep web URLs (.onion). | [optional] 
**ContainsSourceCode** | **bool** | True if the audio transcript contains source code. | [optional] 
**ContainsIpAddress** | **bool** | True if the audio transcript contains IP addresses. | [optional] 
**ContainsMacAddress** | **bool** | True if the audio transcript contains MAC addresses. | [optional] 
**ContainsHealthInsuranceMemberID** | **bool** | True if the audio transcript contains health insurance member IDs. | [optional] 
**ContainsMedicalRecordNumber** | **bool** | True if the audio transcript contains medical record numbers. | [optional] 
**ContainsBillingAccountNumber** | **bool** | True if the audio transcript contains billing account numbers (provider/customer billing account IDs, distinct from bank account numbers). | [optional] 
**ContainsHealthInjuryOrDisease** | **bool** | True if the audio transcript contains references to injuries or diseases. | [optional] 
**ContainsHealthTypeOfTreatment** | **bool** | True if the audio transcript contains references to types of medical treatment. | [optional] 
**ContainsHealthDateAndTimeOfTreatment** | **bool** | True if the audio transcript contains dates and times of medical treatment. | [optional] 
**ContainsHealthPlanBeneficiaryNumber** | **bool** | True if the audio transcript contains health plan beneficiary numbers. | [optional] 
**ContainsHealthPaymentsMadeForTreatment** | **bool** | True if the audio transcript contains payments made for medical treatment. | [optional] 
**ContainsVehicleID** | **bool** | True if the audio transcript contains vehicle identifiers (e.g. license plates, VINs). | [optional] 
**ContainsDeviceID** | **bool** | True if the audio transcript contains device identifiers (e.g. serial numbers, IMEIs, MAC-level device IDs). | [optional] 
**ContainsNamesOfRelatives** | **bool** | True if the audio transcript contains names of relatives. | [optional] 
**ContainsHealthUniversalRecordLocator** | **bool** | True if the audio transcript contains health universal record locators (URLs). | [optional] 
**ContainsBiometrics** | **bool** | True if the audio transcript contains biometric data references (e.g. fingerprints, retinal scans, voiceprints). | [optional] 
**AnalysisRationale** | **string** | Rationale for why the conclusion was formed. Only populated when ProvideAnalysisRationale is set to true in the request. | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

