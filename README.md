**APK**
`iq.ihec.pcosqrreportview`

---

### **1002 Updates (ver 1.3)**
1.  Password removed.
2.  For Android: PDFs are now saved to the device's "Download" folder.
    * You **must tap 'Allow'** on the permission prompt immediately after scanning for the PDF file to be saved to the Download folder and appear in the viewer.
1-2. For iPhone: PDFs are saved in "My Documents" (within the app's 'Files' directory).
2.  PDF file naming convention: `PSNumber_YYYYMMDD_HHMMSS.pdf`
    * Example: `PS10522003_20251001_173954.pdf`
3.  Arabic text correction:
    * "Next PS" -> `المحطة التالية`

---

### **1001 Updates**
* Improved recognition rate by implementing the Scandit SDK.

---

### **0922 Updates**
1.  Fixed an issue where buttons were obscured when using Gesture Navigation or 3-button mode.
2.  Version number is now displayed on the QR Code Scan screen.
    * Per app policy, only two decimal places are displayed (e.g., `1.0` -> `ver 1.0`).

**Android Specifics**
* **Android 9 and below:** The viewer button is elevated by the height of the soft-bar.
* **Android 10 and above (with Gesture Navigation or 3-button mode):** Fixed the issue of obscured buttons.
    * On "Restart," the app screen automatically adjusts to prevent overlapping with buttons. This may create vertical spacing between the button area and the navigation bar.

**iOS**
*(No specific notes)*

---

### **0915 Updates**
* Removed the "Polling Station (PS) Number" input screen.
* Removed PS numbers that were previously displayed on reports and screens.
* **QR Scan Status Display:**
    * When scanning, if the QR Code has already been scanned, the reticle color will change to yellow.
    * -> Previously read QRs are de-duplicated and will not be scanned again.
* **Added "Restart" / "Exit" Buttons:**
    * After all QR codes are successfully scanned and the report is generated, a "Restart" button will appear at the very bottom of the screen.

---

### **PCOS QR Report Viewer App User Manual**

*(Original App Flow: App Launch -> Enter Password -> Enter PS Number -> QC Scan -> Camera permission "Allow" prompt (First time only))*

**Step 1: Enter Password**
* `316223900`
*(Note: Changelog indicates this step was removed in `v1.3`)*

**Step 2: Scan QR Code**
* After authentication, the camera screen for scanning QR codes will appear. Align the QR code within the square frame in the center of the screen.
* Upon a successful scan, the reticle will turn green, and a success message (`تم المسح بنجاح!`) will briefly appear at the bottom.

**Step 3: Check Scan Result and Proceed to Next Scan**
* After successfully scanning one QR code, you will be taken to an intermediate results screen.

**Intermediate Results Screen**
* You can see an image of the just-scanned QR code in the center of the screen.
* At the bottom, you can see the overall scan progress (e.g., `1 من أصل 3` → 1 of 3 scans complete).
* Press the purple `المسح التالي` (Next Scan) button to return to Step 2 and scan the next QR code.
* Repeat Steps 2 and 3 until all required QR codes are scanned.

**Step 4: Generate Final Report**
* After the last QR code is successfully scanned, the app will automatically begin generating the final report. Please wait a moment.
* A loading screen will be displayed during report generation.

**Step 5: Review Final Report**
* Once the report is generated, the final result report will be displayed on the screen. You can scroll up and down to review the entire document.

---

### **Troubleshooting: How to Reset the App**

If you encounter a problem, such as an app password error, you can reset the app using the following method:

1.  On your Home Screen, **press and hold** the 'PcosQrReportView' app icon.
2.  From the small menu that appears, tap the **"Info icon (ⓘ)"** (`أيقونة المعلومات`).
3.  On the 'App Info' screen, select the **"Storage"** (`التخزين`) menu.
4.  Tap **"Clear cache"** (`مسح ذاكرة التخزين المؤقت`) and then **"Clear data"** (`مسح البيانات`) to reset the app.
