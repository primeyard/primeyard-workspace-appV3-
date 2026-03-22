# PrimeYard Workspace Flutter v3

This build fixes two issues from the earlier APK:

- uses `Prime.png` as the Android launcher icon source
- uses the same SHA-256 password hashing logic as the Workspace HTML app
- reads the shared Firebase document at `primeyard/sharedState`
- caches the shared state and users locally so sign-in can still work after a successful sync

## Build on GitHub

If `.github` does not appear when you upload from Windows, open the repo on GitHub and create `.github/workflows/build-apk.yml` manually, then paste the contents of `BUILD-APK-WORKFLOW.yml`.

# PrimeYard Workspace v2

Native Flutter rebuild for PrimeYard Workspace.

## Build on GitHub

1. Upload the contents of this folder to a GitHub repo root.
2. Open **Actions**.
3. Run **Build PrimeYard Workspace APK**.
4. Download the artifact.

## Default login

- Username: `admin`
- Password: `PrimeYard2025`

The app syncs with the same Firebase document used by the HTML workspace:
- collection: `primeyard`
- document: `sharedState`
