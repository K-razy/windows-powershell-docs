---
external help file: 
Module Name: RemoteDesktop
online version: 
schema: 2.0.0
title: Remove-RDSessionCollection
description: 
keywords: powershell, cmdlet
author: Kateyanne
manager: jasgro
ms.date: 10/29/2017
ms.topic: reference
ms.prod: powershell
ms.assetid: 68EB435A-53DA-4A71-B6CC-C6F8BDC80658
ms.author: v-kaunu
ms.reviewer: brianlic
---

# Remove-RDSessionCollection

## SYNOPSIS
Removes a session collection from a Remote Desktop deployment.

## SYNTAX

```
Remove-RDSessionCollection [-CollectionName] <String> [-ConnectionBroker <String>] [-Force] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
The **Remove-RDSessionCollection** cmdlet removes a session collection from a Remote Desktop deployment.
A session collection consists of one or more Remote Desktop Session Host (RD Session Host) servers.
The RD Session Host servers remain part of the deployment.
This cmdlet does not remove or modify any of the role services installed on the servers.

## EXAMPLES

### Example 1: Remove a session collection
```
PS C:\> Remove-RDSessionCollection -CollectionName "Session Collection" -ConnectionBroker "RDCB.Contoso.com"
```

This command removes the session collection named Session Collection from the Remote Desktop deployment that has the RD Connection Broker named RDCB.Contoso.com.

## PARAMETERS

### -CollectionName
Specifies the name of a session collection.

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

### -Confirm
Prompts you for confirmation before running the cmdlet.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: cf

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -ConnectionBroker
Specifies the Remote Desktop Connection Broker (RD Connection Broker) server for a Remote Desktop deployment.
If you do not specify a value, the cmdlet uses the fully qualified domain name (FQDN) of the local computer.

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

### -Force
Performs the action without a confirmation message.

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

### -WhatIf
Shows what would happen if the cmdlet runs.
The cmdlet is not run.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: wi

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

### Null

## NOTES

## RELATED LINKS

[Get-RDSessionCollection](./Get-RDSessionCollection.md)

[New-RDSessionCollection](./New-RDSessionCollection.md)

