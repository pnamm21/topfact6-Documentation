# Barcode

**Why barcode?** The method is triggered when the user clicks on the barcode link in the interface. It retrieves the selected row's data and opens the appropriate form to print or display the barcode.

**Functionality:** The `btnBarcode_LinkClicked` method handles the click event for the barcode link and initializes the printing or display of the barcode based on the selected row.

**Description:**

* **Parameters:**
  * `object sender`: The source of the event.
  * `DevExpress.XtraNavBar.NavBarLinkEventArgs e`: Contains the event data related to the link click.
* **Row Validation:** The method first checks if any row in `gridView1` is focused. If no row is selected (`FocusedRowHandle < 0`), the method returns early.
* **Value Retrieval:** It retrieves the value of the barcode field from the focused row. If the value is `null` or `DBNull.Value`, the method returns without further action.
* **Data Collection:** A dictionary (`items`) is created to store the values of the relevant fields in the focused row. The method iterates through the `DataForm.DataFormFields`, fetching the values for each field and adding them to the dictionary if they are not already present.
* **Form Display:**
  * If the `PrintDirect` option is enabled in `DataForm.BarcodeOptions`, a new instance of `frmPrintBarcode` is created with the necessary parameters, and it is displayed centered on the screen.
  * Otherwise, a new instance of `frmBarcode` is created and shown, also centered on the screen.

**Error Handling:** The method currently does not implement specific error handling. It is advisable to add error handling for potential issues when retrieving values or showing forms.

**Link to the part of the code for this function:** [Link](https://services.topfact.de/wiki/pages/page?pageid=35845\&g=99da3d7b-ddec-429a-b75e-5bcddea2c627)

**Link to the User Documentation:** [Link](https://services.topfact.de/wiki/pages/view?g=99da3d7b-ddec-429a-b75e-5bcddea2c627)
