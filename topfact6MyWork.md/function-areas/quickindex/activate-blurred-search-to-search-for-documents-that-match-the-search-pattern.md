# Enhancing blurred Document Search

#### **Why this option?**

The **blurred search** option is designed to help users find documents even if the search term isn’t an exact match. This improves search results and saves time.

#### **Functionality:**

Blurred search lets the system find documents that contain the search term, not just those with exact matches. For example, searching "invoice" will also show "incoming invoice."

***

#### **Description:**

In the program, blurred search is controlled by specific user settings. The main setting, `cbSearchWithLike.Checked`, activates the blurred search function. When this option is enabled, the system searches for documents containing the search term, even if the words aren't exact. For instance, if you search for "Rechnung," the system will also find "Eingangsrechnung" or "Rechnung 2023."

Additional settings, like `cbSearchSuggestions.Checked`, improve the search experience by offering suggestions as you type, making it easier to find the right document. Other settings, such as `ddlTreeFindBehavior` and `ddlGridFindBehavior`, allow users to customize how searches are performed in different parts of the interface, like trees or grids.

Furthermore, there are options to control the display of document-related icons (`cbShowArchiveIconsSmall.EditValue`) and how filters behave when loading new data (`cbClearFilter.EditValue`). These improve how documents are displayed and managed in the system.

All of these settings work together to create a flexible and user-friendly document search system, where blurred search plays a key role in helping users find documents more easily and efficiently.

**Link to the part of the code for this function**: [GitHub](https://github.com/topfact-AG/topfact6/blob/aee3a94d411bef87aad8b7910abea60216861305/topfact.MyWork/topfact.MyWork/Forms/Settings/frmUserSettings.cs#L95C2-L118C79)\
**Link to the User Documentation**:  [topfactwiki](https://services.topfact.de/wiki/pages/page?pageid=35821\&g=d3f90d36-46cb-40b0-9b9b-54029a612494)

