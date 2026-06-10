# Magida Flureadium Android Patch Notes

This fork is used by the Flutter reader spike/full app to avoid patching Flureadium inside the Pub cache.

## Changes

- Updated Android compile SDK to 36.
- Kept minSdk compatible with the app at 24.
- Enabled Java 17 compile options.
- Enabled core library desugaring.
- Added desugar_jdk_libs 2.1.5 where required.

## Reason

The stock Pub package caused Android dependency conflicts with newer Flutter/Android dependencies such as package_info_plus and wakelock_plus. Pub cache patching worked for the spike but is not production-safe.

## App environment

- Flutter 3.44.1 stable
- Dart 3.12.1
- Android SDK 36.1.0
- Real device tested: Android 12 API 31
