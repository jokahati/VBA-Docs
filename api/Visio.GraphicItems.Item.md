---
title: GraphicItems.Item property (Visio)
keywords: vis_sdr.chm16813765
f1_keywords:
- vis_sdr.chm16813765
ms.prod: visio
api_name:
- Visio.GraphicItems.Item
ms.assetid: bcd5ed67-3913-41ea-0d51-30ad24d04196
ms.date: 06/08/2017
ms.localizationpriority: medium
---


# GraphicItems.Item property (Visio)

Returns the  **GraphicItem** object at the specified index position in the **GraphicItems** collection. Read-only.


> [!NOTE] 
> This Visio object or member is available only to licensed users of Visio Professional 2013.


## Syntax

_expression_.**Item** (_Index_)

_expression_ A variable that represents a **[GraphicItems](Visio.GraphicItems.md)** object.


## Parameters



|Name|Required/Optional|Data type|Description|
|:-----|:-----|:-----|:-----|
| _Index_|Required| **Long**|The index of the object to retrieve.|

## Return value

GraphicItem


## Remarks

 **Item** is the default property of the **GraphicItems** collection.

 The **GraphicItems** collection is indexed starting with 1.

When you retrieve objects from a collection, you can omit  **Item** from the expression because it is the default property of all collections. The following statement is equivalent to the syntax example given above:




```vb
objectReturned = expression(Index)
```

[!include[Support and feedback](~/includes/feedback-boilerplate.md)]