---
title: Dfsdiag TestDCs
description: "Windows Commands topic for **** -- "
ms.custom: na
ms.prod: windows-server-threshold
ms.reviewer: na
ms.suite: na
ms.technology: manage-windows-commands
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: abb915ab-23eb-45d7-9a2e-b6b9a5756a70
author: coreyp-at-msft
ms.author: coreyp
manager: dongill
ms.date: 10/12/2016
---

# Dfsdiag TestDCs

>Applies To: Windows Server&reg; 2016, Windows Server&reg; 2012 R2, Windows Server&reg; 2012

Checks the configuration of domain controllers by performing the following tests on each domain controller in the specified domain:  
  
-   Verifies that the Distributed File System \(DFS\) Namespace service is running and that its Startup Type is set to Automatic.  
  
-   Checks for the support of site\-costed referrals for NETLOGON and SYSVOL.  
  
-   Verifies the consistency of the site association by hostname and IP address.  
  
  
  
## Syntax  
  
```  
DFSDiag /TestDCs [/Domain:<Domain name>]  
```  
  
### Parameters  
  
|Parameter|Description|  
|-------------|---------------|  
|\/Domain:<Domain name>|Domain that you want to check.|  
  
## Remarks  
\/Domain is an optional parameter. The default value is the local domain that the local host is joined to.  
  
## <a name="BKMK_Examples"></a>Examples  
To verify the configuration of domain controllers in the Contoso.com domain, type:  
  
```  
DFSDiag /TestDCs /Domain:Contoso.com  
```  
  
## Additional references  
  
-   [Command-Line Syntax Key](Command-Line-Syntax-Key.md)  
  
-   [Dfsdiag](Dfsdiag.md)  
  
