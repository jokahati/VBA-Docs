---
title: Application.ColumnHistory method (Access)
keywords: vbaac10.chm12620
f1_keywords:
- vbaac10.chm12620
ms.prod: access
api_name:
- Access.Application.ColumnHistory
ms.assetid: e2c1b71f-6561-b38d-8173-9926bc4bd9da
ms.date: 02/05/2019
ms.localizationpriority: medium
---


# Application.ColumnHistory method (Access)

Gets the history of values that have been stored in a **Memo** field.


## Syntax

_expression_.**ColumnHistory** (_TableName_, _ColumnName_, _queryString_)

_expression_ A variable that represents an **[Application](Access.Application.md)** object.


## Parameters

|Name|Required/Optional|Data type|Description|
|:-----|:-----|:-----|:-----|
| _TableName_|Required|**String**|The name of the table that contains the **Append Only** field.|
| _ColumnName_|Required|**String**|The name of the field to display the history for.|
| _queryString_|Required|**String**|A **String** used to locate the record. It is like the WHERE clause in an SQL statement, but without the word WHERE.|

## Return value

String


## Remarks

A **Memo** field's **AppendOnly** property must be set to **True** for Access to store the change history for the field.


## Example

The following example prints the salary history of employee number 147 to the Immediate window.


```vb
Sub colhist() 
 Dim sHistory As String 
 
 sHistory = Application.ColumnHistory("Employees", "Salary", "ID=147") 
 Debug.Print sHistory 
End Sub
```




[!include[Support and feedback](~/includes/feedback-boilerplate.md)]