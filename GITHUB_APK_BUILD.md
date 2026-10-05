# MIHIR AI — Direct APK Build

This project includes a GitHub Actions workflow that builds a directly installable Android debug APK.

## Steps
1. Create a new GitHub repository.
2. Upload the contents of this folder to the repository root.
3. Push to the `main` branch.
4. Open **Actions → Build MIHIR AI APK**.
5. After the workflow succeeds, open the workflow run and download the artifact **mihir-ai-v0.20-testing-apk**.
6. Extract `app-debug.apk` and install it on the Android phone.

No Supabase, OpenAI, D-ID or Razorpay credentials are required for this testing build.
