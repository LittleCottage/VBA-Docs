---
title: CustomControl.ObjectVerbsCount property (Access)
keywords: vbaac10.chm12037
f1_keywords:
- vbaac10.chm12037
ms.prod: access
api_name:
- Access.CustomControl.ObjectVerbsCount
ms.assetid: f7c74900-3f0d-b6b1-3606-ca8d206f85b3
ms.date: 03/06/2019
ms.localizationpriority: medium
---


# CustomControl.ObjectVerbsCount property (Access)

Use the **ObjectVerbsCount** property in Visual Basic to determine the number of verbs supported by an OLE object. Read-only **Long**.


## Syntax

_expression_.**ObjectVerbsCount** 

_expression_ A variable that represents a **[CustomControl](Access.CustomControl.md)** object.


## Remarks

The **ObjectVerbsCount** property setting is a value that specifies the number of elements in the **ObjectVerbs** property array.

This property setting isn't available in Design view.

The list of verbs an OLE object supports may vary, depending on the state of the object. To update the list of supported verbs, set the control's **Action** property to **acOLEFetchVerbs**.


## Example

The following example returns the verbs supported by the OLE object in the OLE1 control and displays each verb in a message box.


```vb
Sub GetVerbList(frm As Form, OLE1 As Control) 
 Dim intX As Integer, intNumVerbs As Integer 
 Dim strVerbList As String 
 
 ' Update verb list. 
 With frm!OLE1 
 .Action = acOLEFetchVerbs 
 intNumVerbs = .ObjectVerbsCount 
 For intX = 0 To intNumVerbs - 1 
 strVerbList = strVerbList & .ObjectVerbs(intX) & "; " 
 Next intX 
 End With 
 
 ' Display verbs in message box. 
 MsgBox Left(strVerbList, Len(strVerbList) - 2) 
End Sub
```




[!include[Support and feedback](~/includes/feedback-boilerplate.md)]