# Show stamps in the QuickIndex as a menu

#### Why This Option?

Displaying stamps in the QuickIndex as a menu provides users with a streamlined way to access and select different stamps without cluttering the interface. This option enhances user experience by allowing users to easily choose from various stamps when managing documents.

#### Functionality

The `ShowQuickCheckIconsSmall` property is controlled by the state of a corresponding checkbox in the user interface. When checked, stamps will be presented as a dropdown menu in the QuickIndex panel, enabling users to select their desired stamp efficiently.

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
*   **Example:** The user’s choice is saved through the following line of code:

    ```csharp
    csharpCode kopierenAppData.AppUserSettings.QuickIndexOptions.ShowQuickCheckIconsSmall = cbShowQuickCheckIconsSmall.Checked;
    ```

#### Error Handling

* If an error occurs during the execution of related settings or configurations, it is managed appropriately to prevent application crashes and maintain a smooth user experience.

***

**Link to the part of the code for this function**: [GitHub](https://github.com/topfact-AG/topfact6/blob/aee3a94d411bef87aad8b7910abea60216861305/topfact.MyWork/topfact.MyWork/Forms/Settings/frmUserSettings.cs#L259)\
**Link to the User Documentation**:[ ](https://services.topfact.de/wiki/pages/view?g=a011d893-d0d9-45d4-8337-510ee3ff2f6c)[topfactwiki](https://services.topfact.de/wiki/pages/view?g=aa9246cf-88be-417c-bd21-d6f610675d0f)
