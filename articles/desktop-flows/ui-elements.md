---
title: UI elements and controls | Microsoft Docs
description: UI elements and controls
author: mariosleon
ms.service: power-automate
ms.subservice: desktop-flow
ms.topic: article
ms.date: 12/02/2020
ms.author: marleon
ms.reviewer:
search.app: 
  - Flow
search.audienceType: 
  - flowmaker
  - enduser
---
# Automate using UI elements

Actions under the **UI automation** group are designed to directly interact with windows and applications. To achieve this result without resorting to image recognition or absolute coordinates, Power Automate utilizes **UI elements** to identify windows and their elements.

## UI elements

When using a UI automation action, a UI element will have to be provided as input. You can add a new UI element either directly from the action properties, or from the UI elements pane on the right-hand side of the designer:

![The Press button in window action.](./media/ui-elements/ui-element-input.png)

To add an element to the flow, highlight it and press **Ctrl & Left click**:

![Capturing an UI element.](./media/ui-elements/capturing-ui-elements.png)

When finished, press **Done**. Any UI elements captured will be added to the UI elements pane.

To access the UI elements pane, select the **UI elements** tab on the right-hand side of the flow designer:

![The UI elements pane.](./media/ui-elements/access-ui-elements-pane.png)

Elements can be sorted alphabetically by selecting the **Sort** option. To remove all the UI elements that aren't used in any action, select the dots icon next to the **Sort** option and then select **Remove unused UI elements**.

To rename or delete UI elements, right-click on an item and select the appropriate function. 

To use a captured element in an action, simply select it from the drop-down list:

![Adding a UI elemen as input in an action.](./media/ui-elements/add-ui-element-as-input.png)


To find where the element is being used in the flow, right-click the element and select **Find usages**. The results will show the actions which use the it. Double-clicking on a result will highlight the action in the workspace.

![The option to find the usages of a UI element.](./media/ui-elements/ui-element-right-click.png)

## Element Types

Captured elements are divided into two main categories, based on the type of application they were captured from: **UI controls** and **Web controls**.

Any captured elements that are part of a web page displayed in a compatible web browser (Internet Explorer, Microsoft Edge, Firefox, Google Chrome) are automatically saved as web controls, and may be used as input to **Browser automation** actions. All other elements are considered UI controls, and may be used in the respective actions.

## Element properties

Manage an element’s selectors by right-clicking any UI element and selecting **Edit selector**. This brings up the Selector builder, where the selector can be edited with a visual editor.

![The visual selector builder.](./media/ui-elements/visual-selector-editor.png)

To manually enter the selector’s value, toggle off Visual editor, and the text value of the selector will become editable:

![The manual selector builder.](./media/ui-elements/manual-selector-editor.png)

[!INCLUDE[footer-include](../includes/footer-banner.md)]

