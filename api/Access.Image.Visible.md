---
title: Image.Visible property (Access)
keywords: vbaac10.chm10374
f1_keywords:
- vbaac10.chm10374
ms.prod: access
api_name:
- Access.Image.Visible
ms.assetid: 022201dd-2847-dba5-2a0e-86e94feab535
ms.date: 02/27/2019
ms.localizationpriority: medium
---


# Image.Visible property (Access)

Returns or sets whether the object is visible. Read/write **Boolean**.


## Syntax

_expression_.**Visible**

_expression_ A variable that represents an **[Image](Access.Image.md)** object.


## Remarks

To hide an object when printing, use the **DisplayWhen** property.

You can use the **Visible** property to hide a control on a form or report by including the property in a macro or event procedure that runs when the **Current** event occurs. For example, you can show or hide a congratulatory message next to a salesperson's monthly sales total in a sales report, depending on the sales total.




[!include[Support and feedback](~/includes/feedback-boilerplate.md)]