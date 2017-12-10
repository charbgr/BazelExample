Bazel example
========================

This is a "hello world" example that uses a variety of Bazel features. There is
a backend server and a couple of front-end applications that use this backend,
including:

* an [Android application](#android-app)

To build these examples, you will need to
[install Bazel](http://bazel.io/docs/install.html).

Android application
-------------------

Once these are done, set up the android_sdk_repository rule in the WORKSPACE file,
following the instructions in the comments there.

You can build and install this application by connecting an Android emulator or
device via adb and running:

```
$ bazel build //android:android
$ bazel mobile-install //android
```
