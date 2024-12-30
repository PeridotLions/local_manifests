# local_manifests

# Patches:

## Xiaomi TouchFeature Calls
```
# repopick -g https://review.blissroms.org 21268 -P frameworks/base/ (OLD)
cd frameworks/base && curl -s https://raw.githubusercontent.com/PeridotLions/local_manifests/los-22.1/patches/framework/base/0001-DNM-SystemUI-Add-xiaomi-fingerprintextension-and-tou.patch && git am - && cd -

cd hardware/xiaomi && curl -s https://raw.githubusercontent.com/PeridotLions/local_manifests/los-22.1/patches/hardware/xiaomi/e3bbd377774f9577f4159f77018e220cc60b1786.patch && git am - && cd -

```