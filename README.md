# Expo CLI Error: React Native/Expo SDK Version Mismatch

This repository demonstrates a common Expo CLI error stemming from incompatibility between the Expo SDK version and the versions of React Native or its dependencies.  The `bug.js` file shows an example of code that might trigger this error (though the specific trigger will vary depending on the incompatibility). The `bugSolution.js` demonstrates solutions.

## Steps to Reproduce

1.  Clone this repository.
2.  Follow instructions to install and run the example in `bug.js`. (You'll likely need to modify package.json to trigger the error)
3.  Observe the error message.
4.  Apply the solutions in `bugSolution.js` to resolve the issue.

## Solutions

- **Upgrade Expo SDK:**  Use `expo upgrade` to update to the latest stable Expo SDK.
- **Check Package.json:** Examine dependencies for version conflicts; use npm-check-updates or yarn upgrade to check for updates
- **Clean and Rebuild:** Sometimes, a clean reinstall of your project can resolve dependency issues. Try deleting the `node_modules` folder and reinstalling all dependencies.
- **Specify React Native Version:** Ensure the React Native version in your `package.json` is compatible with your Expo SDK version.