---
applicable: SharePoint Online
external help file: PnP.PowerShell.dll-Help.xml
Module Name: PnP.PowerShell
online version: https://pnp.github.io/powershell/cmdlets/remove-pnpdeletedmicrosoft365group
schema: 2.0.0
title: Remove-PnPDeletedMicrosoft365Group
---

# Remove-PnPDeletedMicrosoft365Group

## SYNOPSIS

**Required Permissions**

  * Microsoft Graph API: Group.ReadWrite.All

Permanently removes one deleted Microsoft 365 Group

## SYNTAX

```powershell
Remove-PnPDeletedMicrosoft365Group -Identity <Microsoft365GroupPipeBind> 
 [<CommonParameters>]
```

## DESCRIPTION

## EXAMPLES

### EXAMPLE 1
```powershell
Remove-PnPDeletedMicrosoft365Group -Identity 38b32e13-e900-4d95-b860-fb52bc07ca7f
```

Permanently removes a deleted Microsoft 365 Group based on its ID

### EXAMPLE 2
```powershell
$group = Get-PnPDeletedMicrosoft365Group -Identity 38b32e13-e900-4d95-b860-fb52bc07ca7f
Remove-PnPDeletedMicrosoft365Group -Identity $group
```

Permanently removes the provided deleted Microsoft 365 Group

## PARAMETERS

### -Identity
The identity of the deleted Microsoft 365 Group to be deleted

```yaml
Type: Microsoft365GroupPipeBind
Parameter Sets: (All)

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

## RELATED LINKS

[Microsoft 365 Patterns and Practices](https://aka.ms/m365pnp)