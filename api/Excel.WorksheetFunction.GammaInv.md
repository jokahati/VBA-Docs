---
title: WorksheetFunction.GammaInv method (Excel)
keywords: vbaxl10.chm137191
f1_keywords:
- vbaxl10.chm137191
ms.prod: excel
api_name:
- Excel.WorksheetFunction.GammaInv
ms.assetid: 7b0e95f4-dd58-50f2-89ec-22bfa932766f
ms.date: 05/23/2019
ms.localizationpriority: medium
---


# WorksheetFunction.GammaInv method (Excel)

Returns the inverse of the gamma cumulative distribution. If p = GAMMADIST(x,...), then GAMMAINV(p,...) = x.

> [!IMPORTANT] 
> This function has been replaced with one or more new functions that may provide improved accuracy and whose names better reflect their usage. This function is still available for compatibility with earlier versions of Excel. However, if backward compatibility is not required, you should consider using the new functions from now on, because they more accurately describe their functionality.
> 
> For more information about the new function, see the **[Gamma_Inv](Excel.WorksheetFunction.GammaInv.md)** method.

## Syntax

_expression_.**GammaInv** (_Arg1_, _Arg2_, _Arg3_)

_expression_ A variable that represents a **[WorksheetFunction](Excel.WorksheetFunction.md)** object.


## Parameters

|Name|Required/Optional|Data type|Description|
|:-----|:-----|:-----|:-----|
| _Arg1_|Required| **Double**|Probability - the probability associated with the gamma distribution.|
| _Arg2_|Required| **Double**|Alpha - a parameter to the distribution.|
| _Arg3_|Required| **Double**|Beta - a parameter to the distribution. If beta = 1, **GammaInv** returns the standard gamma distribution.|

## Return value

**Double**


## Remarks

You can use this function to study a variable whose distribution may be skewed.

If any argument is text, **GammaInv** returns the #VALUE! error value.
    
If probability < 0 or probability > 1, **GammaInv** returns the #NUM! error value.
    
If alpha ≤ 0 or if beta ≤ 0, **GammaInv** returns the #NUM! error value.
    
Given a value for probability, **GammaInv** seeks that value x such that GAMMADIST(x, alpha, beta, TRUE) = probability. Thus, precision of **GammaInv** depends on precision of **GammaDist**. **GammaInv** uses an iterative search technique. If the search has not converged after 64 iterations, the function returns the #N/A error value.



[!include[Support and feedback](~/includes/feedback-boilerplate.md)]