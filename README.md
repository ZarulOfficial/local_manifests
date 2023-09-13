```
# Initialize local repository
repo init -u https://github.com/PixelOS-AOSP/manifest.git -b thirteen

# Clone custom manifest
git clone https://github.com/2by2-Project/local_manifests .repo/local_manifests -b 13

# Sync
repo sync -j$(nproc --all)
```
