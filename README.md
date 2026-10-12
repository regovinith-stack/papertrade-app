# PaperTrade APK
## Easiest (no computer tools): GitHub
1. Create a new GitHub repo, upload ALL files in this folder (keep .github/workflows/build.yml).
2. Repo > Actions > "Build APK" > Run workflow (it also runs on push).
3. When done, open the run > Artifacts > PaperTrade-apk > download, unzip, install app-debug.apk.
## Locally (needs Node 18+, JDK 17, Android SDK)
npm install && npx cap add android && npx cap sync android
cd android && ./gradlew assembleDebug
APK: android/app/build/outputs/apk/debug/app-debug.apk
