# macOS エラー

> 18:24	Gradle sync failed: executing external native build for cmake /Users/ytabuchi/GitHub/KudanCV-Android-Demo/app/CMakeLists.txt (9 s 896 ms)
>   
> 18:24	NDK Resolution Outcome: Project settings: Gradle model version=UNKNOWN, NDK version=15.2.4203891

"clang" と "id" が開けないとのエラーが出る場合は、「設定＞セキュリティとプライバシー＞一般」で以下のように許可する必要がある。

## Samsung SC-02M (Galaxy A20 (Android 9)) でのエラー

Pixel 2 (Android 10), Galaxy S8 (Android 9) では発生しない。要調査。

```sh
2020-02-17 18:57:32.257 29804-29804/? E/Zygote: isWhitelistProcess - Process is Whitelisted
2020-02-17 18:57:32.260 29804-29804/? E/Zygote: accessInfo : 1
2020-02-17 18:57:32.274 29804-29804/? I/.xlsoft.kudanc: Late-enabling -Xcheck:jni
2020-02-17 18:57:32.773 29804-29804/com.xlsoft.kudancv I/MultiWindowDecorSupport: updateCaptionType >> DecorView@d928d3e[], isFloating: false, isApplication: true, hasWindowDecorCaption: false, hasWindowControllerCallback: true
2020-02-17 18:57:32.774 29804-29804/com.xlsoft.kudancv D/MultiWindowDecorSupport: setCaptionType = 0, DecorView = DecorView@d928d3e[]
2020-02-17 18:57:32.887 29804-29804/com.xlsoft.kudancv D/OpenGLRenderer: Skia GL Pipeline
2020-02-17 18:57:32.945 29804-29804/com.xlsoft.kudancv E/SensorManager: sensor is null
2020-02-17 18:57:32.956 29804-29804/com.xlsoft.kudancv D/EmergencyMode: [EmergencyManager] android createPackageContext successful
2020-02-17 18:57:33.003 29804-29804/com.xlsoft.kudancv D/InputTransport: Input channel constructed: fd=62
2020-02-17 18:57:33.003 29804-29804/com.xlsoft.kudancv D/ViewRootImpl@dd19177[MainActivity]: setView = DecorView@d928d3e[MainActivity] TM=true MM=false
2020-02-17 18:57:33.030 29804-29804/com.xlsoft.kudancv D/SurfaceView: onWindowVisibilityChanged(0) true eu.kudan.ar.CameraSurfaceView{59761e4 V.E...... ......I. 0,0-0,0 #7f070078 app:id/surface_view} of ViewRootImpl@dd19177[MainActivity]
2020-02-17 18:57:33.081 29804-29804/com.xlsoft.kudancv D/ViewRootImpl@dd19177[MainActivity]: Relayout returned: old=[0,0][1560,720] new=[58,0][1560,720] result=0x7 surface={true 493331861504} changed=true
2020-02-17 18:57:33.118 29804-29804/com.xlsoft.kudancv D/SurfaceView: show() Surface(name=SurfaceView - com.xlsoft.kudancv/eu.kudan.ar.MainActivity@59761e4@0[29804])/@0xa1e6502 eu.kudan.ar.CameraSurfaceView{59761e4 V.E...... ......ID 0,0-1406,1054 #7f070078 app:id/surface_view}
2020-02-17 18:57:33.120 29804-29860/com.xlsoft.kudancv I/ConfigStore: android::hardware::configstore::V1_0::ISurfaceFlingerConfigs::hasWideColorDisplay retrieved: 0
2020-02-17 18:57:33.120 29804-29860/com.xlsoft.kudancv I/ConfigStore: android::hardware::configstore::V1_0::ISurfaceFlingerConfigs::hasHDRDisplay retrieved: 0
2020-02-17 18:57:33.121 29804-29860/com.xlsoft.kudancv I/OpenGLRenderer: Initialized EGL, version 1.4
2020-02-17 18:57:33.121 29804-29860/com.xlsoft.kudancv D/OpenGLRenderer: Swap behavior 2
2020-02-17 18:57:33.133 29804-29860/com.xlsoft.kudancv D/mali_winsys: EGLint new_window_surface(egl_winsys_display *, void *, EGLSurface, EGLConfig, egl_winsys_surface **, EGLBoolean) returns 0x3000
2020-02-17 18:57:33.133 29804-29860/com.xlsoft.kudancv D/OpenGLRenderer: eglCreateWindowSurface = 0x72d67dd600, 0x72dcded010
2020-02-17 18:57:33.135 29804-29804/com.xlsoft.kudancv D/SurfaceView: surfaceCreated 1 #8 eu.kudan.ar.CameraSurfaceView{59761e4 V.E...... ......ID 0,0-1406,1054 #7f070078 app:id/surface_view}
2020-02-17 18:57:33.138 29804-29804/com.xlsoft.kudancv I/CameraManagerGlobal: Connecting to camera service
2020-02-17 18:57:33.142 29804-29804/com.xlsoft.kudancv D/VendorTagDescriptor: addVendorDescriptor: vendor tag id 3854507339 added
2020-02-17 18:57:33.192 29804-29858/com.xlsoft.kudancv I/CameraDevice: CameraDevice Opened.
2020-02-17 18:57:33.193 29804-29804/com.xlsoft.kudancv D/SurfaceView: surfaceChanged (1406,1054) 1 #8 eu.kudan.ar.CameraSurfaceView{59761e4 V.E...... ......ID 0,0-1406,1054 #7f070078 app:id/surface_view}
2020-02-17 18:57:33.211 29804-29804/com.xlsoft.kudancv D/ViewRootImpl@dd19177[MainActivity]: Relayout returned: old=[58,0][1560,720] new=[58,0][1560,720] result=0x3 surface={true 493331861504} changed=false
2020-02-17 18:57:33.403 29804-29804/com.xlsoft.kudancv D/ViewRootImpl@dd19177[MainActivity]: MSG_RESIZED_REPORT: frame=[58,0][1560,720] ci=[0,0][96,0] vi=[0,48][96,0] or=2
2020-02-17 18:57:33.405 29804-29804/com.xlsoft.kudancv D/ViewRootImpl@dd19177[MainActivity]: MSG_WINDOW_FOCUS_CHANGED 1 1
2020-02-17 18:57:33.405 29804-29804/com.xlsoft.kudancv D/InputMethodManager: prepareNavigationBarInfo() DecorView@d928d3e[MainActivity]
2020-02-17 18:57:33.406 29804-29804/com.xlsoft.kudancv D/InputMethodManager: getNavigationBarColor() -855310
2020-02-17 18:57:33.419 29804-29804/com.xlsoft.kudancv D/InputMethodManager: prepareNavigationBarInfo() DecorView@d928d3e[MainActivity]
2020-02-17 18:57:33.419 29804-29804/com.xlsoft.kudancv D/InputMethodManager: getNavigationBarColor() -855310
2020-02-17 18:57:33.420 29804-29804/com.xlsoft.kudancv V/InputMethodManager: Starting input: tba=com.xlsoft.kudancv ic=null mNaviBarColor -855310 mIsGetNaviBarColorSuccess true , NavVisible : true , NavTrans : false
2020-02-17 18:57:33.421 29804-29804/com.xlsoft.kudancv D/InputMethodManager: startInputInner - Id : 0
2020-02-17 18:57:33.421 29804-29804/com.xlsoft.kudancv I/InputMethodManager: startInputInner - mService.startInputOrWindowGainedFocus
2020-02-17 18:57:33.456 29804-29826/com.xlsoft.kudancv D/InputTransport: Input channel constructed: fd=75
2020-02-17 18:57:33.486 29804-29804/com.xlsoft.kudancv D/ViewRootImpl@dd19177[MainActivity]: MSG_RESIZED_REPORT: frame=[58,0][1560,720] ci=[0,0][96,0] vi=[0,0][96,0] or=2
2020-02-17 18:57:33.488 29804-29804/com.xlsoft.kudancv D/InputMethodManager: prepareNavigationBarInfo() DecorView@d928d3e[MainActivity]
2020-02-17 18:57:33.489 29804-29804/com.xlsoft.kudancv D/InputMethodManager: getNavigationBarColor() -855310
2020-02-17 18:57:33.489 29804-29804/com.xlsoft.kudancv V/InputMethodManager: Starting input: tba=com.xlsoft.kudancv ic=null mNaviBarColor -855310 mIsGetNaviBarColorSuccess true , NavVisible : true , NavTrans : false
2020-02-17 18:57:33.489 29804-29804/com.xlsoft.kudancv D/InputMethodManager: startInputInner - Id : 0
2020-02-17 18:57:34.454 29804-29858/com.xlsoft.kudancv A/libc: Fatal signal 6 (SIGABRT), code -6 (SI_TKILL) in tid 29858 (BackgroundCamer), pid 29804 (.xlsoft.kudancv)
```

