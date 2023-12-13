# WebApp

See also https://www.npmjs.com/package/nativescript

Start your development as follows, from within containers/app/webapp/:

```
$ ns preview
```

You will be presented with a QR code (in the GitPod Terminal window or the sidepanel), which you need to scan with your iOS device (iPhone or iPad, on which your previously installed the NativeScript preview App from the App Store).

You should now see the NativeScipt app on your iPhone or iPad, ready to monitor whilst developing further, as it will be synced.

In the Terminal window of GitPod you are able to monitor the communication between GitPod and your iOS device, like:

```
 i  ┌───────────────────────────────────────────┐
 i  ├─ {N} NativeScript Preview 2.0 [v1.0.12] ──┤
 i  └───────────────────────────── Public Beta ─┘
┃   ========= A QR CODE IS SHOWN HERE ============
 i  Scan the above QR code with your device to connect to this session.
 i  Scanning can be done with the default camera app on iOS or any other application capable of scanning QR codes.
 i  
 i  This CLI is interactive, you can press the following keys any time (make sure the terminal has focus):
 i  
 i    [R] - restart the Preview app on all connected devices
 i    [S] - reset the Preview app on all connected devices
 i    [O] - open the Web UI to scan the QR code
 i  
 i  Waiting for device connections...
 i  Device connected:    iPhone (158) [ios: 2.0.8 (1)]
✔ Building for ios
  Compiled successfully in 452.50ms
 ...
 i  Build complete. Uploading files...
 i  Upload complete. Applying changes on connected devices...
 iPhone (158)  14:08:33 [HMR][ee7bd0985d3e39f144c5] success | Successfully applied update.
 i  Device disconnected: iPhone (158) [ios: 2.0.8 (1)]
 i  Device connected:    iPhone (158) [ios: 2.0.8 (1)]
 iPhone (158)  14:09:02 39 taps left
 i  Device disconnected: iPhone (158) [ios: 2.0.8 (1)]
```