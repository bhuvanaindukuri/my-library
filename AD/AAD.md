### Intro
- on Azure
- Not directory Service implemented on servers
- Can manage users
- Can manage devices
- Hybrid Identity
  - Sync on-prem AD accounts to Azure
  - Can be done using Azure AD Connect
  - Single Sign-on
  - Ways
    - Password Hash
      - Hash of user password stored in AAD
    - Passthrough
      - Credentials not stored in AAD
    - Federation using ADFS
- External accounts ( Azure B2B )
  - identity stored in AAD
  - Credentials can be managed in external IDP
- Authentication types
  - Passwords
  - Multi-factor authentication
  - Password-less options

#### Azure AD Application Proxy
  - Expose internal application to internet
  - DMZ required

#### Conditional Access policies
  - Helps in providing authorization
  - Can be based on users'
    - Group Membership
    - IP Address
    - Region or Country
    - Guest user accounts
    - Device type
    - Device registration & compliance

#### Azure Active Directory Domain Services
- Domain Controller as a Service
- Helps with lift and shift of on-prem applications

#### Notes
- Windows authentication uses Kerberos protocol
    
