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

#
# Makefile for misc devices that really don't fit anywhere else.
#

MTK_PLATFORM := $(subst ",,$(CONFIG_MTK_PLATFORM))
ARCH_MTK_PROJECT := $(subst ",,$(CONFIG_ARCH_MTK_PROJECT))

MTK_CUSTOM_PATH  := $(srctree)/drivers/misc/mediatek


subdir-ccflags-y += -I$(MTK_CUSTOM_PATH)/lens/main2/inc
subdir-ccflags-y += -I$(MTK_CUSTOM_PATH)/lens/main2/common/lc898212xdaf_f/inc

obj-$(CONFIG_MTK_LENS)    += main2af.o

main2af-y  += main2_lens.o
main2af-y  += common/lc898212xdaf_f/LC898212XDAF_F.o
main2af-y  += common/lc898212xdaf_f/LC89821x_STMV.o
main2af-y  += common/ak7371af/AK7371AF.o