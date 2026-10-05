# MIHIR AI v0.20 — Android Testing Mode

This build is for UI/workflow testing without paid provider credentials.

- Open `index.html` in a browser, or serve this folder over HTTP/HTTPS.
- Demo mode mocks OpenAI, D-ID, Razorpay, Supabase and generation endpoints.
- No real payment is processed.
- Free Trial can be simulated; paid plans intentionally return a payment-disabled message.
- Avatar/voice profiles remain demo-pending and do not create real clones.
- Demo credits are stored only in browser localStorage.

## Android packaging
`android/` contains a WebView project source. This environment does not include the Android SDK/Gradle toolchain, so an APK cannot be honestly claimed as compiled here. Open the Android project in Android Studio and build the debug APK.
