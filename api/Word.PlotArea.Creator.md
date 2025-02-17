---
title: PlotArea.Creator property (Word)
keywords: vbawd10.chm53477525
f1_keywords:
- vbawd10.chm53477525
ms.prod: word
api_name:
- Word.PlotArea.Creator
ms.assetid: 340fb047-e239-3d54-853b-8cbc3919ab2b
ms.date: 06/08/2017
ms.localizationpriority: medium
---


# PlotArea.Creator property (Word)

Returns a 32-bit integer that indicates the application in which the specified object was created. Read-only  **Long**.


## Syntax

_expression_.**Creator**

_expression_ A variable that represents a '[PlotArea](Word.PlotArea.md)' object.


## Remarks

If the object was created in Microsoft Word, the **Creator** property returns the hexadecimal number 4D535744, which represents the string "MSWD". This property was primarily designed to be used on the Macintosh, where each application has a four-character creator code. For example, Word has the creator code MSWD. For more information about this property, consult the language reference Help included with Microsoft Office for Mac.


## See also


[PlotArea Object](Word.PlotArea.md)

[!include[Support and feedback](~/includes/feedback-boilerplate.md)]