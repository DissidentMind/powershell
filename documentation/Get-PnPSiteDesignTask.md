---
applicable: SharePoint Online
external help file: PnP.PowerShell.dll-Help.xml
Module Name: PnP.PowerShell
online version: https://docs.microsoft.com/powershell/module/sharepoint-pnp/get-pnpsitedesigntask
schema: 2.0.0
title: Get-PnPSiteDesignTask
---

# Get-PnPSiteDesignTask

## SYNOPSIS
Used to retrieve a scheduled site design script. It takes the ID of the scheduled site design task and the URL for the site where the site design is scheduled to be applied.

## SYNTAX

```
Get-PnPSiteDesignTask [-Identity <TenantSiteDesignTaskPipeBind>] [-WebUrl <String>] [-Web <WebPipeBind>]
 [-Connection <PnPConnection>] [<CommonParameters>]
```

## DESCRIPTION

## EXAMPLES

### EXAMPLE 1
```powershell
Get-PnPSiteDesignTask -Identity 501z8c32-4147-44d4-8607-26c2f67cae82
```

This example retrieves a site design task given the provided site design task id

### EXAMPLE 2
```powershell
Get-PnPSiteDesignTask
```

This example retrieves all site design tasks currently scheduled on the current site

### EXAMPLE 3
```powershell
Get-PnPSiteDesignTask -WebUrl "https://contoso.sharepoint.com/sites/project"
```

This example retrieves all site design tasks currently scheduled on the provided site

## PARAMETERS

### -Connection
Optional connection to be used by the cmdlet. Retrieve the value for this parameter by either specifying -ReturnConnection on Connect-PnPOnline or by executing Get-PnPConnection.

```yaml
Type: PnPConnection
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Identity
The ID of the site design task to retrieve.

```yaml
Type: TenantSiteDesignTaskPipeBind
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Web
This parameter allows you to optionally apply the cmdlet action to a subweb within the current web. In most situations this parameter is not required and you can connect to the subweb using Connect-PnPOnline instead. Specify the GUID, server relative url (i.e. /sites/team1) or web instance of the web to apply the command to. Omit this parameter to use the current web.

```yaml
Type: WebPipeBind
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WebUrl
The URL of the site collection where the site design will be applied. If not specified the site design tasks will be returned for the site you connected to with Connect-PnPOnline.

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

## RELATED LINKS

[SharePoint Developer Patterns and Practices](https://aka.ms/sppnp)