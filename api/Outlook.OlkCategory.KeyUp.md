---
title: OlkCategory.KeyUp event (Outlook)
keywords: vbaol11.chm1000458
f1_keywords:
- vbaol11.chm1000458
ms.prod: outlook
api_name:
- Outlook.OlkCategory.KeyUp
ms.assetid: ce4ad525-fe0e-17d8-656f-4a3557e2ff6f
ms.date: 06/08/2017
ms.localizationpriority: medium
---


# OlkCategory.KeyUp event (Outlook)

Occurs when the user releases a key.


## Syntax

_expression_. `KeyUp`( `_KeyCode_` , `_Shift_` )

_expression_ A variable that represents an [OlkCategory](Outlook.OlkCategory.md) object.


## Parameters



|Name|Required/Optional|Data type|Description|
|:-----|:-----|:-----|:-----|
| _KeyCode_|Required| **Long**|The numerical value of the key pressed.|
| _Shift_|Required| **Integer**|A bitwise-OR mask of constants in the  **[OlShiftState](Outlook.OlShiftState.md)** enumeration that specifies whether the **SHIFT**,  **CTRL**, or  **ALT** keys have been pressed.|

## Remarks

The state of the modifier keys (**SHIFT**,  **CTRL**, or  **ALT**) that are pressed during the  **KeyUp** event is accessible through the _Shift_ parameter.


## See also


[OlkCategory Object](Outlook.OlkCategory.md)

[!include[Support and feedback](~/includes/feedback-boilerplate.md)]