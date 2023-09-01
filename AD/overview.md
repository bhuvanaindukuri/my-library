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
