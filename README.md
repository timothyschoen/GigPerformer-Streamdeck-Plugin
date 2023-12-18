# Stream Deck extension for GigPerformer

<img width="1240" alt="Screenshot 2023-11-01 at 18 23 36" src="https://github.com/timothyschoen/GigPerformer-Streamdeck/assets/44585538/4f4c414c-bf2c-4f6a-afc0-5a5e78756ae7">


<br>

# Note

Source code is down for now, but will be back up soon!

# Build instructions

```
git clone https://github.com/timothyschoen/GigPerformer-Streamdeck.git
cd GigPerformer-Streamdeck
mkdir build && cd build
cmake .. (the generator can be specified using -G"Unix Makefiles", -G"XCode" or -G"Visual Studio 16 2019" -A x64)
cmake --build .
```

This will build both of the extensions and install them as well.

Note that with recent versions of the Stream Deck app, it will not allow you to copy extensions to the extensions folder, it will only allow the installation of plugins through a Stream Deck plugin package. For more info, see: https://docs.elgato.com/sdk/plugins/packaging. For a better development experience, use Stream Deck app version 5.x.x

On recent versions of macOS, the build may fail because of a missing <cassert> header in the Stream Deck SDK. This will hopefully get fixed soon, but for now you can add '''#include \<cassert\>''' at the top of the file where this issue occurs to solve it.

<br>

    The trademark, name, and logo associated with Gig Performer, as well as any assets related to it, 
    including but not limited to images of buttons and knobs, 
    are the exclusive and proprietary intellectual property of Deskew Technologies DE, LLC.
