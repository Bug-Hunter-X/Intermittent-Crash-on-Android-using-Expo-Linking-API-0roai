# Expo Linking API Crash on Android

This repository demonstrates a bug encountered when using the Expo `Linking` API to open URLs in external apps on Android. The app successfully opens the external URL, but then crashes immediately afterward.  The crash is not consistent, making debugging challenging.  This issue only appears on Android; iOS functionality is unaffected.

## Steps to Reproduce

1. Clone this repository.
2. Run the app on an Android emulator or device.
3. Tap the button to open the external URL.
4. Observe that the external app opens but the Expo app crashes shortly after.

## Potential Causes

The root cause is currently unknown, but it is suspected to be related to how Expo handles background processes and inter-app communication on Android.

## Workaround (Partial)

While a complete solution is still pending, a possible mitigation involves delaying the post-linking operation. This is not a permanent fix, but it might reduce the frequency of the crash.  See `LinkingBugSolution.js` for an example of this workaround.

## Further Investigation

More investigation is needed to determine the exact cause and provide a more robust solution.  Please report any findings or helpful suggestions!