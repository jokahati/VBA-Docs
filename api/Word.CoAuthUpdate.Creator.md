---
title: CoAuthUpdate.Creator property (Word)
keywords: vbawd10.chm247792617
f1_keywords:
- vbawd10.chm247792617
ms.prod: word
api_name:
- Word.CoAuthUpdate.Creator
ms.assetid: 68e57f41-0826-87bf-e767-7004268f5824
ms.date: 06/08/2017
ms.localizationpriority: medium
---


# CoAuthUpdate.Creator property (Word)

Returns a 32-bit integer that indicates the application in which the specified object was created. Read-only  **Long**.


## Syntax

_expression_.**Creator**

 _expression_ An expression that returns a [CoAuthUpdate](./Word.CoAuthUpdate.md) object.


## Remarks

If the object was created in Microsoft Word, the **Creator** property returns the hexadecimal number 4D535744, which represents the **string** "MSWD". This property was primarily designed to be used on the Apple Macintosh, where each application has a four-character creator code. For example, Microsoft Word has the creator code MSWD. For more information about this property, see the language reference Help included with Microsoft Office Macintosh Edition.


> [!NOTE] 
> This value can also be represented by the constant **wdCreatorCode**.


## See also


[CoAuthUpdate Object](Word.CoAuthUpdate.md)

[!include[Support and feedback](~/includes/feedback-boilerplate.md)]