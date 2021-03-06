old-dtb := $(dtb-y)
old-dtbo := $(dtbo-y)
dtb-y :=
dtbo-y :=
makefile-path := platform/t210b01/darcy/kernel-dts

dts-include += platform/t210/foster/kernel-dts
dts-include += platform/t210/common/kernel-dts
dts-include += platform/t210b01/ers/kernel-dts
dts-include += $(makefile-path)

dtb-$(CONFIG_ARCH_TEGRA_210_SOC) += tegra210b01-darcy-p2894-0050-a08-00.dtb
dtb-$(CONFIG_ARCH_TEGRA_210_SOC) += tegra210b01-darcy-p2894-2551-b00-00.dtb
dtb-$(CONFIG_ARCH_TEGRA_210_SOC) += tegra210b01-darcy-p2894-3551-b03-00.dtb
dtbo-$(CONFIG_ARCH_TEGRA_210_SOC) += tegra210b01-darcy-p2894-audio-overlay.dtbo

ifneq ($(dtb-y),)
dtb-y := $(addprefix $(makefile-path)/,$(dtb-y))
endif
ifneq ($(dtbo-y),)
dtbo-y := $(addprefix $(makefile-path)/,$(dtbo-y))
endif

dtb-y += $(old-dtb)
dtbo-y += $(old-dtbo)
