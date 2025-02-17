---
title: Document.Redo event (Publisher)
keywords: vbapb10.chm285212679
f1_keywords:
- vbapb10.chm285212679
ms.prod: publisher
api_name:
- Publisher.Document.Redo
ms.assetid: c00db13d-1c03-2536-8923-bd7d9393fee2
ms.date: 06/06/2019
ms.localizationpriority: medium
---


# Document.Redo event (Publisher)

Occurs when reversing the last action that was undone.


## Syntax

_expression_.**Redo**

_expression_ A variable that represents a **[Document](Publisher.Document.md)** object.


## Remarks

The **Redo** event occurs immediately after the action is redone.

If multiple actions are redone, the **Redo** event occurs only once, after all the actions are complete.

For more information about using events with the **Document** object, see [Using events with the Document object](../publisher/Concepts/using-events-with-the-document-object-publisher.md).


## Example

This example displays a message when a user chooses **Undo** on the **Standard** toolbar or selects **Redo** from the **Edit** menu. For this routine to work with the current publication, you must put it in the **ThisDocument** module.

```vb
Private Sub DocPub_Redo() 
 MsgBox "Your last undo has been reversed." 
End Sub
```

<br/>

To trap this event from a non-Microsoft Publisher project, you must place the following code in the General Declarations section of your module and run the InitiatePubApp routine.

```vb
Private WithEvents DocPub As Publisher.Document 
 
Sub InitiatePubApp() 
 Set DocPub = Publisher.ActiveDocument 
End Sub
```

[!include[Support and feedback](~/includes/feedback-boilerplate.md)]