## Repo Init ##
```bash
repo init -u https://github.com/NINJAHUNTER1357/kernel_manifest.git -b pickle
```
## Sync Source ##
```bash
repo sync --force-sync --no-clone-bundle --current-branch --no-tags -j$(nproc --all)
```
## Start building ##
```bash
LTO=thin build/build.sh -j$(nproc --all)
```
