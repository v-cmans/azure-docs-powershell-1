---
external help file: Microsoft.Azure.Commands.Resources.dll-Help.xml
ms.assetid: 52C5CD8B-2489-4FE6-9F33-B3350531CD8E
online version:
schema: 2.0.0
content_git_url: https://github.com/Azure/azure-powershell/blob/preview/src/ResourceManager/Resources/Commands.Resources/help/Get-AzureRmADGroupMember.md
original_content_git_url: https://github.com/Azure/azure-powershell/blob/preview/src/ResourceManager/Resources/Commands.Resources/help/Get-AzureRmADGroupMember.md
gitcommit: https://github.com/Azure/azure-powershell/blob/39673ed92d863c7fba7fbbdb0d919d03c552b71b
---

# Get-AzureRmADGroupMember

## SYNOPSIS
Get a group members.

## SYNTAX

```
Get-AzureRmADGroupMember [-GroupObjectId <Guid>] [<CommonParameters>]
```

## DESCRIPTION
Get a group members.

## EXAMPLES

### --------------------------  Filters group members using group object id  --------------------------
```
PS C:\> Get-AzureRmADGroupMember -GroupObjectId 85F89C90-780E-4AA6-9F4F-6F268D322EEE
```

Gets group members with 85F89C90-780E-4AA6-9F4F-6F268D322EEE id

## PARAMETERS

### -GroupObjectId
Object id of the group.

```yaml
Type: Guid
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Get-AzureRmADUser]()

[Get-AzureRmADServicePrincipal]()

[Get-AzureRmADGroupMemberMember]()

