---
title: Master.BeforeShapeDelete event (Visio)
keywords: vis_sdr.chm10719065
f1_keywords:
- vis_sdr.chm10719065
ms.prod: visio
api_name:
- Visio.Master.BeforeShapeDelete
ms.assetid: 21921e16-3e05-6232-ed89-76217b76149f
ms.date: 06/08/2017
ms.localizationpriority: medium
---


# Master.BeforeShapeDelete event (Visio)

Occurs before a shape is deleted.


## Syntax

_expression_.**BeforeShapeDelete** (_Shape_)

_expression_ A variable that represents a **[Master](Visio.Master.md)** object.


## Parameters



|Name|Required/Optional|Data type|Description|
|:-----|:-----|:-----|:-----|
| _Shape_|Required| **[IVSHAPE]**|The shape that is going to be deleted.|

## Remarks

A **Shape** object can serve as the source object for the **BeforeShapeDelete** event if the shape's **Type** property is **visTypeGroup** (2) or **visTypePage** (1).

The **BeforeSelectionDelete** and **BeforeShapeDelete** events are similar in that they both fire before shape(s) are deleted. They differ in how they behave when a single operation deletes several shapes. Suppose a **Cut** operation deletes three shapes. The **BeforeShapeDelete** event fires three times and acts on each of the three objects. The **BeforeSelectionDelete** event fires once, and it acts on a **Selection** object in which the three shapes that you want to delete are selected.

If you are using Microsoft Visual Basic or Visual Basic for Applications (VBA), the syntax in this topic describes a common, efficient way to handle events.

If you want to create your own **Event** objects, use the **[Add](visio.eventlist.add.md)** or **[AddAdvise](visio.eventlist.addadvise.md)** method. 

To create an **Event** object that runs an add-on, use the **Add** method as it applies to the **EventList** collection. 

To create an **Event** object that receives notification, use the **AddAdvise** method. 

To find an event code for the event that you want to create, see [Event codes](../visio/Concepts/event-codesvisio.md).




> [!NOTE] 
> Use the VBA **WithEvents** keyword to sink the **BeforeShapeDelete** event.

For performance considerations, the **Document** object's event set does not include the **BeforeShapeDelete** event. To sink the **BeforeShapeDelete** event from a **Document** object (and from the **[ThisDocument](../visio/Concepts/about-the-thisdocument-object-visio.md)** object in a VBA project), you must use the **AddAdvise** method.

[!include[Support and feedback](~/includes/feedback-boilerplate.md)]