# Week 4: Your Heroes on your Phone :iphone:

## Day 1: Go Mobile :busstop:
Put your app on your phone!
 - Install the NativeScript command line interface
   ```
   sudo npm install --global nativescript
   ```
 - Add NativeScript to your app
   ```
   npm install --save-dev @schematics/angular@9.1.8
   ng add @nativescript/schematics
   ```
 - Run your app to check that it still works as before in the web browser
 - Build the NativeScript app
   ```
   tns preview
   ```
   - This will display a QR code on your screen
 - To preview your app on your phone, you need to install two companion apps on your Android/iOS device(s):
   - NativeScript Playground ([Android](https://play.google.com/store/apps/details?id=org.nativescript.play), [iOS](https://apps.apple.com/us/app/nativescript-playground/id1263543946)) — used to scan a QR code provided by the NativeScript CLI
   - NativeScript Preview ([Android](https://play.google.com/store/apps/details?id=org.nativescript.preview), [iOS](https://apps.apple.com/us/app/nativescript-preview/id1264484702) — used to host display your app
 - Scan the QR code with the NativeScript Playground app, which will connect your project with the NativeScript Preview app
 - As always commit and synchronize your changes
