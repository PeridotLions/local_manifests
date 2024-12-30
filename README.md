# local_manifests

# Patches:

## Xiaomi TouchFeature Calls
```
# repopick -g https://review.blissroms.org 21268 -P frameworks/base/ (OLD)
cd frameworks/base && curl -s https://raw.githubusercontent.com/PeridotLions/local_manifests/los-22.1/patches/framework/base/0001-DNM-SystemUI-Add-xiaomi-fingerprintextension-and-tou.patch | git am - && cd -

cd hardware/xiaomi && curl -s https://raw.githubusercontent.com/PeridotLions/local_manifests/los-22.1/patches/hardware/xiaomi/e3bbd377774f9577f4159f77018e220cc60b1786.patch | git am - && \
curl -s https://raw.githubusercontent.com/PeridotLions/local_manifests/los-22.1/patches/hardware/xiaomi/298d58637ac6a4cf4ce60dc535a933eb000cf319.patch | git am - && cd -

```

## Pineapple platform support
```
cd hardware/qcom-caf/common && curl -s https://raw.githubusercontent.com/PeridotLions/local_manifests/los-22.1/patches/hardware/qcom-caf/common/cec05faa45fa52528dc428d3a2193ef4f17f4835.patch | git am - && cd -
```

## Xiaomi FastCharge support
```
cd hardware/xiaomi && curl -s https://raw.githubusercontent.com/PeridotLions/local_manifests/los-22.1/patches/hardware/xiaomi/10a0e68c708b3a0184452d3ca66fd28e35f9ccf5.patch | git am - && cd -
```