#
# Copyright (C) 2009 OpenWrt.org
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#
include $(TOPDIR)/rules.mk

ARCH:=mips
BOARD:=livebox2
BOARDNAME:=livebox2
FEATURES:=squashfs jffs2 atm
CFLAGS:=-Os -pipe -mtune=r3000 -funit-at-a-time -mips1

LINUX_VERSION:=2.6.15

include $(INCLUDE_DIR)/target.mk

DEFAULT_PACKAGES += kmod-pppoa ppp-mod-pppoa linux-atm atm-tools br2684ctl swconfig hostapd

define Target/Description
	Firmware para el livebox 2
endef

$(eval $(call BuildTarget))
