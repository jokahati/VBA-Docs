---
title: Understanding conditional compilation (VBA)
keywords: vbcn6.chm1076725
f1_keywords:
- vbcn6.chm1076725
ms.prod: office
ms.assetid: d79bb580-f77e-b9fc-5548-3ee2b193947b
ms.date: 12/21/2018
ms.localizationpriority: medium
---


# Understanding conditional compilation

You can use conditional compilation to run blocks of code selectively, for example, debugging statements comparing the speed of different approaches to the same programming task, or localizing an application for different languages.

You declare a [conditional compiler constant](../../Glossary/vbe-glossary.md#conditional-compiler-constant) in code with the **[#Const](../../reference/user-interface-help/const-directive.md)** directive, and you denote blocks of code to be conditionally compiled with the **[#If...Then...#Else](../../reference/user-interface-help/ifthenelse-directive.md)** directive. 

The following example runs debug code or production code, based on the value of the [variable](../../Glossary/vbe-glossary.md#variable).

```vb
' Declare public compilation constant in Declarations section. 
#Const conDebug = 1 
 
Sub SelectiveExecution() 
 #If conDebug = 1 Then 
 . ' Run code with debugging statements. 
 . 
 . 
 #Else 
 . ' Run normal code. 
 . 
 . 
 #End If 
End Sub
```

## See also

- [Compiler constants](compiler-constants.md)
- [Visual Basic conceptual topics](../../reference/user-interface-help/visual-basic-conceptual-topics.md)

[!include[Support and feedback](~/includes/feedback-boilerplate.md)]