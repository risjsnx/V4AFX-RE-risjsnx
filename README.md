# ViPERFX_RE
> [!NOTE]
> this module is based on WSTxda's module with a few tweaks, so please support WstXDA for it's work 

This is a reverse-engineering project aimed to make ViPER4Android more easy to access, modify, and improve.
Some QOL changes have been made, such as processing audio as float32, removing unused code, using more modern libraries, etc.
To view the progress, see [Issue #2 (old/unused)](https://github.com/AndroidAudioMods/ViPERFX_RE/issues/2)

# Building

- Install the NDK, CMake and Make.
- Run `cmake . -DCMAKE_TOOLCHAIN_FILE=<NDKROOT>/build/cmake/android.toolchain.cmake -DANDROID_ABI=<ABI>` where <NDKROOT> is where you installed the NDK and <ABI> is the target ABI to build for.
- Run `make`
- You should now find a `libv4afx_r.so` file in your project root.

# CLion

Make sure to install `ninja`
In CLion, make sure to set the following custom arguments: `-DCMAKE_TOOLCHAIN_FILE=<NDKROOT>/build/cmake/android.toolchain.cmake -DANDROID_ABI=<ABI> -G Ninja`
Then you can build the project with `ninja` instead of `make`

# Credits

Zhuhang and ViPER520 for making ViPER4Android
Martmists and Iscle for reverse-engineering
