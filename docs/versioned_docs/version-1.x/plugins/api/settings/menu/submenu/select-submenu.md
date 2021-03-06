---
title: SelectSubmenu
sidebar_label: SelectSubmenu
---

**Type:** `Component`

Extends the base [submenu](./submenu.md) with a list of radio buttons.

## Props

### `title`

**Type:** `string|null` | **Default:** `null`

The title for the control that is responsible for showing/hiding the menu.

### `value`

**Type:** `any` | **Default:** `null`

The value of the currently selected radio button.

### `options`

**Type:** `any[]` | **Default:** `[]`

List of objects, where each `object` is a set of `MenuItemRadio` [props](../menu-item-radio.md#props).

### `emptyHint`

**Type:** `string|null` | **Default:** `''`

The `hint` text to be used if there are no options.

### `isActive`

**Type:** `boolean` | **Default:** `false`

Whether the menu is visible or not.

### `isEnabled`

**Type:** `boolean` | **Default:** `true`

Whether the menu and controller should be rendered in the DOM or not.

### `isLocked`

**Type:** `boolean` | **Default:** `false`

Whether the menu is rendered or not. The menu controller responsible for opening/closing the 
submenu is visible.

### `hideController`

**Type:** `boolean` | **Default:** `false`

Whether to hide the menu controller or not.

## Methods

### `getSubmenu`

**Return Type:** [`Submenu`](./submenu.md)

The underlying `Submenu` instance.

### `getMenuOptions`

**Return Type:** [`MenuOptions`](../menu-options.md)

The underlying `MenuOptions` instance.

## Events

### `open`

**Data Type:** `undefined`

Fired when the menu becomes visible.

### `close`

**Data Type:** `undefined`

Fired when the menu becomes hidden.

### `valuechange`

**Data Type:** `any`

Fired when a radio button is clicked. The event data contains the radio's respective value.