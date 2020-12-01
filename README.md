# OrangeFox Recovery Project for the Samsung Galaxy A40

### How to build ###

```bash
# Create dirs
$ mkdir ofox; cd ofox

# Init repo
$ repo init --depth=1 -u https://gitlab.com/OrangeFox/Manifest.git -b fox_9.0

# Clone a40 repo
$ git clone https://github.com/Galaxy-A-Devices/android_device_samsung_a40 -b fox-9.0 device/samsung/a40

# Sync
$ repo sync --no-repo-verify -c --force-sync --no-clone-bundle --no-tags --optimized-fetch --prune -j`nproc`

# Build
$ chmod +x build_ofox.sh ; ./build_ofox.sh
```

## Credits
* Astrako: For build_ofox.sh file
