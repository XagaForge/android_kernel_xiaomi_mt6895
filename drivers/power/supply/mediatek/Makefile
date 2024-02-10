# SPDX-License-Identifier: GPL-2.0
subdir-ccflags-y += -I$(srctree)/drivers/misc/mediatek/typec/tcpc/inc
subdir-ccflags-y += -I$(srctree)/drivers/misc/mediatek/power_throttling
subdir-ccflags-y += -I$(srctree)/drivers/misc/mediatek/include

obj-$(CONFIG_BATTERY_MT6359P) += mt6359p_battery.o
mt6359p_battery-objs := mtk_battery_coulomb_service.o mtk_battery.o mtk_battery_algo.o mt6359p-gauge.o mtk_battery_daemon.o
obj-$(CONFIG_AXP288_FUEL_GAUGE) += axp288_fuel_gauge.o
obj-$(CONFIG_CHARGER_MT6360)	+= mt6360_pmu_chg.o
obj-$(CONFIG_CHARGER_MT6362)	+= mt6362-chg.o
obj-$(CONFIG_CHARGER_MT6375)	+= mt6375-charger.o
obj-$(CONFIG_CHARGER_RT9759) += rt9759.o
obj-$(CONFIG_GAUGE_MT6375)	+= mt6375-battery.o
mt6375-battery-objs := mtk_battery_coulomb_service.o mtk_battery.o mtk_battery_algo.o mt6375-gauge.o mtk_battery_daemon.o
obj-$(CONFIG_MTK_CHARGER_TYPE_DETECT)	+= mtk_chg_type_det.o
obj-$(CONFIG_MTK_CHARGER) += mtk_charger_framework.o mtk_pd_charging.o charger_class.o adapter_class.o mtk_charger_algorithm_class.o mtk_pd_adapter.o
mtk_charger_framework-objs := mtk_charger.o mtk_charger_intf.o mtk_basic_charger.o mtk_pulse_charger.o pmic_voter.o step_jeita_charge.o
mtk_pd_charging-objs := mtk_pd.o mtk_pd_hal.o
obj-$(CONFIG_MTK_PUMP_EXPRESS_PLUS_20_SUPPORT) += mtk_pep20.o
mtk_pep20-objs := mtk_pe2.o mtk_pe2_hal.o
obj-$(CONFIG_MTK_PUMP_EXPRESS_PLUS_SUPPORT) += mtk_pep.o
mtk_pep-objs := mtk_pe.o mtk_pe_hal.o
obj-$(CONFIG_MTK_PUMP_EXPRESS_40_SUPPORT) += mtk_pep40.o
mtk_pep40-objs := mtk_pe4.o mtk_pe4_hal.o
obj-$(CONFIG_MTK_PUMP_EXPRESS_50_SUPPORT) += mtk_pep50.o
mtk_pep50-objs := mtk_pe5.o mtk_pe5_hal.o
obj-$(CONFIG_XMUSB350_CHARGER_DET) += xmusb350.o
obj-$(CONFIG_XMEXT_TI_GAUGE) += bq28z610.o
obj-$(CONFIG_XMEXT_CHG_PUMP) += sc8561.o
obj-$(CONFIG_XMEXT_SC8551A_CHG_PUMP) += sc8551.o
obj-$(CONFIG_XMEXT_LN8000_CHG_PUMP) += ln8000_charger.o
ifeq ($(CONFIG_BUILD_PRODUCT_NAME),"daumier")
obj-$(CONFIG_XM_PD_MANAGER) += pd_single_cp_manager.o
else
obj-$(CONFIG_XM_PD_MANAGER) += pd_cp_manager.o
endif
obj-$(CONFIG_XM_QC_MANAGER) += qc_cp_manager.o
