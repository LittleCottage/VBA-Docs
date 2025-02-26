---
title: Font.ItalicBi property (Publisher)
keywords: vbapb10.chm5373969
f1_keywords:
- vbapb10.chm5373969
ms.prod: publisher
api_name:
- Publisher.Font.ItalicBi
ms.assetid: 604e776c-92b0-6e5b-2599-ab879c61a78a
ms.date: 06/08/2019
ms.localizationpriority: medium
---


# Font.ItalicBi property (Publisher)

Returns or sets an **[MsoTriState](Office.MsoTriState.md)** constant indicating whether the specified text is formatted as italic; applies to text in a right-to-left language. Read/write.


## Syntax

_expression_.**ItalicBi**

_expression_ A variable that represents a **[Font](Publisher.Font.md)** object.


## Return value

MsoTriState


## Remarks

The **ItalicBi** property value can be one of the **MsoTriState** constants declared in the Microsoft Office type library and shown in the following table.

|Constant|Description|
|:-----|:-----|
| **msoFalse**| None of the characters in the range are formatted as italic.|
| **msoTriStateMixed**|A return value indicating a combination of **msoTrue** and **msoFalse** for the specified shape range.|
| **msoTriStateToggle**|A set value that switches between **msoTrue** and **msoFalse**.|
| **msoTrue**|All of the characters in the range are formatted as italic.|

## Example

This example tests the text in the first story and displays one of two possible text boxes, depending on whether the text is right-to-left formatted and whether its font is formatted as italic.

```vb
Sub ItalicRtoL() 
 
 Dim stf As Font 
 
 Set stf = Application.ActiveDocument.Stories(1).TextRange.Font 
 With stf 
 If .ItalicBi = msoTrue Then 
 MsgBox "This story is right-to-left and is formatted as italic." 
 Else 
 MsgBox "This story is either not right-to-left" & _ 
 " or it is not formatted as italic" 
 End If 
 End With 
 
End Sub
```

[!include[Support and feedback](~/includes/feedback-boilerplate.md)]