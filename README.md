# device/lineage/sepolicy (Miku-Picked UI)

Miku-Picked UI keeps its common SELinux policy in `device/miku/sepolicy`,
which already includes the LineageOS 23.2 HAL policy.

Only the parts LineageOS 23.2 device trees include directly are kept:

- `libperfmgr/` (`device/lineage/sepolicy/libperfmgr/sepolicy.mk`)
- `exynos/` (`device/lineage/sepolicy/exynos/sepolicy.mk`, Samsung Exynos
  trees such as universal2100-common); its LiveDisplay domain builds on the
  `hal_lineage_livedisplay` attribute from `device/miku/sepolicy`

The rest was removed so no type is defined twice.

Original source: https://github.com/LineageOS/android_device_lineage_sepolicy (lineage-23.2)
