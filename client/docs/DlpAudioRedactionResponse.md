# Cloudmersive.APIClient.NET.DLP.Model.DlpAudioRedactionResponse
Response object for DLP audio redaction with 23 PII detection results, redacted audio, and redacted transcript.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**RedactedAudio** | **byte[]** | The redacted audio file bytes with PII segments bleeped or muted, or the original audio if no disallowed PII was found. | [optional] 
**RedactedTranscript** | **string** | The redacted transcript text with PII removed or replaced. | [optional] 
**OriginalTranscript** | **string** | Full original transcript of the audio file. | [optional] 
**Timestamps** | [**List&lt;AudioTimestamp&gt;**](AudioTimestamp.md) | Token-level timestamps from speech recognition. | [optional] 
**RedactedSegments** | [**List&lt;RedactedAudioSegment&gt;**](RedactedAudioSegment.md) | List of audio segments that were redacted, with their time ranges. | [optional] 
**CleanResult** | **bool** | True if no disallowed PII or sensitive data types were detected; false if any disallowed type was found and redacted. | [optional] 
**ContainsEmailAddress** | **bool** | True if the audio transcript contains email addresses. | [optional] 
**ContainsPhoneNumber** | **bool** | True if the audio transcript contains phone numbers. | [optional] 
**ContainsStreetAddress** | **bool** | True if the audio transcript contains street addresses. | [optional] 
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

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

