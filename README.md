# SliceTime for Android Emulator #

SliceTime for Android enables use of Android programs with the SliceTime network emulation platform.

This is a fork of original Android emulator. Original repository can be found at [https://android.googlesource.com/platform/external/qemu](https://android.googlesource.com/platform/external/qemu).

For more info see [Android open source project](http://source.android.com/) and [Project SliceTime](http://www.comsys.rwth-aachen.de/research/projects/slicetime/).

## Modifications to android emulator ##

Two commands were added to android emulator console:

* `init_sync <host> <server_port> <client_port> <client_id>`
which pauses emulator, connects to slicetime synchronizer and starts listening for incoming run permissions. set client id and client port to different values on every emulator instance, otherwise they won't work on same machine.

* `stop_sync`
disconnects from synchronizer and resumes normal operation.

## Instructions ##

For user instructions you should see documentation in [SliceTime GitHub](https://github.com/mr-kimia/slicetime).

## Legal ##

Most of the Android system is Licensed under [Apache Software License, 2.0](http://www.apache.org/licenses/LICENSE-2.0).
Android emulator is based on QEMU which is a trademark of [Fabrice Bellard](http://bellard.org/). For licensing info see [QEMU license](http://wiki.qemu.org/License).
Original licenses apply to this fork.

