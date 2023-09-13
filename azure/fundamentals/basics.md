####Om

#### Account
- Heirarchy (Top Down)
  - Management Groups
  - Subscriptions
    - Can define quotas
  - Resource Groups
  - Resources ( Instances like VMs, Databases)

#### Management Groups
- Max 10000 Management groups in a single directory
- Max 6 levels of depth
- Only one parent and many children
- Within a single heirarchy in each directory
- 
#### Subscriptions
- 2 Types
  - Billing Boundary
  - Access Control Boundary
- All subscriptions under the same Management group must trust the same Azure AD Tenant
- Only one parent
- Within a single heirarchy in each directory

#### Resource Groups
- Logical grouping of resources
- All resources must be in RG
- Resource can only be in single RG
- Cant be nested
- Deleting RG deletes all resources
- Apply RBAC permissions to ease administration

#### Billing Arrangement
- Heirarchy ( Top to Bottom)
  - Blling Account
  - Billing Profile
    - Can set payment methods
  - Invoice section
  - Subscriptions

#### Notes
- Azure Resource Manager - ARM
  - Deployment and Management service for Azure
  - CRUD on Resources
  - Access control, locks , tags
- Region Pairs
  - Services  automatically come up at the paired region when region goes down
