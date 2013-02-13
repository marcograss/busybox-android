Busybox for Android, Statically Linked
====================================================

Compiling yourself
------------------
It should be pretty easy to recompile the binary yourself by following these
steps:

1. Get and install the latest GNU/Linux toolchain from [here]
(http://www.codesourcery.com/sgpp/lite/arm/portal/subscription?@template=lite)
(unless you already have a working toolchain installed). Make sure the binaries
directory is in your PATH.
2. Get and unpack the latest source for Busybox.
3. Apply `busybox-android.patch` from the git repo to Busybox source if you
want to be able to use the profile and history under Android.
4. Copy `busybox-android.config` from the git into Busybox's source root and
rename it to `.config`. Edit it and make sure `CONFIG_CROSS_COMPILER_PREFIX` is
correctly set to your compiler's name.
5. Run `make` and you should obtain the `busybox` binary.

