# QuickIndexReset

**Why reset?** The window parameters for QuickIndex are outside a usable range and need to be reset. The document is not displayed!

**Functionality:** The `btnResetQuickIndex_Click` method is triggered when the user clicks the 'Reset QuickIndex' button to reset the QuickIndex settings.

**Description:**

* **Registry Paths:** Two paths to the registry keys are defined:
  * `keyName`: Path to `Software\pro effectus\topfact6 MyWork\DockManager`.
  * `keyName2`: Path to `Software\topfact\topfact6 MyWork\DockManager`.
* **Opening and Deleting Keys:** The method attempts to open the registry keys in the current user's area. If the key exists, the subkey `frmQuickIndex` and its contents are deleted.
* **Popup Message:** After resetting, a message appears: "The QuickIndex settings have been reset."
* **Error Handling:** If an error occurs, it is suppressed in the `catch` block, without showing a specific error message.

***

**Link to the part of the code for this function**: [GitHub](https://github.com/topfact-AG/topfact6/blob/97253914e8f78c153a791c816fd44a15f42987ed/topfact.MyWork/topfact.MyWork/Forms/Settings/frmUserSettings.cs#L378)\
**Link to the User Documentation**:[ ](https://services.topfact.de/wiki/pages/view?g=a011d893-d0d9-45d4-8337-510ee3ff2f6c)[topfactwiki](https://services.topfact.de/wiki/pages/view?g=60448220-ae05-4bcc-9b05-f1d6f1fc058d)

***
