--- 
 
# required metadata 
title: "OlapConnection (olapR package for R, Microsoft Machine Learning Server) | Microsoft Docs" 
description: "Constructs an OlapConnection object. " 
keywords: "olapR, OlapConnection" 
author: "richcalaway"
ms.author: "richcala" 
manager: "jhubbard" 
ms.date: "03/23/2017" 
ms.topic: "reference" 
ms.prod: "microsoft-r" 
ms.service: "" 
ms.assetid: "" 
 
# optional metadata 
#ROBOTS: "" 
#audience: "" 
#ms.devlang: "" 
#ms.reviewer: "" 
#ms.suite: "" 
#ms.tgt_pltfrm: "" 
ms.technology: "r-server" 
#ms.custom: "" 
 
--- 
 
 # **OlapConnection**

 Applies to: [**olapR package for R**](../r-reference/olapR/olapr.md), version 1.0.0 

 ##Description
 
Constructs an OlapConnection object.
 
 ##Usage

```   
  OlapConnection(connectionString="Data Source=localhost; Provider=MSOLAP;")
  
  is.OlapConnection(ocs)
  
  print.OlapConnection(ocs)
 
```
## (metadata)

This is what the metadata looks like:

`title: "OlapConnection (olapR package for R, Microsoft Machine Learning Server) | Microsoft Docs" `

`description: "Constructs an OlapConnection object. " `
 
 ##Arguments
    
 ### connectionString
 A valid connection string for connecting to Analysis Services 
  
    
 ### ocs
 An object of class "OlapConnection" 
  
 
 
 
 ##Details
 
`OlapConnection` validates and holds an Analysis Services connection string.
 
 
 
 ##Value
 
`OlapConnection` returns an object of type "OlapConnection". A warning is shown if the connection string is invalid.
 
 
 ##References
  For more information on Analysis Services connection strings: [`https://msdn.microsoft.com/en-us/library/dn140245.aspx`](https://msdn.microsoft.com/en-us/library/dn140245.aspx)
  
 
 
 ##See Also
 
[Query](query.md), [executeMD](executemd.md), [execute2D](execute2d.md)`, `[explore](explore.md)
   
 
 ##Examples

 ```
   
  cnnstr <- "Data Source=localhost; Provider=MSOLAP;"
  olapCnn <- OlapConnection(cnnstr)
 
```
 