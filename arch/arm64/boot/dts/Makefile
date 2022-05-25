# SPDX-License-Identifier: GPL-2.0

dtb-y += exynos/exynos9610.dtb


ifdef CONFIG_SEC_M31_PROJECT
dtbo-y += samsung/exynos9611-m31_eur_open_00.dtbo
endif

ifdef CONFIG_SEC_M21_PROJECT
dtbo-y += samsung/exynos9611-m21_swa_open_00.dtbo
dtbo-y += samsung/exynos9611-m21_swa_open_06.dtbo
endif

ifdef CONFIG_SEC_A51_PROJECT
dtbo-y += samsung/exynos9611-a51_eur_open_00.dtbo
dtbo-y += samsung/exynos9611-a51_eur_open_01.dtbo
dtbo-y += samsung/exynos9611-a51_eur_open_03.dtbo
dtbo-y += samsung/exynos9611-a51_eur_open_07.dtbo
endif

ifdef CONFIG_SEC_F41_PROJECT
dtbo-y += samsung/exynos9611-f41_swa_open_00.dtbo
endif

ifdef CONFIG_SEC_M31S_PROJECT
dtbo-y += samsung/exynos9611-m31s_eur_open_00.dtbo
endif

targets += dtbs

DTB_LIST  := $(dtb-y) $(dtbo-y)
always    := $(DTB_LIST)

dtbs: $(addprefix $(obj)/, $(DTB_LIST))

clean-files := *.dtb*
