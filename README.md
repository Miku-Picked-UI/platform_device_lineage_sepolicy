# device/lineage/sepolicy (Miku-Picked UI)

Miku-Picked UI keeps its common SELinux policy in `device/miku/sepolicy`,
which already includes the LineageOS 23.2 HAL policy.

Only `libperfmgr/` is kept here, because LineageOS 23.2 device trees
include `device/lineage/sepolicy/libperfmgr/sepolicy.mk` directly.
The rest was removed so no type is defined twice.

Original source: https://github.com/LineageOS/android_device_lineage_sepolicy (lineage-23.2)
