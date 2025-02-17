---
title: Shape.ScaleWidth method (Publisher)
keywords: vbapb10.chm2228262
f1_keywords:
- vbapb10.chm2228262
ms.prod: publisher
api_name:
- Publisher.Shape.ScaleWidth
ms.assetid: 07dcc04e-cb84-9c69-c589-87c0ff0bb147
ms.date: 06/13/2019
ms.localizationpriority: medium
---


# Shape.ScaleWidth method (Publisher)

Scales the width of the shape by a specified factor. For pictures and OLE objects, you can indicate whether you want to scale the shape relative to the original size or relative to the current size.


## Syntax

_expression_.**ScaleWidth** (_Factor_, _RelativeToOriginalSize_, _fScale_)

_expression_ A variable that represents a **[Shape](Publisher.Shape.md)** object.


## Parameters

|Name|Required/Optional|Data type|Description|
|:-----|:-----|:-----|:-----|
|_Factor_|Required| **Single**|Specifies the ratio between the width of the shape after you resize it and the current or original width. For example, to make a rectangle 50 percent larger, specify 1.5 for this argument.|
|_RelativeToOriginalSize_|Required| **[MsoTriState](office.msotristate.md)**| Specifies whether to scale relative to the object's original or current size.|
|_fScale_|Optional| **[MsoScaleFrom](office.msoscalefrom.md)**|The part of the shape that retains its position when the shape is scaled. Can be one of the **MsoScaleFrom** constants declared in the Microsoft Office type library.|

## Remarks

The _RelativeToOriginalSize_ parameter can be one of the **MsoTriState** constants declared in the Microsoft Office type library and shown in the following table.

|Constant|Description|
|:-----|:-----|
| **msoFalse**|Scales the shape relative to its current size.|
| **msoTrue**|Scales the shape relative to its original size.|


Shapes other than pictures and OLE objects are always scaled relative to their current width; specifying a _RelativeToOriginalSize_ value of **msoTrue** for shapes other than pictures or OLE objects causes an error.

Use the **[ScaleHeight](Publisher.Shape.ScaleHeight.md)** method to scale the height of a shape.


## Example

This example scales all pictures and OLE objects on the first page of the active publication to 175 percent of their original height and width, and it scales all other shapes to 175 percent of their current height and width.

```vb
' Looping variable. 
Dim shpLoop As Shape 
 
' Loop through all the shapes on the first page. 
For Each shpLoop In ActiveDocument.Pages(1).Shapes 
 With shpLoop 
 Select Case .Type 
 ' If the shape is a picture or OLE object, 
 ' scale relative to original size. 
 Case pbPicture, pbLinkedPicture, _ 
 pbEmbeddedOLEObject, pbLinkedOLEObject, _ 
 pbOLEControlObject 
 .ScaleHeight Factor:=1.75, _ 
 RelativeToOriginalSize:=True 
 .ScaleWidth Factor:=1.75, _ 
 RelativeToOriginalSize:=True 
 ' If the shape is not a picture or OLE object, 
 ' scale relative to the current size. 
 Case Else 
 .ScaleHeight Factor:=1.75, _ 
 RelativeToOriginalSize:=False 
 .ScaleWidth Factor:=1.75, _ 
 RelativeToOriginalSize:=False 
 End Select 
 End With 
Next shpLoop 

```

[!include[Support and feedback](~/includes/feedback-boilerplate.md)]