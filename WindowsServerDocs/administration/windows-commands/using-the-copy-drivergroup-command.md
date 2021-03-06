---
title: Using the copy-DriverGroup Command
description: "Windows Commands topic for **** - "
ms.custom: na
ms.prod: windows-server-threshold
ms.reviewer: na
ms.suite: na
ms.technology: manage-windows-commands
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: 0aaf6fa5-8b5b-4a1e-ae9b-8b5c6d89f571
author: coreyp-at-msft
ms.author: coreyp
manager: dongill
ms.date: 10/12/2016
---
# Using the copy-DriverGroup Command

>Applies To: Windows Server 2016, Windows Server 2012 R2, Windows Server 2012

Duplicates an existing driver group on the server including the filters, driver packages, and enabled/disabled status.
## Syntax
```
wdsutil /copy-DriverGroup [/Server:<Server name>] /DriverGroup:<Source Group Name> /GroupName:<New Group Name>
```
## Parameters
|Parameter|Description|
|-------|--------|
|[/Server:<Server name>]|Specifies the name of the server. This can be the NetBIOS name or the FQDN. If no server name is specified, the local server is used.|
|/DriverGroup:<Source Group Name>|Specifies the name of the source driver group.|
|/GroupName:<New Group Name>|Specifies the name of the new driver group.|
## <a name="BKMK_examples"></a>Examples
To copy a driver group, type one of the following:
```
wdsutil /copy-DriverGroup /Server:MyWdsServer /DriverGroup:printerdrivers /GroupName:X86printerdrivers
```
```
wdsutil /copy-DriverGroup /DriverGroup:printerdrivers /GroupName:colorprinterdrivers
```
#### additional references
[Command-Line Syntax Key](command-line-syntax-key.md)
