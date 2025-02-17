---
title: Document.LayoutGuides property (Publisher)
keywords: vbapb10.chm196626
f1_keywords:
- vbapb10.chm196626
ms.prod: publisher
api_name:
- Publisher.Document.LayoutGuides
ms.assetid: 0c45366d-6b7a-7cf3-a566-bb945ff32ba4
ms.date: 06/06/2019
ms.localizationpriority: medium
---


# Document.LayoutGuides property (Publisher)

Returns a **[LayoutGuides](Publisher.LayoutGuides.md)** object consisting of the margin and grid layout guides for all pages including master pages in the publication.


## Syntax

_expression_.**LayoutGuides**

_expression_ A variable that represents a **[Document](Publisher.Document.md)** object.


## Example

The following example changes the grid layout guides so that there are three columns and five rows.

```vb
Dim layTemp As LayoutGuides 
 
Set layTemp = ActiveDocument.LayoutGuides 
 
With layTemp 
 .Rows = 5 
 .Columns = 3 
End With 

```

[!include[Support and feedback](~/includes/feedback-boilerplate.md)]