---
title: Menu.FaceID property (Visio)
keywords: vis_sdr.chm13113495
f1_keywords:
- vis_sdr.chm13113495
ms.prod: visio
api_name:
- Visio.Menu.FaceID
ms.assetid: 03270afe-84ea-d21d-9077-5967dfce3550
ms.date: 06/08/2017
ms.localizationpriority: medium
---


# Menu.FaceID property (Visio)

Gets or sets the icon for an item. Read/write.


## Syntax

_expression_. `FaceID`

_expression_ A variable that represents a **[Menu](Visio.Menu.md)** object.


## Return value

Integer


## Remarks


> [!NOTE] 
> Starting with Visio 2010, the Microsoft Office Fluent user interface (UI) replaced the previous system of layered menus, toolbars, and task panes. VBA objects and members that you used to customize the user interface in previous versions of Visio are still available in Visio, but they function differently.

Use any of the constants prefixed with **visIconIX** that are declared by the Visio type library in **[VisUIIconIDs](Visio.visuiiconids.md)**.

The **FaceID** property is the same as the **TypeSpecific1** property when the **CtrlType** property is type **visCtrlTypeBUTTON**, which is declared in the Visio type library in **[VisUICtrlTypes](Visio.visuictrltypes.md)**.

[!include[Support and feedback](~/includes/feedback-boilerplate.md)]