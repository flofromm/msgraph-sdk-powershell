---
external help file:
Module Name: Microsoft.Graph.Identity.SignIns
online version: https://docs.microsoft.com/en-us/powershell/module/microsoft.graph.identity.signins/confirm-mginformationprotectionsignature
schema: 2.0.0
---

# Confirm-MgInformationProtectionSignature

## SYNOPSIS
Invoke action verifySignature

## SYNTAX

### VerifyExpanded (Default)
```
Confirm-MgInformationProtectionSignature [-AdditionalProperties <Hashtable>] [-DigestInputFile <String>]
 [-SignatureInputFile <String>] [-SigningKeyId <String>] [-Confirm] [-WhatIf] [<CommonParameters>]
```

### Verify
```
Confirm-MgInformationProtectionSignature
 -BodyParameter <IPathsSit1AcInformationprotectionMicrosoftGraphVerifysignaturePostRequestbodyContentApplicationJsonSchema>
 [-Confirm] [-WhatIf] [<CommonParameters>]
```

## DESCRIPTION
Invoke action verifySignature

## EXAMPLES

## PARAMETERS

### -AdditionalProperties
Additional Parameters

```yaml
Type: System.Collections.Hashtable
Parameter Sets: VerifyExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BodyParameter
.
To construct, please use Get-Help -Online and see NOTES section for BODYPARAMETER properties and create a hash table.

```yaml
Type: Microsoft.Graph.PowerShell.Models.IPathsSit1AcInformationprotectionMicrosoftGraphVerifysignaturePostRequestbodyContentApplicationJsonSchema
Parameter Sets: Verify
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -DigestInputFile
Input File for Digest (.)

```yaml
Type: System.String
Parameter Sets: VerifyExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SignatureInputFile
Input File for Signature (.)

```yaml
Type: System.String
Parameter Sets: VerifyExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SigningKeyId
.

```yaml
Type: System.String
Parameter Sets: VerifyExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Confirm
Prompts you for confirmation before running the cmdlet.

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases: cf

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WhatIf
Shows what would happen if the cmdlet runs.
The cmdlet is not run.

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases: wi

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Microsoft.Graph.PowerShell.Models.IPathsSit1AcInformationprotectionMicrosoftGraphVerifysignaturePostRequestbodyContentApplicationJsonSchema

## OUTPUTS

### System.Boolean

## NOTES

ALIASES

COMPLEX PARAMETER PROPERTIES

To create the parameters described below, construct a hash table containing the appropriate properties. For information on hash tables, run Get-Help about_Hash_Tables.


BODYPARAMETER <IPathsSit1AcInformationprotectionMicrosoftGraphVerifysignaturePostRequestbodyContentApplicationJsonSchema>: .
  - `[(Any) <Object>]`: This indicates any property can be added to this object.
  - `[Digest <Byte[]>]`: 
  - `[Signature <Byte[]>]`: 
  - `[SigningKeyId <String>]`: 

## RELATED LINKS

