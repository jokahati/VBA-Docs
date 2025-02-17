---
title: PageBreak.Application property (Access)
keywords: vbaac10.chm11667
f1_keywords:
- vbaac10.chm11667
ms.prod: access
api_name:
- Access.PageBreak.Application
ms.assetid: 6f5eb0f3-5a82-882c-4c57-08613fb6421a
ms.date: 03/23/2019
ms.localizationpriority: medium
---


# PageBreak.Application property (Access)

You can use the **Application** property to access the active Microsoft Access **[Application](Access.Application.md)** object and its related properties. Read-only **Application** object.


## Syntax

_expression_.**Application**

_expression_ A variable that represents a **[PageBreak](Access.PageBreak.md)** object.


## Remarks

The **Application** property is set by Microsoft Access and is read-only in all views.

Each Microsoft Access object has an **Application** property that returns the current **Application** object. You can use this property to access any of the object's properties. For example, you could refer to the menu bar for the **Application** object from the current form by using the following syntax.

```vb
Me.Application.MenuBar 

```



[!include[Support and feedback](~/includes/feedback-boilerplate.md)]