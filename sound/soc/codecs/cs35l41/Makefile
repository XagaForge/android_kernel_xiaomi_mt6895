#for cs35l41 build
snd-soc-cs35l41-objs += cs35l41.o
snd-soc-cs35l41-objs += cs35l41-tables.o
snd-soc-cs35l41-objs += cs35l41-i2c.o
snd-soc-cs35l41-objs += wm_adsp.o

obj-$(CONFIG_SND_SOC_CS35L41) += snd-soc-cs35l41.o

ccflags-$(CONFIG_TARGET_PRODUCT_PLATO) += -DCONFIG_TARGET_PRODUCT_CUPID -DCONFIG_SWITCH_PROTECTION
ccflags-$(CONFIG_TARGET_PRODUCT_DAUMIER) += -DCONFIG_SWITCH_PROTECTION
