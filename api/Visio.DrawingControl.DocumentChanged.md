---
title: DrawingControl.DocumentChanged event (Visio)
ms.prod: visio
api_name:
- Visio.DrawingControl.DocumentChanged
ms.assetid: b929c918-d12f-22f9-bd5b-4461a84dfb83
ms.date: 06/08/2017
ms.localizationpriority: medium
---


# DrawingControl.DocumentChanged event (Visio)

Occurs after certain properties of a document are changed.


## Syntax

_expression_.**DocumentChanged** (_doc_)

_expression_ A variable that represents a **[DrawingControl](Visio.DrawingControl.md)** object.


## Parameters



|Name|Required/Optional|Data type|Description|
|:-----|:-----|:-----|:-----|
| _doc_|Required| **[IVDOCUMENT]**|The document whose properties were changed.|

## Remarks

The **DocumentChanged** event indicates that one of a document's properties, such as **Author** or **Description**, has changed.

If you are using Microsoft Visual Basic or Visual Basic for Applications (VBA), the syntax in this topic describes a common, efficient way to handle events.

If you want to create your own **Event** objects, use the **[Add](visio.eventlist.add.md)** or **[AddAdvise](visio.eventlist.addadvise.md)** method. 

To create an **Event** object that runs an add-on, use the **Add** method as it applies to the **EventList** collection. 

To create an **Event** object that receives notification, use the **AddAdvise** method. 

To find an event code for the event that you want to create, see [Event codes](../visio/Concepts/event-codesvisio.md).

[!include[Support and feedback](~/includes/feedback-boilerplate.md)]