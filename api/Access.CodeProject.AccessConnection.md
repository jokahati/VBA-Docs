---
title: CodeProject.AccessConnection property (Access)
keywords: vbaac10.chm12726
f1_keywords:
- vbaac10.chm12726
ms.prod: access
api_name:
- Access.CodeProject.AccessConnection
ms.assetid: 04b389d0-b87f-9eb9-f067-6b5e0d68e3f8
ms.date: 02/27/2019
ms.localizationpriority: medium
---


# CodeProject.AccessConnection property (Access)

You can use the **AccessConnection** property to return a reference to the current Microsoft ActiveX Data Objects (ADO) **Connection** object and its related properties. Read-only **Connection**.


## Syntax

_expression_.**AccessConnection**

_expression_ A variable that represents a **[CodeProject](Access.CodeProject.md)** object.


## Remarks

You should use the **AccessConnection** property if you intend to create ADO recordsets that will be bound to Access forms. The form will not be updateable unless it is created by using the OLE DB Provider for Microsoft Access, even if the recordset is updateable in ADO. 




[!include[Support and feedback](~/includes/feedback-boilerplate.md)]