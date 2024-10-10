# Automatically save changes to index data in the QuickIndex

**Why this option?**\
The "Close" button in the QuickIndex panel provides users with a convenient way to close the QuickIndex view. However, not all users may need this button visible at all times. This option allows the user to hide or show the "Close" button based on their preference.

**Functionality**:\
The `ShowQuickIndexCloseButton` property is controlled by the state of the `cbShowQuickIndexCloseButton` checkbox in the user interface. If checked, the "Close" button will appear in the QuickIndex view, providing quick access to closing it.

**Description:**

* **UI Element**:
  * Checkbox: `cbShowQuickIndexCloseButton`
  * Path: Appears on the application's settings page under QuickIndex options.
* **Property Binding**:
  * The checkbox state (`Checked` or not) is assigned to the `AppData.AppUserSettings.MyWorkOptions.ShowQuickIndexCloseButton` property.
* **Visibility Control**:
  * When `ShowQuickIndexCloseButton` is set to `true`, the QuickIndex view will display a "Close" button.
  * If set to `false`, the "Close" button is hidden from the QuickIndex interface.
* **Behavior**:
  * This setting is part of the user’s customizable preferences. It allows toggling the "Close" button based on individual workflow needs.

**Example:**

After saving this setting, the QuickIndex section will either show or hide the close button based on the user’s preference.

```csharp
AppData.AppUserSettings.MyWorkOptions.ShowQuickIndexCloseButton = cbShowQuickIndexCloseButton.Checked;
```

***

**Link to the part of the code for this function**: [GitHub](https://github.com/topfact-AG/topfact6/blob/aee3a94d411bef87aad8b7910abea60216861305/topfact.MyWork/topfact.MyWork/Forms/Settings/frmUserSettings.cs#L264) \
**Link to the User Documentation**:[ ](https://services.topfact.de/wiki/pages/view?g=a011d893-d0d9-45d4-8337-510ee3ff2f6c)[topfactwiki](https://services.topfact.de/wiki/pages/view?g=a011d893-d0d9-45d4-8337-510ee3ff2f6c)

***
