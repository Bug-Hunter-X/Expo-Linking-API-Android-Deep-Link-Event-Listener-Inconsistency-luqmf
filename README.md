# Expo Linking API Android Deep Link Issue

This repository demonstrates a bug in Expo's `Linking` API on Android where the `Linking.addEventListener` for deep links does not always fire when the app is already running.  The problem is that while `Linking.getInitialURL()` works correctly on app launch, it fails to catch deep links while the application is in the foreground. 

The `bug.js` file showcases the issue; the `bugSolution.js` provides a workaround.