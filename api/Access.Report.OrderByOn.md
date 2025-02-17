---
title: Report.OrderByOn property (Access)
keywords: vbaac10.chm13693
f1_keywords:
- vbaac10.chm13693
ms.prod: access
api_name:
- Access.Report.OrderByOn
ms.assetid: 8784e57f-e4f1-a606-36b0-1200d6f17b89
ms.date: 03/15/2019
ms.localizationpriority: medium
---


# Report.OrderByOn property (Access)

You can use the **OrderByOn** property to specify whether an object's **OrderBy** property setting is applied. Read/write **Boolean**.


## Syntax

_expression_.**OrderByOn**

_expression_ A variable that represents a **[Report](Access.Report.md)** object.


## Remarks

The **OrderByOn** property uses the following settings.

|Setting|Visual Basic|Description|
|:-----|:-----|:-----|
|Yes|**True**|The **OrderBy** property setting is applied when the object is opened.|
|No|**False**|(Default) The **OrderBy** property setting isn't applied when the object is opened.|

When a new object is created, it inherits the **RecordSource**, **Filter**, **OrderBy**, **OrderByOn**, and **FilterOn** properties of the table or query that it was created from.


## Example

The following example displays a message indicating the state of the **OrderByOn** property for the **Mailing List** form.

```vb
MsgBox "OrderByOn property is " & Forms("Mailing List").OrderByOn
```



[!include[Support and feedback](~/includes/feedback-boilerplate.md)]