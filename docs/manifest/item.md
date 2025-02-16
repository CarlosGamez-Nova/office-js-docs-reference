---
title: Item element in the manifest file
description: Specifies an item in a menu.
ms.date: 03/29/2022
ms.localizationpriority: medium
---

# Item element

Specifies an item in a menu.

**Add-in type:** Task pane, Mail

**Valid only in these VersionOverrides schemas**:

- Task pane 1.0
- Mail 1.0
- Mail 1.1

For more information, see [Version overrides in the manifest](/office/dev/add-ins/develop/add-in-manifests#version-overrides-in-the-manifest).

**Associated with these requirement sets**:

- [AddinCommands 1.1](../requirement-sets/common/add-in-commands-requirement-sets.md) when the parent **\<VersionOverrides\>** is type Taskpane 1.0.
- [Mailbox 1.3](../requirement-sets/outlook/requirement-set-1.3/outlook-requirement-set-1.3.md) when the parent **\<VersionOverrides\>** is type Mail 1.0.
- [Mailbox 1.5](../requirement-sets/outlook/requirement-set-1.5/outlook-requirement-set-1.5.md) when the parent **\<VersionOverrides\>** is type Mail 1.1.

## Child elements

|  Element |  Required  |  Description  |
|:-----|:-----:|:-----|
|  [Label](#label)     | Yes |  The text for the menu item. |
|  [Supertip](supertip.md)  | Yes |  The supertip for the menu item.    |
|  [Icon](icon.md)      | No |  An image for the menu item.         |
|  [Action](action.md)    | Yes |  Specifies the action to perform. There can be only one **\<Action\>** child of an **\<Item\>** element.  |
|  [Enabled](enabled.md)    | No |  Specifies whether the menu item is enabled when the add-in launches.  |
|  [OverriddenByRibbonApi](overriddenbyribbonapi.md)      | No |  Specifies whether the menu item should appear on application and platform combinations that support custom contextual tabs. If used, it must be the *first* child element. |

### Label

Specifies the text for the button by means of its only attribute, **resid**, which can be no more than 32 characters and must be set to the value of the **id** attribute of a **\<String\>** element in the **\<ShortStrings\>** child of the [Resources](resources.md) element.

**Add-in type:** Task pane, Mail

**Valid only in these VersionOverrides schemas**:

- Task pane 1.0
- Mail 1.0
- Mail 1.1

For more information, see [Version overrides in the manifest](/office/dev/add-ins/develop/add-in-manifests#version-overrides-in-the-manifest).

**Associated with these requirement sets**:

- [AddinCommands 1.1](../requirement-sets/common/add-in-commands-requirement-sets.md) when the parent **\<VersionOverrides\>** is type Taskpane 1.0.
- [Mailbox 1.3](../requirement-sets/outlook/requirement-set-1.3/outlook-requirement-set-1.3.md) when the parent **\<VersionOverrides\>** is type Mail 1.0.
- [Mailbox 1.5](../requirement-sets/outlook/requirement-set-1.5/outlook-requirement-set-1.5.md) when the parent **\<VersionOverrides\>** is type Mail 1.1.

## Examples

For examples, see [Control of type Menu](control-menu.md).