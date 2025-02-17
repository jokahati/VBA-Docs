---
title: Wizard.Name property (Publisher)
keywords: vbapb10.chm1441796
f1_keywords:
- vbapb10.chm1441796
ms.prod: publisher
api_name:
- Publisher.Wizard.Name
ms.assetid: 1e0a7ec6-87ee-7c26-cf98-e849c5617e58
ms.date: 06/18/2019
ms.localizationpriority: medium
---


# Wizard.Name property (Publisher)

Returns a **String** value indicating the name of the specified object. Read-only.


## Syntax

_expression_.**Name**

_expression_ A variable that represents a **[Wizard](Publisher.Wizard.md)** object.


## Remarks

You can use an object's name in conjunction with the **Item** method or **Item** property to return a reference to the object if the **Item** method or property for the collection that contains the object takes a **Variant** argument. 

For example, if the value of the **Name** property for a shape is Rectangle 2, `.Shapes("Rectangle 2")` returns a reference to that shape.

The **Name** property is the default property for the **BorderArt**, **BorderArtFormat**, and **Label** objects.

[!include[Support and feedback](~/includes/feedback-boilerplate.md)]