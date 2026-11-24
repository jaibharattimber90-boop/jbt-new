JAI BHARAT TIMBERS - SmartDesk Android project

This is an Android Studio project wrapping the supplied SmartDesk web application.
The existing billing UI, calculations, modules and localStorage data logic are retained.

Android-specific handling:
- Android WebView with DOM storage for app records/drafts.
- Print Invoice opens Android's system print dialog; select Save as PDF.
- WhatsApp opens a pre-filled message containing invoice number and total.
- PDF file picker is enabled for the existing PDF bill import.

Known limitation in the supplied upload:
- server.js is empty, so the original desktop Cloudinary PDF-upload backend is not present.
- Android WhatsApp sharing therefore sends invoice summary text; it does not attach a cloud PDF link.
- Save the PDF separately using Print Invoice > Save as PDF.

Build:
1. Open this folder in Android Studio.
2. Let Android Studio install the Android SDK and Gradle components it requests.
3. Select Build > Build Bundle(s) / APK(s) > Build APK(s).
4. Debug APK: app/build/outputs/apk/debug/app-debug.apk

Application ID: com.jaibharat.smartdesk
Minimum Android version: 6.0 (API 23)
