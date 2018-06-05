---
title: Hot Key Control (MSAA UI Element Reference)
description: Hot key controls allow users to enter a combination of keystrokes used as a hot key, which enables them to perform an action quickly. A hot key control displays the keystrokes entered by the user and ensures that the user selects a valid key combination.
ms.assetid: 56c9fee4-f3d3-4f61-8587-bf80186aa5b3
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# Hot Key Control (MSAA UI Element Reference)

Hot key controls allow users to enter a combination of keystrokes used as a hot key, which enables them to perform an action quickly. A hot key control displays the keystrokes entered by the user and ensures that the user selects a valid key combination.

The window class name for a hot key control is HOTKEY\_CLASS, which is defined as "msctls\_hotkey32" in Commctrl.h.

## IAccessible Methods

Hot key controls support the following [**IAccessible**](/windows/desktop/api/oleacc/nn-oleacc-iaccessible) methods:

-   [**accHitTest**](/windows/desktop/api/Oleacc/nf-oleacc-iaccessible-acchittest)
-   [**accLocation**](/windows/desktop/api/Oleacc/nf-oleacc-iaccessible-acclocation)
-   [**accNavigate**](/windows/desktop/api/Oleacc/nf-oleacc-iaccessible-accnavigate)
-   [**accSelect**](/windows/desktop/api/Oleacc/nf-oleacc-iaccessible-accselect)

## IAccessible Properties

The Hot key controls support the following [**IAccessible**](/windows/desktop/api/oleacc/nn-oleacc-iaccessible) properties:



| Property                                                                             | Comments                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
|--------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [**get\_accChildCount**](/windows/desktop/api/Oleacc/nf-oleacc-iaccessible-get_accchildcount)             | The **ChildCount** property is always zero.                                                                                                                                                                                                                                                                                                                                                                                                                              |
| [**get\_accFocus**](/windows/desktop/api/Oleacc/nf-oleacc-iaccessible-get_accfocus)                       |                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| [**get\_accKeyboardShortcut**](/windows/desktop/api/Oleacc/nf-oleacc-iaccessible-get_acckeyboardshortcut) | The **KeyboardShortcut** property is the hot key control's access key, which is an underlined character in the text of the hot key control's label. The returned string contains the access key character appended to the string "Alt+".                                                                                                                                                                                                                                 |
| [**get\_accName**](/windows/desktop/api/Oleacc/nf-oleacc-iaccessible-get_accname)                         | The **Name** property is the text from a static text control that labels the hot key control.                                                                                                                                                                                                                                                                                                                                                                            |
| [**get\_accParent**](/windows/desktop/api/Oleacc/nf-oleacc-iaccessible-get_accparent)                     | The **Parent** property is a window ( [**ROLE\_SYSTEM\_WINDOW**](https://www.bing.com/search?q=**ROLE\_SYSTEM\_WINDOW**) ) that surrounds the control and has the same **Name** property and window class name as the control.                                                                                                                                                                                                                                                              |
| [**get\_accRole**](/windows/desktop/api/Oleacc/nf-oleacc-iaccessible-get_accrole)                         | The **Role** property is [**ROLE\_SYSTEM\_HOTKEYFIELD**](https://www.bing.com/search?q=**ROLE\_SYSTEM\_HOTKEYFIELD**).                                                                                                                                                                                                                                                                                                                                                                      |
| [**get\_accState**](/windows/desktop/api/Oleacc/nf-oleacc-iaccessible-get_accstate)                       | The **State** property is a combination of one or more of the following [values](object-state-constants.md):[**STATE\_SYSTEM\_INVISIBLE**](https://www.bing.com/search?q=**STATE\_SYSTEM\_INVISIBLE**) \| [**STATE\_SYSTEM\_UNAVAILABLE**](https://www.bing.com/search?q=**STATE\_SYSTEM\_UNAVAILABLE**) \| [**STATE\_SYSTEM\_FOCUSED**](https://www.bing.com/search?q=**STATE\_SYSTEM\_FOCUSED**) \| [**STATE\_SYSTEM\_FOCUSABLE**](https://www.bing.com/search?q=**STATE\_SYSTEM\_FOCUSABLE**)<br/> |
| [**get\_accValue**](/windows/desktop/api/Oleacc/nf-oleacc-iaccessible-get_accvalue)                       | The **Value** property is a string that contains the text in the hot key field.                                                                                                                                                                                                                                                                                                                                                                                          |



 

## Related topics

<dl> <dt>

[IAccessible Interface](/windows/desktop/api/oleacc/nn-oleacc-iaccessible)
</dt> </dl>

 

 




