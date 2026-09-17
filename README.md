# Hotpoint Tools Tracker Android

This Android app reads shared tools and transfer history from Supabase. Public users have read-only access. The configured administrator can sign in and add, assign, transfer, release, edit, or remove records according to the database policies.

## Build the APK with GitHub

1. Upload this complete folder to a new GitHub repository, keeping `.github/workflows/build-apk.yml` in place.
2. Open the repository's **Actions** tab.
3. Select **Build Android APK**, then choose **Run workflow**.
4. When the build finishes, open it and download the `Hotpoint-Tools-Tracker-APK` artifact.
5. Extract the artifact to obtain `app-debug.apk`.

The debug APK is installable for testing. A Play Store or public production release should use a private release signing key stored as encrypted GitHub secrets.

## Security

The app contains only the Supabase publishable key. Never add the service-role key or database password. Database row-level security is the enforcement layer for administrator-only changes.
