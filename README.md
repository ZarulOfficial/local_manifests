```
# Initialize local repository
repo init -u https://github.com/PixelExperience/manifest -b thirteen-plus

# Clone custom manifest
git clone https://github.com/2by2-Project/local_manifest .repo/local_manifests -b 13

# Sync
repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
```
