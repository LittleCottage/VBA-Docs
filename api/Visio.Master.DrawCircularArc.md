---
title: Master.DrawCircularArc method (Visio)
keywords: vis_sdr.chm10752015
f1_keywords:
- vis_sdr.chm10752015
ms.prod: visio
api_name:
- Visio.Master.DrawCircularArc
ms.assetid: f9557127-8470-2968-3056-0e295cd05633
ms.date: 06/08/2017
ms.localizationpriority: medium
---


# Master.DrawCircularArc method (Visio)

Creates a new shape whose path consists of a circular arc defined by its center, radius, and start and end angles.


## Syntax

_expression_. `DrawCircularArc`( `_xCenter_` , `_yCenter_` , `_Radius_` , `_StartAngle_` , `_EndAngle_` )

_expression_ A variable that represents a **[Master](Visio.Master.md)** object.


## Parameters



|Name|Required/Optional|Data type|Description|
|:-----|:-----|:-----|:-----|
| _xCenter_|Required| **Double**|The x-coordinate of the center of the arc.|
| _yCenter_|Required| **Double**|The y-coordinate of the center of the arc.|
| _Radius_|Required| **Double**|The radius of the arc.|
| _StartAngle_|Optional| **Double**|The angle in radians with respect to the x-axis at which to start drawing the arc. The default is 0.|
| _EndAngle_|Optional| **Double**|The angle in radians with respect to the x-axis at which to end the arc. The default is pi (3.14592634898).|

## Return value

Shape


## Remarks

By default, **DrawCircularArc** draws a 180-degree arc on the drawing page.


## Example

This Microsoft Visual Basic for Applications (VBA) macro shows how to use the **DrawCircularArc** method to draw an arc on the drawing page.


```vb
Public Sub DrawCircularArc_Example 
 
 Dim vsoShape As Visio.Shape 
 Set vsoShape = ActivePage.DrawCircularArc(3, 3, 3) 
 
End Sub
```

[!include[Support and feedback](~/includes/feedback-boilerplate.md)]