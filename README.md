# Local Manifests #
Just grab the manifest and sync to get device sources

### AOSP S ###

Required patches for IMS: https://gerrit.pixelexperience.org/q/topic:%22mediatek-ims%22+(status:open%20OR%20status:merged)

# Grab Local Manifest
```bash
curl -o .repo/local_manifests/local_manifests.xml https://raw.githubusercontent.com/Himemoria/local_manifests/master/twelve.xml --create-dirs
```

# Sync
```bash
repo sync -j$(nproc --all) --force-sync
```