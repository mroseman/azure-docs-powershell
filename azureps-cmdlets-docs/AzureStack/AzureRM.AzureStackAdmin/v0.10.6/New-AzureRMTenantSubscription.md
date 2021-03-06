---
external help file: Microsoft.AzureStack.Commands.dll-Help.xml
online version: 
schema: 2.0.0
---

# New-AzureRMTenantSubscription

## SYNOPSIS
The cmdlet New-AzureRMTenantSubscription creates a subscription as a tenant for the specified offer

## SYNTAX

```
New-AzureRMTenantSubscription -OfferId <String> [-DisplayName <String>] [-InformationAction <ActionPreference>]
 [-InformationVariable <String>] [-PipelineVariable <String>] [<CommonParameters>]
```

## DESCRIPTION

## EXAMPLES

### -------------------------- EXAMPLE 1 --------------------------
```
New-AzureRmTenantSubscription  -OfferId $offer.Id -DisplayName "Compute Subscription"
```

Description

-----------

The example creates a subscription for the logged in tenant user

            $Offer =  Get-AzureRMOffer -Provider "default" | Where-Object name -eq "ComputeOffer"
            New-AzureRmTenantSubscription  -OfferId $offer.Id -DisplayName "Compute Subscription"

## PARAMETERS

### -DisplayName
@{Text=}

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

### -InformationAction
Not Specified

The following values are permitted for this object type.

```yaml
Type: ActionPreference
Parameter Sets: (All)
Aliases: infa
Accepted values: SilentlyContinue, Stop, Continue, Inquire

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InformationVariable
Not Specified

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

### -OfferId
Specifies the Id of the offer to which the tenant subscribes to create a new subscription

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PipelineVariable
Not Specified

```yaml
Type: String
Parameter Sets: (All)
Aliases: pv

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

### Microsoft.AzureStack.Management.Models.SubscriptionDefinition

## NOTES

## RELATED LINKS

