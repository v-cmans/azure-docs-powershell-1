---
external help file: Microsoft.Azure.Commands.Management.Storage.dll-Help.xml
online version:
schema: 2.0.0
---

# New-AzureRmStorageAccountKey

## SYNOPSIS
Regenerates a storage key for an Azure storage Account.

## SYNTAX

```
New-AzureRmStorageAccountKey [-ResourceGroupName] <String> [-Name] <String> [-KeyName] <String>
 [-InformationAction <ActionPreference>] [-InformationVariable <String>] [<CommonParameters>]
```

## DESCRIPTION
The **New-AzureRmStorageAccountKey** cmdlet regenerates a storage key for an Azure storage account.

## EXAMPLES

### Example 1: Regenerate a storage key
```
PS C:\> New-AzureRmStorageKey -ResourceGroupName "myresourcegroup" -Name "mystorageaccount" -keyName "key1"
```

This command regenerates the "key1" storage key for the storage account named "mystorageaccount".

## PARAMETERS

### -InformationAction
Specifies how this cmdlet responds to an information event.

The acceptable values for this parameter are:

- Continue
- Ignore
- Inquire
- SilentlyContinue
- Stop
- Suspend

```yaml
Type: ActionPreference
Parameter Sets: (All)
Aliases: infa

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InformationVariable
Specifies a variable that is used for storing an informational message.

```yaml
Type: String
Parameter Sets: (All)
Aliases: iv

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -KeyName
Specifies which key to regenerate.
The valid values for this parameter are:
- key1
- key2

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: True
Position: 2
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Name
Specifies the name of the storage account for which to regenerate a storage key.

```yaml
Type: String
Parameter Sets: (All)
Aliases: StorageAccountName, AccountName

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ResourceGroupName
Specifies the name of the resource group that contains the storage account.

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### None

## OUTPUTS

### None

## NOTES

## RELATED LINKS

[Get-AzureRmStorageAccountKey](./Get-AzureRmStorageAccountKey.md)
