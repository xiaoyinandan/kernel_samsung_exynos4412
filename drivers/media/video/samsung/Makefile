obj-$(CONFIG_VIDEO_FIMC)	+= fimc/
obj-$(CONFIG_VIDEO_JPEG)	+= jpeg/
obj-$(CONFIG_VIDEO_JPEG_V2X)	+= jpeg_v2x/
obj-$(CONFIG_VIDEO_TVOUT)	+= tvout/
obj-$(CONFIG_VIDEO_MFC5X)	+= mfc5x/

ifeq ($(CONFIG_ARCH_EXYNOS4), y)
obj-$(CONFIG_VIDEO_FIMG2D3X)	+= fimg2d3x-exynos4/
obj-$(CONFIG_VIDEO_FIMG2D4X)	+= fimg2d4x-exynos4/
else
obj-$(CONFIG_VIDEO_FIMG2D3X)	+= fimg2d3x/
obj-$(CONFIG_VIDEO_FIMG2D4X)	+= fimg2d4x/
endif

ifeq ($(CONFIG_BUILD_TARGET_AOSP), y)
obj-$(CONFIG_VIDEO_UMP)		+= ump/
obj-$(CONFIG_VIDEO_MALI400MP)	+= mali/
else
obj-$(CONFIG_VIDEO_UMP)		+= ump_sam/
obj-$(CONFIG_VIDEO_MALI400MP)	+= mali_sam/
endif
obj-$(CONFIG_VIDEO_TSI)		+= tsi/

EXTRA_CFLAGS += -Idrivers/media/video
