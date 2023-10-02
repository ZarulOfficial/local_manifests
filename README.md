## Normal Sync (recommended)

The normal syncing.

```
# Initialize local repository
repo init -u https://github.com/ArrowOS/android_manifest.git -b arrow-13.1

# Clone custom manifest
git clone https://github.com/2by2-Project/local_manifests .repo/local_manifests -b 13

# Sync
repo sync -j$(nproc --all)
```

## Force Sync

For force syncing, use `--force-sync` flag with `repo sync`.

**NOTE: For contributor, don't forget commit && pushing the local changes to anywhere before force syncing, otherwise repo will discard unpushed changes!**

```
# Initialize local repository
repo init -u https://github.com/ArrowOS/android_manifest.git -b arrow-13.1

# Clone custom manifest
git clone https://github.com/2by2-Project/local_manifests .repo/local_manifests -b 13

# Sync
repo sync -j$(nproc --all) --force-sync
```