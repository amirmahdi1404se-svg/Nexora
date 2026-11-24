# NEXORA

A futuristic personal digital environment built with Flutter.

## Version 1.0 starter

Included:
- Futuristic dark dashboard and custom orb illustration
- Bottom navigation
- Workspace overview
- Offline demo chat interface
- Persistent offline preference
- GitHub Actions Android APK workflow

## Build locally

Install Flutter and Android SDK, then:

```bash
flutter pub get
flutter analyze
flutter test
flutter build apk --release
```

APK output:

`build/app/outputs/flutter-apk/app-release.apk`

## Build using GitHub

1. Create a Flutter project in a GitHub repository (or upload this source).
2. Ensure the repository contains the `.github/workflows/android.yml` workflow.
3. Push to the `main` branch.
4. Open the Actions tab and wait for the workflow.
5. Download `NEXORA-Android-APK` from the workflow run's Artifacts section.

The workflow creates the Android platform project using Flutter's generated project files.
If the repository was not created from `flutter create`, run `flutter create . --platforms=android` in a Codespace and commit the generated Android folder.

## Important scope notes

This is a functional UI and architecture starter, not the complete product yet.
The AI screen currently uses an offline demonstration response. Add a secure backend
before connecting a real AI provider. Never embed private API keys in the APK.
Cloud sync, real file operations, extension sandboxing, and full workspace editing
are planned for later milestones.
