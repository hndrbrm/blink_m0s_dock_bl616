cmake_minimum_required(VERSION 3.15)

include(board.conf)
include(common.conf)
include(project.conf)

find_package(bouffalo_sdk REQUIRED HINTS $ENV{BL_SDK_BASE})

sdk_set_main_file(main.c)

project(blink)
