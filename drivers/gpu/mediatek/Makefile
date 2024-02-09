#
# Copyright (C) 2015 MediaTek Inc.
#
# This program is free software: you can redistribute it and/or modify
# it under the terms of the GNU General Public License version 2 as
# published by the Free Software Foundation.
#
# This program is distributed in the hope that it will be useful,
# but WITHOUT ANY WARRANTY; without even the implied warranty of
# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
# GNU General Public License for more details.
#

ifneq ($(CONFIG_MTK_PLATFORM),)
export MTK_PLATFORM = $(subst ",,$(CONFIG_MTK_PLATFORM))
else
export MTK_PLATFORM = $(word 4,$(MTK_GPU_VERSION))
endif

ifeq ($(MTK_PLATFORM),mt6873)
subdir-ccflags-y += -DCONFIG_GPU_MT6873
else ifeq ($(MTK_PLATFORM),mt6893)
subdir-ccflags-y += -DCONFIG_GPU_MT6893
else ifeq ($(MTK_PLATFORM),mt6853)
subdir-ccflags-y += -DCONFIG_GPU_MT6853
endif

obj-$(CONFIG_MTK_GPU_SUPPORT) += ged/
obj-$(CONFIG_MTK_GPU_SUPPORT) += hal/
obj-$(CONFIG_MTK_GPU_SUPPORT) += gpufreq/
obj-$(CONFIG_MTK_GPU_SUPPORT) += gpu_bm/
obj-$(CONFIG_MTK_GPU_SUPPORT)+= gpueb/
