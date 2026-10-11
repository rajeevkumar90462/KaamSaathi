KaamSaathi Android project — HTML OTP UI version

WHAT THIS PROJECT IS
- An Android Studio project that opens the current KaamSaathi HTML prototype inside an Android WebView.
- Includes the mobile OTP screen UI from KaamSaathi_HTML_OTP_Option.html.
- The OTP controls are only a demo UI at this stage. They do not send or verify real SMS messages.
- Job posts, profiles and applications are still stored locally in the browser storage on that phone. They are not synchronized with other users yet.

BUILD APK ON A COMPUTER
1. Extract this ZIP.
2. Open the extracted folder in Android Studio.
3. Let Gradle sync finish.
4. Choose Build > Build Bundle(s) / APK(s) > Build APK(s).
5. Debug APK output: app/build/outputs/apk/debug/app-debug.apk

BUILD APK WITHOUT A COMPUTER (CLOUD BUILD OPTION)
This project includes .github/workflows/build-apk.yml for GitHub Actions.
1. Create/sign in to a GitHub account in your mobile browser.
2. Create a new repository named KaamSaathi and upload the extracted project files/folders (including the hidden .github folder).
3. Open the repository's Actions tab and select “Build KaamSaathi APK”.
4. Tap “Run workflow”. Wait for the run to finish successfully.
5. Open the successful run and download the “KaamSaathi-debug-APK” artifact. Extract the downloaded artifact ZIP to get app-debug.apk.
Note: uploading folders from a phone browser can be awkward. Do not share passwords, OTPs, Firebase secrets, or private user data in the repository.

NEXT STEPS
1. Build and install the prototype APK, then test its screens.
2. Create a Firebase project and configure Phone Authentication.
3. Integrate real Firebase phone OTP and test it on a real Android phone.
4. Add Firestore and secure rules so job posts, profiles and applications sync between different phones.
5. Add testing, privacy/data deletion features and production security review before public launch.

IMPORTANT
- This ZIP is source code, not a compiled APK. No APK has been built or tested in this environment.
- Firebase OTP, cloud database sync, push notifications, admin tools and production security are not activated yet.
- Keep user contact details and sensitive IDs private. Do not launch publicly until authentication, database rules, privacy and deletion are implemented and tested.
