#
# Copyright (c) 2019, NXP
#
# SPDX-License-Identifier: Apache-2.0
#

zephyr_include_directories(./include)
add_subdirectory_ifdef(
  CONFIG_USB_DEVICE_DRIVER
  device
  )
add_subdirectory_ifdef(
  CONFIG_USB_DEVICE_DRIVER
  phy
  )
