# SPDX-License-Identifier: GPL-2.0+

dtb-$(CONFIG_TARGET_AX25_AE350) += ae350_32.dtb ae350_64.dtb
dtb-$(CONFIG_TARGET_ALDEC_TYSOM_M_MPFS250T) += mpfs-tysom-m.dtb
dtb-$(CONFIG_TARGET_ARIES_M100PFSEVP) += mpfs-m100pfsevp.dtb
dtb-$(CONFIG_TARGET_BEAGLEBOARD_BEAGLEVFIRE) += mpfs-beaglev-fire.dtb
dtb-$(CONFIG_TARGET_MICROCHIP_ICICLE) += microchip-mpfs-icicle-kit.dtb \
microchip-mpfs-icicle-kit-amp.dtb microchip-mpfs-icicle-kit-qspi-nor.dtb
dtb-$(CONFIG_TARGET_MICROCHIP_DISCOKIT) += microchip-mpfs-disco-kit.dtb
dtb-$(CONFIG_TARGET_MICROCHIP_VIDEOKIT) += microchip-mpfs-video-kit.dtb
dtb-$(CONFIG_TARGET_MICROCHIP_PIC64GX_CURIOSITY) += \
microchip-pic64gx-curiosity-kit.dtb microchip-pic64gx-curiosity-kit-amp.dtb
dtb-$(CONFIG_TARGET_SUNDANCEDSP_POLARBERRY) += mpfs-polarberry.dtb
dtb-$(CONFIG_TARGET_QEMU_VIRT) += qemu-virt32.dtb qemu-virt64.dtb
dtb-$(CONFIG_TARGET_OPENPITON_RISCV64) += openpiton-riscv64.dtb
dtb-$(CONFIG_TARGET_SIFIVE_UNLEASHED) += hifive-unleashed-a00.dtb
dtb-$(CONFIG_TARGET_SIFIVE_UNMATCHED) += hifive-unmatched-a00.dtb
dtb-$(CONFIG_TARGET_SIPEED_MAIX) += k210-maix-bit.dtb
dtb-$(CONFIG_TARGET_STARFIVE_VISIONFIVE2) += jh7110-starfive-visionfive-2-v1.3b.dtb
dtb-$(CONFIG_TARGET_STARFIVE_VISIONFIVE2) += jh7110-starfive-visionfive-2-v1.2a.dtb
include $(srctree)/scripts/Makefile.dts

targets += $(dtb-y)

DTC_FLAGS += -R 4 -p 0x1000

PHONY += dtbs
dtbs: $(addprefix $(obj)/, $(dtb-y))
	@:

clean-files := *.dtb
