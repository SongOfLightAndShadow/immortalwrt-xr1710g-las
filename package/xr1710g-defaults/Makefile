include $(TOPDIR)/rules.mk

PKG_NAME:=xr1710g-defaults
PKG_VERSION:=1.0
PKG_RELEASE:=1

include $(INCLUDE_DIR)/package.mk

define Package/xr1710g-defaults
  SECTION:=base
  CATEGORY:=Base system
  TITLE:=Default Kconfig overrides for Gemtek XR1710G
  DEFAULT:=y if TARGET_airoha_an7581
endef

define Package/xr1710g-defaults/config
        imply LUCI_LANG_zh_Hans
	imply LUCI_LANG_ja
        select BUSYBOX_CUSTOM
        select BUSYBOX_CONFIG_DEVMEM
endef

define Build/Compile
endef

define Package/xr1710g-defaults/install
        $(INSTALL_DIR) $(1)/etc
endef

$(eval $(call BuildPackage,xr1710g-defaults))
