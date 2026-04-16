## Repo Init ##
```bash
repo init -u https://github.com/Adarsh0127-Elite/zephyr_manifest.git -b main
```
## Sync Source ##
```bash
repo sync --force-sync --no-clone-bundle --current-branch --no-tags -j$(nproc --all)
```
## Start building ##
```bash
LTO=thin build/build.sh -j$(nproc --all)
```
