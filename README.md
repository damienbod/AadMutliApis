# AAD Multi tenant API

[![.NET](https://github.com/damienbod/AadMutliApis/actions/workflows/dotnet.yml/badge.svg)](https://github.com/damienbod/AadMutliApis/actions/workflows/dotnet.yml)

## Create the service principal for the API in your tenant

```powershell
Connect-AzureAD -TenantId '<UI-tenantId>'                                            

New-AzureADServicePrincipal -AppId 'AppId-from-multi-tenant-api'
```

## Give Consent in your tenant to the Enterprise applications

1. Open the Enterprise Applications blade
2. Find your enterprise application using the guid ObjectId from the powershell script
3. Open the permissions blade
4. Grant Admin consent

## Azure AD Permissions API

Permissions used in the AAD API

- none

## Azure AD Permissions UI 

- User.Read

## Links

https://damienbod.com/2023/01/02/azure-ad-multi-tenant-azure-app-registration-consent/

https://stackoverflow.com/questions/60929155/how-to-create-service-principal-of-multi-tenant-application