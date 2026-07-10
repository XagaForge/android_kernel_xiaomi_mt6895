# SPDX-License-Identifier: GPL-2.0
DTC_INCLUDE += $(srctree)/arch/arm64/boot/dts/vendor

dtb-$(CONFIG_ARCH_MEDIATEK) += \
	mt6853.dtb \
	mt6873.dtb \
	mt6895.dtb \
	mt6983.dtb

dtbo-$(CONFIG_TARGET_PRODUCT_XAGA) += xaga.dtbo
xaga.dtbo-base := mt6895.dtb

dtbo-$(CONFIG_TARGET_PRODUCT_PLATO) += plato.dtbo
plato.dtbo-base := mt6895.dtb
