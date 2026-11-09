include $(TOPDIR)/rules.mk

ARCH:=aarch64
BOARD:=qualcommax
BOARDNAME:=Qualcomm Atheros 802.11ax WiSoC-s
FEATURES:=squashfs ramdisk fpu nand rtc emmc
KERNELNAME:=Image
CPU_TYPE:=cortex-a53
SUBTARGETS:=ipq807x ipq60xx ipq50xx

KERNEL_PATCHVER:=6.12

include $(INCLUDE_DIR)/target.mk
DEFAULT_PACKAGES += \
	autocore cpufreq luci-app-cpufreq uboot-envtools \
	kmod-ath11k kmod-ath11k-ahb kmod-ath11k-pci kmod-dsa kmod-dsa-qca8k kmod-phy-aquantia kmod-phy-qca83xx \
	kmod-gpio-button-hotplug kmod-leds-gpio kmod-leds-pwm \
	kmod-qca-nss-dp kmod-nss-ifb \
	kmod-qca-nss-drv kmod-qca-nss-ecm

$(eval $(call BuildTarget))
