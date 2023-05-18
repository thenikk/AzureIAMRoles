## Azure IAM role definition

This repo contains one .json file for each built-in role within Azure IAM. Currently covering:
* **Entra Azure AD roles** 
* **Intune roles**
* **Cloud PC roles** (found in Intune)

The files in the folders contain corresponding infos of the role:
* Description
* Display name
* Role permissions, which are the effective paths of allowedResourceActions.

# Key features
* View effective permissions of built-in AAD roles
* Track changes and the history of the roles
* Compare roles by their rolePermissions

## Schedule
This repository is automatically filled by an Azure DevOps pipeline. A schedule performs an upload (if changes were made) on a daily basis.

## Graph API
All the data is grabbed by Graph API calls to a Microsoft tenant.

### Unsupported IAM role types
Not all role types are covered, currently missing:
* Exchange
* Entitlement Management
* Enterprise Apps

### Creators
[@NiklasTinner](https://twitter.com/NiklasTinner)
[@jannik_reinhard](https://twitter.com/jannik_reinhard)



