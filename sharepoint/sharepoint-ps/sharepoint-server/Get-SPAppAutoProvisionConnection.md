---
external help file: 
applicable: SharePoint Server 2013, SharePoint Server 2016
schema: 2.0.0
---

# Get-SPAppAutoProvisionConnection

## SYNOPSIS

Returns provision connection settings for an app.



## SYNTAX

```
Get-SPAppAutoProvisionConnection [-AssignmentCollection <SPAssignmentCollection>]
 [-ConnectionType <ConnectionTypes>] [-SiteSubscription <SPSiteSubscriptionPipeBind>] [<CommonParameters>]
```

## DESCRIPTION
Use the Get-SPAppAutoProvisionConnection cmdlet to return the provision connection settings for an app.

For permissions and the most current information about Windows PowerShell for SharePoint Products, see the online documentation at http://go.microsoft.com/fwlink/p/?LinkId=251831 (http://go.microsoft.com/fwlink/p/?LinkId=251831).

## EXAMPLES

### ---------------EXAMPLE 1---------- 
```
C:\PS>Get-SpAppAutoProvisionConnection
```

This example returns the entire app auto provisioning connection information for the default site subscription.

### ---------------EXAMPLE 2---------- 
```
C:\PS>$subscription = Get-SPSiteSubscription http://Contoso.com

C:\PS>Get-SPAppAutoProvisionConnection -SiteSubscription $subscription -ConnectionType RemoteWebHost
```

This example returns the remote web host app auto provisioning connection information for the site subscription for Contoso.com site

## PARAMETERS

### -AssignmentCollection
Manages objects for the purpose of proper disposal.
Use of objects, such as SPWeb or SPSite, can use large amounts of memory and use of these objects in Windows PowerShell scripts requires proper memory management.
Using the SPAssignment object, you can assign objects to a variable and dispose of the objects after they are needed to free up memory.
When SPWeb, SPSite, or SPSiteAdministration objects are used, the objects are automatically disposed of if an assignment collection or the Global parameter is not used.

When the Global parameter is used, all objects are contained in the global store.
If objects are not immediately used, or disposed of by using the Stop-SPAssignment command, an out-of-memory scenario can occur.

```yaml
Type: SPAssignmentCollection
Parameter Sets: (All)
Aliases: 
Applicable: SharePoint Server 2013, SharePoint Server 2016

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -ConnectionType
Specifies the connection type to provision the app.

```yaml
Type: ConnectionTypes
Parameter Sets: (All)
Aliases: 
Applicable: SharePoint Server 2013, SharePoint Server 2016

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SiteSubscription
Specifies the site collection from which to return the provision connection.

```yaml
Type: SPSiteSubscriptionPipeBind
Parameter Sets: (All)
Aliases: 
Applicable: SharePoint Server 2013, SharePoint Server 2016

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Set-SPAppAutoProvisionConnection]()
