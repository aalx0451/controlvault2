## ControlVault 2 support (binpatch)
This folder provides simple Nix module downloading, patching and installing libfprint-2-tod-1-broadcom.so for ControlVault 2.

Note deleting is not clearing CV2's NVRAM. 
Note error codes are not handled properly.

## Installation
1. Don't forget to configure `allowUnfree = true`, due to unfree TOD plugin installation
2. Place `cv2-fingerprint.nix` to `/etc/nixos`
3. Include it and rebuild NixOS

## Caveats
While deleting can be fixed, there is actually no reason for using this instead of source code patch.

## License
This code is a Public Domain and licensed under the Unlicense; see ../LICENSE.
Unlike it, the patched binary is licensed under the Broadcom Inc. and/or its subsidiaries Software License Agreement.
