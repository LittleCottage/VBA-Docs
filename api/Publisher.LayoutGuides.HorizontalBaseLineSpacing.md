---
title: LayoutGuides.HorizontalBaseLineSpacing property (Publisher)
keywords: vbapb10.chm1114132
f1_keywords:
- vbapb10.chm1114132
ms.prod: publisher
api_name:
- Publisher.LayoutGuides.HorizontalBaseLineSpacing
ms.assetid: 19899a25-c1a5-9c81-f022-d842a3d6c7d8
ms.date: 06/08/2019
ms.localizationpriority: medium
---


# LayoutGuides.HorizontalBaseLineSpacing property (Publisher)

Returns a **Single** that represents the horizontal baseline spacing of the specified **LayoutGuides** object. Read/write.


## Syntax

_expression_.**HorizontalBaseLineSpacing**

_expression_ A variable that represents a **[LayoutGuides](Publisher.LayoutGuides.md)** object.


## Return value

Single


## Remarks

When setting the layout guide properties of a **Page** object, it must be returned from the **MasterPages** collection.


## Example

This example sets the horizontal baseline spacing of the **LayoutGuides** object to 20 for the second master page in the active document.

```vb
Dim objLayout As LayoutGuides 
Set objLayout = ActiveDocument.MasterPages(2).LayoutGuides 
objLayout.HorizontalBaseLineSpacing = 20 

```

[!include[Support and feedback](~/includes/feedback-boilerplate.md)]