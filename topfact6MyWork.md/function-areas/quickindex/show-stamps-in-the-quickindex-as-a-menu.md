# Show stamps in the QuickIndex as a menu

#### Why Use This Feature?

The `ShowQuickCheckIconsSmall` option allows users to customize the appearance of check icons in the QuickIndex area of the application, enhancing the user experience by accommodating personal preferences for icon size.

#### Functionality

The setting is configured when the user interacts with the `cbShowQuickCheckIconsSmall` checkbox. If checked, the QuickIndex will display smaller check icons; if unchecked, the icons will revert to their default size.

#### Description:

* **Property Binding:** The property is bound to the following setting in the user preferences:
  * **`AppData.AppUserSettings.QuickIndexOptions.ShowQuickCheckIconsSmall`**: This boolean value determines whether the small check icons are shown in the QuickIndex.
* **User Interface Element:**
  * **Checkbox:** `cbShowQuickCheckIconsSmall`
* **Behavior:**
  * **When Checked:**
    * If `cbShowQuickCheckIconsSmall.Checked` is true, the QuickIndex will display check icons in a smaller size.
  * **When Unchecked:**
    * If the checkbox is false, the check icons will display in their default size.
*   **Saving Preferences:** The user’s choice is saved through the following line of code:

    ```csharp
    csharpCode kopierenAppData.AppUserSettings.QuickIndexOptions.ShowQuickCheckIconsSmall = cbShowQuickCheckIconsSmall.Checked;
    ```

#### Popup Message

* A confirmation message may be displayed to inform the user that the settings have been applied successfully.

#### Error Handling

* If an error occurs during the execution of related settings or configurations, it is managed appropriately to prevent application crashes and maintain a smooth user experience.

***

**Link to the part of the code for this function**: [GitHub](https://github.com/topfact-AG/topfact6/blob/aee3a94d411bef87aad8b7910abea60216861305/topfact.MyWork/topfact.MyWork/Forms/Settings/frmUserSettings.cs#L259)\
**Link to the User Documentation**:[ ](https://services.topfact.de/wiki/pages/view?g=a011d893-d0d9-45d4-8337-510ee3ff2f6c)[topfactwiki](https://services.topfact.de/wiki/pages/view?g=aa9246cf-88be-417c-bd21-d6f610675d0f)
