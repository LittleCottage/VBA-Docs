---
title: Line.Width property (Access)
keywords: vbaac10.chm10334
f1_keywords:
- vbaac10.chm10334
ms.prod: access
api_name:
- Access.Line.Width
ms.assetid: 01bb11d8-2d82-c3d6-cf04-f30ed3259193
ms.date: 02/27/2019
ms.localizationpriority: medium
---


# Line.Width property (Access)

Gets or sets the width of the specified object in [twips](../language/glossary/vbe-glossary.md#twip). Read/write **Integer**.


## Syntax

_expression_.**Width**

_expression_ A variable that represents a **[Line](Access.Line.md)** object.


## Remarks

For report controls, you can set the **Width** property when you print or preview a report only by using a macro or an event procedure specified in a section's **OnFormat** event property setting.

You can't set this property for an object after the print process has started.

Microsoft Access automatically sets the **Width** property when you create or size a control or when you size a window in form Design view or report Design view.

The width of forms and reports is measured from the inside of their borders. The width of controls is measured from the center of their borders so that controls with different border widths align correctly. 

The margins for forms and reports are set in the **Page Setup** dialog box, available by choosing **Page Setup** on the **File** menu.



[!include[Support and feedback](~/includes/feedback-boilerplate.md)]