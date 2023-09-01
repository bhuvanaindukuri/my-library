#### Terms
- Directory - Heirarchichal Structure that stores information about objects on the network
- Directory Service
  - Provides methods for storing directory data and making it available to network users and administrators
- Active Directory
  - Directory service
  - Implements LDAP

#### Heirarchy
  - Domain
    - Containers (Ex: Computers, Users)
      - Object
        - Attributes
  - Can be grouped to OUs
  - OU can have other OUs
  - Administration can be delegated at OU level
  - Link group policy Objects to OUs

#### Security groups
- Created as objects
- Can add people
- Can assign Password settings
 
#### AD Services
- Active Directory Domain Service ( ADDS )
  - Implements core functionalities of Directory Service 
- Active Directory Certificate Services ( ADCS )
  - Allows provisioning of PKI certificates
  - Trusted on the network
-  Active Directory Federation Services ( ADFS )
  - Single Sing-on
- Active Directory Rights Management Services ( AD RMS )
  - Manage permissions to files
  - Not in active development

#### ADFS
- Access resources across networks
- Allow external user access
- Publish internal apps to internet using Web Application Proxy (WAP)
- Can federate with Azure AD

#### Windows login methods
- Password based
  - Password stored as cryptographic hash
  - Symmetric key for encryption & decryption
- Smartcard based
  - Asymmetric key
  - private key used for decryption is stored in the smartcard
  - public key stored in the identity provider
- Biometric

#### Windows Hello for Business
- Pin or biometric is only stored on the device and not in the central repo
- Deployment models
  - On-Prem - ADFS MFA
  - Cloud only Register - Azure MFA
  - Hybrid Register - Azure MFA
- Trust models
  - Key Trust
  - Certificate Trust
  - Cloud Kerberos Trust
    - For Hybrid deployments
    - Azure based
    - AAD can provide kerberos ticket for hybrid
    - Dont need to sync
   
#### Single Sign-on
- Seamless SSO
- Azure AD SSO (Device Registration)
  - credentials stored only in device
  - device registers with identity provider
  - ADFS used for on-prem only deployments
  - Azure AD used for cloud-only and hybrid

#### Device Registration (Azure AD SSO)
- Azure AD Registered
  - BYOD
  - Object created only in AAD
  - Not for on-premises
- Azure AD joined
  - Joined to Azure AD
  - AAD Connect should sync cloud devices to AD for being able to access on-prem resources
- Hybrid AD joined
  - Joined to AD
  - Device identity synced to Azure

