# CMSIS Build CMakeLists generated on 2023-07-23T00:05:59

cmake_minimum_required(VERSION 3.22)

# Target options

set(TARGET Project)
set(CPU Cortex-M3)
set(PRJ_DIR "/Users/jeremy/Documents/STM32项目/项目模版")
set(OUT_DIR "/Users/jeremy/Documents/STM32项目/项目模版/out/Project/Target_1")
set(INT_DIR "/Users/jeremy/Documents/STM32项目/项目模版/tmp/Project/Target_1")
set(FPU NO_FPU)
set(SECURE Non-secure)
set(BYTE_ORDER Little-endian)
set(OPTIMIZE none)
set(DEBUG on)
set(AS_FLAGS_GLOBAL "-masm=auto")
set(CC_FLAGS_GLOBAL "-fno-rtti -funsigned-char -fshort-enums -fshort-wchar -ffunction-sections -std=c99 -Wno-packed -Wno-missing-variable-declarations -Wno-missing-prototypes -Wno-missing-noreturn -Wno-sign-conversion -Wno-nonportable-include-path -Wno-reserved-id-macro -Wno-unused-macros -Wno-documentation-unknown-command -Wno-documentation -Wno-license-management -Wno-parentheses-equality")
set(CXX_FLAGS_GLOBAL "-fno-rtti -funsigned-char -fshort-enums -fshort-wchar -ffunction-sections -std=c99 -Wno-packed -Wno-missing-variable-declarations -Wno-missing-prototypes -Wno-missing-noreturn -Wno-sign-conversion -Wno-nonportable-include-path -Wno-reserved-id-macro -Wno-unused-macros -Wno-documentation-unknown-command -Wno-documentation -Wno-license-management -Wno-parentheses-equality")
set(LD_FLAGS_GLOBAL "--map --load_addr_map_info --xref --callgraph --symbols --info sizes --info totals --info unused --info veneers --list --strict --summary_stderr --info summarysizes")
set(LD_SCRIPT "/Users/jeremy/Documents/STM32项目/项目模版/Project_Target_1.sct")

set(DEFINES
  STM32F10X_MD
  USE_STDPERIPH_DRIVER
)

set(INC_PATHS
  "/Users/jeremy/Documents/STM32项目/项目模版/Start"
  "/Users/jeremy/Documents/STM32项目/项目模版/Library"
  "/Users/jeremy/Documents/STM32项目/项目模版/User"
  "/Users/jeremy/Documents/STM32项目/项目模版/System"
  "/Users/jeremy/.cache/arm/packs/Keil/STM32F1xx_DFP/2.4.1/Device/Include"
)

set(AS_ARM_SRC_FILES
  "/Users/jeremy/Documents/STM32项目/项目模版/Start/startup_stm32f10x_md.s"
)

set(CC_SRC_FILES
  "/Users/jeremy/Documents/STM32项目/项目模版/Library/misc.c"
  "/Users/jeremy/Documents/STM32项目/项目模版/Library/stm32f10x_adc.c"
  "/Users/jeremy/Documents/STM32项目/项目模版/Library/stm32f10x_bkp.c"
  "/Users/jeremy/Documents/STM32项目/项目模版/Library/stm32f10x_can.c"
  "/Users/jeremy/Documents/STM32项目/项目模版/Library/stm32f10x_cec.c"
  "/Users/jeremy/Documents/STM32项目/项目模版/Library/stm32f10x_crc.c"
  "/Users/jeremy/Documents/STM32项目/项目模版/Library/stm32f10x_dac.c"
  "/Users/jeremy/Documents/STM32项目/项目模版/Library/stm32f10x_dbgmcu.c"
  "/Users/jeremy/Documents/STM32项目/项目模版/Library/stm32f10x_dma.c"
  "/Users/jeremy/Documents/STM32项目/项目模版/Library/stm32f10x_exti.c"
  "/Users/jeremy/Documents/STM32项目/项目模版/Library/stm32f10x_flash.c"
  "/Users/jeremy/Documents/STM32项目/项目模版/Library/stm32f10x_fsmc.c"
  "/Users/jeremy/Documents/STM32项目/项目模版/Library/stm32f10x_gpio.c"
  "/Users/jeremy/Documents/STM32项目/项目模版/Library/stm32f10x_i2c.c"
  "/Users/jeremy/Documents/STM32项目/项目模版/Library/stm32f10x_iwdg.c"
  "/Users/jeremy/Documents/STM32项目/项目模版/Library/stm32f10x_pwr.c"
  "/Users/jeremy/Documents/STM32项目/项目模版/Library/stm32f10x_rcc.c"
  "/Users/jeremy/Documents/STM32项目/项目模版/Library/stm32f10x_rtc.c"
  "/Users/jeremy/Documents/STM32项目/项目模版/Library/stm32f10x_sdio.c"
  "/Users/jeremy/Documents/STM32项目/项目模版/Library/stm32f10x_spi.c"
  "/Users/jeremy/Documents/STM32项目/项目模版/Library/stm32f10x_tim.c"
  "/Users/jeremy/Documents/STM32项目/项目模版/Library/stm32f10x_usart.c"
  "/Users/jeremy/Documents/STM32项目/项目模版/Library/stm32f10x_wwdg.c"
  "/Users/jeremy/Documents/STM32项目/项目模版/Start/system_stm32f10x.c"
  "/Users/jeremy/Documents/STM32项目/项目模版/System/Delay.c"
  "/Users/jeremy/Documents/STM32项目/项目模版/User/main.c"
  "/Users/jeremy/Documents/STM32项目/项目模版/User/stm32f10x_it.c"
)

# Toolchain config map

set(REGISTERED_TOOLCHAIN_ROOT "/Users/jeremy/.vcpkg/artifacts/fd3d78d7/compilers.arm.armclang/6.20.0/bin")
set(REGISTERED_TOOLCHAIN_VERSION "6.20.0")
set(TOOLCHAIN_VERSION_MIN "6.20.0")
include ("/Users/jeremy/.vcpkg/artifacts/fd3d78d7/tools.open.cmsis.pack.cmsis.toolbox/2.0.0/etc/AC6.6.18.0.cmake")
include ("/Users/jeremy/.vcpkg/artifacts/fd3d78d7/tools.open.cmsis.pack.cmsis.toolbox/2.0.0/etc/CMSIS-Build-Utils.cmake")

# Setup project

project(${TARGET} LANGUAGES AS_ARM C)

cbuild_get_running_toolchain(TOOLCHAIN_ROOT TOOLCHAIN_VERSION C)

# Global Flags

set(CMAKE_AS_ARM_FLAGS "${AS_ARM_CPU} ${AS_ARM_BYTE_ORDER} ${AS_ARM_DEFINES} ${AS_ARM_OPTIONS_FLAGS} ${AS_ARM_FLAGS} ${AS_FLAGS_GLOBAL}")
cbuild_get_system_includes(CC_SYS_INC_PATHS_LIST CC_SYS_INC_PATHS)
set(CMAKE_C_FLAGS "${CC_CPU} ${CC_BYTE_ORDER} ${CC_DEFINES} ${CC_SECURE} ${CC_OPTIONS_FLAGS} ${CC_FLAGS} ${CC_FLAGS_GLOBAL} ${CC_SYS_INC_PATHS}")
set(CMAKE_C_LINK_FLAGS "${LD_CPU} ${_LS}\"${LD_SCRIPT}\" ${LD_SECURE} ${LD_FLAGS_GLOBAL} ${LD_OPTIONS_FLAGS} ${LD_FLAGS}")

# Local Flags

foreach(SRC ${AS_ARM_SRC_FILES})
  set_source_files_properties(${SRC} PROPERTIES LANGUAGE AS_ARM)
endforeach()

# Compilation Database

set(CMAKE_EXPORT_COMPILE_COMMANDS ON)
add_custom_target(database COMMAND ${CMAKE_COMMAND} -E copy_if_different "${INT_DIR}/compile_commands.json" "${OUT_DIR}")

# Setup Target

add_executable(${TARGET} ${AS_ARM_SRC_FILES} ${CC_SRC_FILES})
set_target_properties(${TARGET} PROPERTIES PREFIX "" SUFFIX ".axf" OUTPUT_NAME "Project")
set_target_properties(${TARGET} PROPERTIES RUNTIME_OUTPUT_DIRECTORY ${OUT_DIR} LINK_DEPENDS ${LD_SCRIPT})
target_include_directories(${TARGET} PUBLIC ${INC_PATHS})
