# WebApp

See also https://www.npmjs.com/package/nativescript

Start your development as follows, from within containers/app/webapp/:

```
$ ns preview
```

You will be presented with a QR code, which you need to scan with your iOS device (iPhone or iPad, on which your previously installed the NativeScript preview App from the App Store).

You should now see the NativeScipt app on your iPhone or iPad, ready to monitor whilst developing further, as it will be synced.

In the console of GitPod you are able to monitor the communication between GitPod and your iOS device, like:

```
✔ Building for ios
  Compiled successfully in 452.50ms

 i  Build complete. Uploading files...
 i  Upload complete. Applying changes on connected devices...
 iPhone (158)  14:08:33 [HMR][ee7bd0985d3e39f144c5] success | Successfully applied update.
 i  Device disconnected: iPhone (158) [ios: 2.0.8 (1)]
 i  Device connected:    iPhone (158) [ios: 2.0.8 (1)]
 iPhone (158)  14:09:02 39 taps left
 i  Device disconnected: iPhone (158) [ios: 2.0.8 (1)]
```