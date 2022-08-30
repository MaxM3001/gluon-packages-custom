include $(TOPDIR)/rules.mk

PKG_NAME:=gluon-offloader-config
PKG_BUILD_DIR:=$(BUILD_DIR)/$(PKG_NAME)

include $(TOPDIR)/../package/gluon.mk

define Package/$(PKG_NAME)
	TITLE:=offloader config
        DEPENDS:=+gluon-core
endef

define Package/$(PKG_NAME)/install
	$(CP) ./files/* $(1)/
endef

$(eval $(call BuildPackage,$(PKG_NAME)))
