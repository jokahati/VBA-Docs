---
title: Editors.Creator property (Word)
keywords: vbawd10.chm9176041
f1_keywords:
- vbawd10.chm9176041
ms.prod: word
api_name:
- Word.Editors.Creator
ms.assetid: 4589fef6-ca9d-ab15-cbc4-77a72ddce4a2
ms.date: 06/08/2017
ms.localizationpriority: medium
---


# Editors.Creator property (Word)

Returns a 32-bit integer that indicates the application in which the specified object was created. Read-only  **Long**.


## Syntax

_expression_.**Creator**

_expression_ Required. A variable that represents an '[Editors](Word.Editors.md)' collection.


## Remarks

If the object was created in Microsoft Word, the **Creator** property returns the hexadecimal number 4D535744, which represents the string "MSWD." This property was primarily designed to be used on the Macintosh, where each application has a four-character creator code. For example, Microsoft Word has the creator code MSWD. For additional information about this property, consult the language reference Help included with Microsoft Office Macintosh Edition.


## See also


[Editors Collection](Word.Editors.md)

[!include[Support and feedback](~/includes/feedback-boilerplate.md)]