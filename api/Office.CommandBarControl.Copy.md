---
title: CommandBarControl.Copy method (Office)
ms.prod: office
api_name:
- Office.CommandBarControl.Copy
ms.assetid: 4314de01-8a25-0ab4-582f-7a61f62f8a18
ms.date: 01/04/2019
ms.localizationpriority: medium
---


# CommandBarControl.Copy method (Office)

Copies a command bar control to an existing command bar.

> [!NOTE] 
> The use of CommandBars in some Microsoft Office applications has been superseded by the new ribbon component of the Microsoft Office Fluent user interface. For more information, see [Overview of the Office Fluent ribbon](../library-reference/concepts/overview-of-the-office-fluent-ribbon.md).


## Syntax

_expression_.**Copy** (_Bar_, _Before_)

_expression_ A variable that represents a **[CommandBarControl](Office.CommandBarControl.md)** object.


## Parameters

|Name|Required/Optional|Data type|Description|
|:-----|:-----|:-----|:-----|
| _Bar_|Optional|**Variant**|A **[CommandBar](office.commandbar.md)** object that represents the destination command bar. If this argument is omitted, the control is copied to the command bar where the control already exists.|
| _Before_|Optional|**Variant**|A number that indicates the position for the new control on the command bar. The new control will be inserted before the control at this position. If this argument is omitted, the control is copied to the end of the command bar.|

## Return value

CommandBarControl


## See also

- [CommandBarControl object members](overview/library-reference/commandbarcontrol-members-office.md)

[!include[Support and feedback](~/includes/feedback-boilerplate.md)]