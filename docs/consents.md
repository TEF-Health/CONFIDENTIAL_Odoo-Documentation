# Consent (draft)

## Consent checkboxes

>By checking the boxes below, I consent to the processing of my personal data as described in the Data Protection Information, which I have read and understood, for the following purposes:
>
>
>  [ ]  TEF-Health Platform access   
>  [ ]  Communication about TEF-Health"   
 
In addition (marketing, unrelated to GDPR)
 
>[ ] By checking this box, I consent to receive marketing emails about TEF-Health, including promotional offers, newsletters, and related information. I understand that I can withdraw this consent at any time.



# Processing Needs

(a) record (archive) these specific individual choices and 
(b) only send emails newsletters when consent was given
(c) allow that consent is revoked as easily as it was given.

(When no consent was given to the first checkbox, platform access, then the registration doesn't even continue.)

For (a): for archival, after each user registration, either a dedicated small file is created or a new row is added to an Excel file, either on S-drive or Sharepoint.

For (b) we need to write out these choices from Keycloak into a place where they can later be read by Odoo.

For (c) we need a page in the Keycloak User Management dashboard that each user sees where the check can be removed.

We would add an attribute to Keycloak User Roles, e.g. "marketing_consent". 

Then, via the existing Odoo-Keycloak user federation, we define an attribute mapping that maps Keycloak's "marketing_consent" to a corresponding field in Odoo that is then read out before sending emails.

If the consent for platform access is unchecked, the user gets a warning, and after they approve, the account is closed.

Importantly, every time a consent is given or removed this is tracked in the archive on Sharepoint/S-drive with a timestamp. We would still keep the user's names and emails even if they remove consent for platform -- as we need this information to track consenting, but we need to inform the user that the legal basis of the processing changed.

> Your decision to withdraw consent for processing your name and email for platform access has been recorded. To comply with GDPR, we will continue to store your name and email address under the legal basis of GDPR Art. 6(1)(c), which allows us to process personal data as necessary to comply with a legal obligation. This ensures we can maintain accurate records and comply with any legal requirements."