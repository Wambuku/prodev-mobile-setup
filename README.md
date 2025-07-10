Project Setup Documentation
1. Setup and Installation Process
Steps Followed:

Installed Node.js (LTS):
Downloaded from nodejs.org and verified with node -v.

Installed Expo CLI:


Edit
npm install -g expo-cli
Installed VS Code:
Downloaded and set up extensions for React Native & TypeScript.

Installed Expo Go:
Downloaded Expo Go app on my Android device from Expo Go.

Created New Expo Project:


Edit
npx create-expo-app@latest prodev-mobile-app-0x01
cd prodev-mobile-app-0x01
Started the Project:


Edit
npx expo start
Scanned the QR code using Expo Go on my device.

2. Issues Encountered and Solutions
Issue: Expo Go app could not connect to development server on first try.
Solution:

Made sure phone and computer were on the same WiFi network.

Disabled VPN and firewall temporarily.

Restarted Expo CLI and Expo Go app.

Issue: Slow initial install of npm dependencies.
Solution:

Checked my internet connection.

Waited a few extra minutes for dependencies to finish installing.

3. Project Scaffolding and File Structure
Default structure after running npx create-expo-app@latest:


Edit
prodev-mobile-app-0x01/
├── app/
│   ├── index.tsx
│   ├── (tabs)/
│   └── ...
├── assets/
│   ├── images/
│   └── ...
├── node_modules/
├── package.json
├── app.json
├── README.md
└── ...
app/index.tsx – Entry point for app UI

assets/ – Place for images, logos, backgrounds

package.json – Project dependencies

app.json – Expo config

4. Effects of Running reset-project
Command run:


Edit
npm run reset-project
Observations:

Removes node_modules and reinstalls all dependencies.

Resets any modifications to the project template, returning it to its original state.

Useful for troubleshooting if the project breaks or dependencies become out of sync.

After reset, the app starts up as a fresh template (all previous code changes lost if not committed).

