---
external help file: Microsoft.Azure.Commands.TrafficManager.dll-Help.xml
online version:
schema: 2.0.0
---

# Remove-AzureRmTrafficManagerEndpoint

## SYNOPSIS
Removes an endpoint from Azure Traffic Manager.

## SYNTAX

### Fields
```
Remove-AzureRmTrafficManagerEndpoint -Name <String> -Type <String> -ProfileName <String>
 -ResourceGroupName <String> [-Force] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Object
```
Remove-AzureRmTrafficManagerEndpoint -TrafficManagerEndpoint <TrafficManagerEndpoint> [-Force] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
The **Remove-AzureRmTrafficManagerEndpoint** cmdlet removes an endpoint from Azure Traffic Manager.

This cmdlet commits each change to the Traffic Manager service.
To remove multiple endpoints from a local Traffic Manager profile object and commit changes in a single operation, use the **Remove-AzureRmTrafficManagerEndpointConfig** cmdlet.

You can use the pipeline operator to pass a **TrafficManagerEndpoint** object to this cmdlet or you can pass a **TrafficManagerEndpoint** object in the *TrafficManagerEndpoint* parameter.
Alternatively, you can specify the endpoint by using the *Name* and *Type* parameters together with the *ProfileName* and *ResourceGroupName* parameters.

## EXAMPLES

### Example 1: Remove an Azure endpoint from a profile
```
PS C:\> Remove-AzureRmTrafficManagerEndpoint -Name "contoso" -ProfileName "ContosoProfile" -ResourceGroupName "ResourceGroup11" -Type AzureEndpoints
```

This command removes the Azure endpoint named "contoso" from the profile named "ContosoProfile" in the resource group named "ResourceGroup11".

## PARAMETERS

### -Force
Indicates whether to forcefully remove the endpoint.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Name
Specifies the name of the endpoint to remove.

```yaml
Type: String
Parameter Sets: Fields
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ProfileName
Specifies the name of a Traffic Manager profile from which this cmdlet removes the endpoint.

```yaml
Type: String
Parameter Sets: Fields
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ResourceGroupName
Specifies the name of the resource group that contains the profile.

```yaml
Type: String
Parameter Sets: Fields
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TrafficManagerEndpoint
Specifies a **TrafficManagerEndpoint** object that contains details about the endpoint to remove.

```yaml
Type: TrafficManagerEndpoint
Parameter Sets: Object
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Type
Specifies the type of endpoint that this cmdlet removes from the Traffic Manager profile.
Valid values are:

- AzureEndpoints
- ExternalEndpoints
- NestedEndpoints


```yaml
Type: String
Parameter Sets: Fields
Aliases:
Accepted values: AzureEndpoints, ExternalEndpoints, NestedEndpoints

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Confirm
Indicates whether to prompt the user for confirmation before running the cmdlet.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: cf

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WhatIf
Indicates whether to show what would happen if the cmdlet runs without actually running the cmdlet.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: wi

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Microsoft.Azure.Commands.TrafficManager.Models.TrafficManagerEndpoint

## OUTPUTS

### System.Boolean

## NOTES

## RELATED LINKS

[Get-AzureRmTrafficManagerEndpoint](./Get-AzureRmTrafficManagerEndpoint.md)

[Get-AzureRmTrafficManagerProfile](./Get-AzureRmTrafficManagerProfile.md)

[New-AzureRmTrafficManagerEndpoint](./New-AzureRmTrafficManagerEndpoint.md)

[Remove-AzureRmTrafficManagerEndpointConfig](./Remove-AzureRmTrafficManagerEndpointConfig.md)

[Set-AzureRmTrafficManagerProfile](./Set-AzureRmTrafficManagerProfile.md)
