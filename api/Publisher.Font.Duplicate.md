---
title: Font.Duplicate method (Publisher)
keywords: vbapb10.chm5373992
f1_keywords:
- vbapb10.chm5373992
ms.prod: publisher
api_name:
- Publisher.Font.Duplicate
ms.assetid: 26ae64bc-036e-5c19-cbac-99f11da7fb60
ms.date: 06/08/2019
ms.localizationpriority: medium
---


# Font.Duplicate method (Publisher)

Creates a duplicate of the specified **Font** object and then returns the new **Font** object.


## Syntax

_expression_.**Duplicate**

_expression_ A variable that represents a **[Font](Publisher.Font.md)** object.


## Return value

Font


## Example

The following example duplicates the character formatting information from the text range in shape one on page one of the active publication and applies it to the text range in shape two.

```vb
Dim fntTemp As Font 
 
With ActiveDocument.Pages(1) 
 Set fntTemp = _ 
 .Shapes(1).TextFrame.TextRange.Font.Duplicate 
 .Shapes(2).TextFrame.TextRange.Font = fntTemp 
End With
```

[!include[Support and feedback](~/includes/feedback-boilerplate.md)]