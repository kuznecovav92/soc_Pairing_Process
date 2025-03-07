################################################################################
# Automatically-generated file. Do not edit!
################################################################################

-include ../makefile.init

RM := rm -rf

# All of the sources participating in the build are defined here
-include sources.mk
-include gecko_sdk_3.2.3/util/third_party/segger/systemview/SEGGER/subdir.mk
-include gecko_sdk_3.2.3/util/third_party/freertos/kernel/portable/SiliconLabs/subdir.mk
-include gecko_sdk_3.2.3/util/third_party/freertos/kernel/portable/MemMang/subdir.mk
-include gecko_sdk_3.2.3/util/third_party/freertos/kernel/portable/GCC/ARM_CM33_NTZ/non_secure/subdir.mk
-include gecko_sdk_3.2.3/util/third_party/freertos/kernel/subdir.mk
-include gecko_sdk_3.2.3/util/third_party/freertos/cmsis/Source/subdir.mk
-include gecko_sdk_3.2.3/util/third_party/crypto/sl_component/sl_psa_driver/src/subdir.mk
-include gecko_sdk_3.2.3/util/third_party/crypto/sl_component/sl_protocol_crypto/src/subdir.mk
-include gecko_sdk_3.2.3/util/third_party/crypto/sl_component/sl_alt/source/subdir.mk
-include gecko_sdk_3.2.3/util/third_party/crypto/sl_component/se_manager/src/subdir.mk
-include gecko_sdk_3.2.3/util/third_party/crypto/mbedtls/library/subdir.mk
-include gecko_sdk_3.2.3/util/silicon_labs/silabs_core/memory_manager/subdir.mk
-include gecko_sdk_3.2.3/protocol/bluetooth/src/subdir.mk
-include gecko_sdk_3.2.3/protocol/bluetooth/lib/EFR32MG21/GCC/subdir.mk
-include gecko_sdk_3.2.3/platform/service/udelay/src/subdir.mk
-include gecko_sdk_3.2.3/platform/service/system/src/subdir.mk
-include gecko_sdk_3.2.3/platform/service/sleeptimer/src/subdir.mk
-include gecko_sdk_3.2.3/platform/service/power_manager/src/subdir.mk
-include gecko_sdk_3.2.3/platform/service/mpu/src/subdir.mk
-include gecko_sdk_3.2.3/platform/service/iostream/src/subdir.mk
-include gecko_sdk_3.2.3/platform/service/hfxo_manager/src/subdir.mk
-include gecko_sdk_3.2.3/platform/service/device_init/src/subdir.mk
-include gecko_sdk_3.2.3/platform/radio/rail_lib/plugin/rail_util_rf_path/subdir.mk
-include gecko_sdk_3.2.3/platform/radio/rail_lib/plugin/rail_util_pti/subdir.mk
-include gecko_sdk_3.2.3/platform/radio/rail_lib/plugin/pa-conversions/subdir.mk
-include gecko_sdk_3.2.3/platform/middleware/glib/glib/subdir.mk
-include gecko_sdk_3.2.3/platform/middleware/glib/dmd/display/subdir.mk
-include gecko_sdk_3.2.3/platform/emlib/src/subdir.mk
-include gecko_sdk_3.2.3/platform/emdrv/nvm3/src/subdir.mk
-include gecko_sdk_3.2.3/platform/emdrv/gpiointerrupt/src/subdir.mk
-include gecko_sdk_3.2.3/platform/driver/leddrv/src/subdir.mk
-include gecko_sdk_3.2.3/platform/driver/button/src/subdir.mk
-include gecko_sdk_3.2.3/platform/common/toolchain/src/subdir.mk
-include gecko_sdk_3.2.3/platform/common/src/subdir.mk
-include gecko_sdk_3.2.3/platform/bootloader/api/subdir.mk
-include gecko_sdk_3.2.3/platform/Device/SiliconLabs/EFR32MG21/Source/GCC/subdir.mk
-include gecko_sdk_3.2.3/platform/Device/SiliconLabs/EFR32MG21/Source/subdir.mk
-include gecko_sdk_3.2.3/platform/CMSIS/RTOS2/Source/subdir.mk
-include gecko_sdk_3.2.3/hardware/driver/memlcd/src/memlcd_usart/subdir.mk
-include gecko_sdk_3.2.3/hardware/driver/memlcd/src/subdir.mk
-include gecko_sdk_3.2.3/hardware/board/src/subdir.mk
-include gecko_sdk_3.2.3/app/common/util/app_log/subdir.mk
-include gecko_sdk_3.2.3/app/bluetooth/common/ota_dfu/subdir.mk
-include autogen/subdir.mk
-include subdir.mk
-include objects.mk

ifneq ($(MAKECMDGOALS),clean)
ifneq ($(strip $(C_DEPS)),)
-include $(C_DEPS)
endif
endif

-include ../makefile.defs

OPTIONAL_TOOL_DEPS := \
$(wildcard ../makefile.defs) \
$(wildcard ../makefile.init) \
$(wildcard ../makefile.targets) \


BUILD_ARTIFACT_NAME := soc_Pairing_Process
BUILD_ARTIFACT_EXTENSION := axf
BUILD_ARTIFACT_PREFIX :=
BUILD_ARTIFACT := $(BUILD_ARTIFACT_PREFIX)$(BUILD_ARTIFACT_NAME)$(if $(BUILD_ARTIFACT_EXTENSION),.$(BUILD_ARTIFACT_EXTENSION),)

# Add inputs and outputs from these tool invocations to the build variables 

# All Target
all: main-build

# Main-build Target
main-build: soc_Pairing_Process.axf

# Tool invocations
soc_Pairing_Process.axf: $(OBJS) $(USER_OBJS) makefile objects.mk $(OPTIONAL_TOOL_DEPS)
	@echo 'Building target: $@'
	@echo 'Invoking: GNU ARM C Linker'
	arm-none-eabi-gcc -g -gdwarf-2 -mcpu=cortex-m33 -mthumb -T "C:\Users\kuznecovav.ZAV\SimplicityStudio\v5_workspace_ble\soc_Pairing_Process/autogen/linkerfile.ld" -Xlinker --gc-sections -Xlinker -Map="soc_Pairing_Process.map" -mfpu=fpv5-sp-d16 -mfloat-abi=hard --specs=nano.specs -o soc_Pairing_Process.axf -Wl,--start-group "./app.o" "./app_properties.o" "./main.o" "./autogen/gatt_db.o" "./autogen/sl_bluetooth.o" "./autogen/sl_board_default_init.o" "./autogen/sl_device_init_clocks.o" "./autogen/sl_event_handler.o" "./autogen/sl_iostream_handles.o" "./autogen/sl_iostream_init_usart_instances.o" "./autogen/sl_simple_button_instances.o" "./autogen/sl_simple_led_instances.o" "./gecko_sdk_3.2.3/app/bluetooth/common/ota_dfu/sl_ota_dfu.o" "./gecko_sdk_3.2.3/app/common/util/app_log/app_log.o" "./gecko_sdk_3.2.3/hardware/board/src/sl_board_control_gpio.o" "./gecko_sdk_3.2.3/hardware/board/src/sl_board_init.o" "./gecko_sdk_3.2.3/hardware/driver/memlcd/src/memlcd_usart/sl_memlcd_spi.o" "./gecko_sdk_3.2.3/hardware/driver/memlcd/src/sl_memlcd.o" "./gecko_sdk_3.2.3/hardware/driver/memlcd/src/sl_memlcd_display.o" "./gecko_sdk_3.2.3/platform/CMSIS/RTOS2/Source/os_systick.o" "./gecko_sdk_3.2.3/platform/Device/SiliconLabs/EFR32MG21/Source/GCC/startup_efr32mg21.o" "./gecko_sdk_3.2.3/platform/Device/SiliconLabs/EFR32MG21/Source/system_efr32mg21.o" "./gecko_sdk_3.2.3/platform/bootloader/api/btl_interface.o" "./gecko_sdk_3.2.3/platform/bootloader/api/btl_interface_storage.o" "./gecko_sdk_3.2.3/platform/common/src/sl_slist.o" "./gecko_sdk_3.2.3/platform/common/src/sli_cmsis_os2_ext_task_register.o" "./gecko_sdk_3.2.3/platform/common/toolchain/src/sl_memory.o" "./gecko_sdk_3.2.3/platform/driver/button/src/sl_button.o" "./gecko_sdk_3.2.3/platform/driver/button/src/sl_simple_button.o" "./gecko_sdk_3.2.3/platform/driver/leddrv/src/sl_led.o" "./gecko_sdk_3.2.3/platform/driver/leddrv/src/sl_simple_led.o" "./gecko_sdk_3.2.3/platform/emdrv/gpiointerrupt/src/gpiointerrupt.o" "./gecko_sdk_3.2.3/platform/emdrv/nvm3/src/nvm3_default_common_linker.o" "./gecko_sdk_3.2.3/platform/emdrv/nvm3/src/nvm3_hal_flash.o" "./gecko_sdk_3.2.3/platform/emdrv/nvm3/src/nvm3_lock.o" "./gecko_sdk_3.2.3/platform/emlib/src/em_assert.o" "./gecko_sdk_3.2.3/platform/emlib/src/em_burtc.o" "./gecko_sdk_3.2.3/platform/emlib/src/em_cmu.o" "./gecko_sdk_3.2.3/platform/emlib/src/em_core.o" "./gecko_sdk_3.2.3/platform/emlib/src/em_emu.o" "./gecko_sdk_3.2.3/platform/emlib/src/em_gpio.o" "./gecko_sdk_3.2.3/platform/emlib/src/em_msc.o" "./gecko_sdk_3.2.3/platform/emlib/src/em_prs.o" "./gecko_sdk_3.2.3/platform/emlib/src/em_rtcc.o" "./gecko_sdk_3.2.3/platform/emlib/src/em_se.o" "./gecko_sdk_3.2.3/platform/emlib/src/em_system.o" "./gecko_sdk_3.2.3/platform/emlib/src/em_usart.o" "./gecko_sdk_3.2.3/platform/middleware/glib/dmd/display/dmd_memlcd.o" "./gecko_sdk_3.2.3/platform/middleware/glib/glib/bmp.o" "./gecko_sdk_3.2.3/platform/middleware/glib/glib/glib.o" "./gecko_sdk_3.2.3/platform/middleware/glib/glib/glib_bitmap.o" "./gecko_sdk_3.2.3/platform/middleware/glib/glib/glib_circle.o" "./gecko_sdk_3.2.3/platform/middleware/glib/glib/glib_font_narrow_6x8.o" "./gecko_sdk_3.2.3/platform/middleware/glib/glib/glib_font_normal_8x8.o" "./gecko_sdk_3.2.3/platform/middleware/glib/glib/glib_font_number_16x20.o" "./gecko_sdk_3.2.3/platform/middleware/glib/glib/glib_line.o" "./gecko_sdk_3.2.3/platform/middleware/glib/glib/glib_polygon.o" "./gecko_sdk_3.2.3/platform/middleware/glib/glib/glib_rectangle.o" "./gecko_sdk_3.2.3/platform/middleware/glib/glib/glib_string.o" "./gecko_sdk_3.2.3/platform/radio/rail_lib/plugin/pa-conversions/pa_conversions_efr32.o" "./gecko_sdk_3.2.3/platform/radio/rail_lib/plugin/pa-conversions/pa_curves_efr32.o" "./gecko_sdk_3.2.3/platform/radio/rail_lib/plugin/rail_util_pti/sl_rail_util_pti.o" "./gecko_sdk_3.2.3/platform/radio/rail_lib/plugin/rail_util_rf_path/sl_rail_util_rf_path.o" "./gecko_sdk_3.2.3/platform/service/device_init/src/sl_device_init_emu_s2.o" "./gecko_sdk_3.2.3/platform/service/device_init/src/sl_device_init_hfrco.o" "./gecko_sdk_3.2.3/platform/service/device_init/src/sl_device_init_hfxo_s2.o" "./gecko_sdk_3.2.3/platform/service/device_init/src/sl_device_init_lfxo_s2.o" "./gecko_sdk_3.2.3/platform/service/device_init/src/sl_device_init_nvic.o" "./gecko_sdk_3.2.3/platform/service/hfxo_manager/src/sl_hfxo_manager.o" "./gecko_sdk_3.2.3/platform/service/hfxo_manager/src/sl_hfxo_manager_hal_s2.o" "./gecko_sdk_3.2.3/platform/service/iostream/src/sl_iostream.o" "./gecko_sdk_3.2.3/platform/service/iostream/src/sl_iostream_retarget_stdio.o" "./gecko_sdk_3.2.3/platform/service/iostream/src/sl_iostream_rtt.o" "./gecko_sdk_3.2.3/platform/service/iostream/src/sl_iostream_stdlib_config.o" "./gecko_sdk_3.2.3/platform/service/iostream/src/sl_iostream_uart.o" "./gecko_sdk_3.2.3/platform/service/iostream/src/sl_iostream_usart.o" "./gecko_sdk_3.2.3/platform/service/mpu/src/sl_mpu.o" "./gecko_sdk_3.2.3/platform/service/power_manager/src/sl_power_manager.o" "./gecko_sdk_3.2.3/platform/service/power_manager/src/sl_power_manager_debug.o" "./gecko_sdk_3.2.3/platform/service/power_manager/src/sl_power_manager_hal_s2.o" "./gecko_sdk_3.2.3/platform/service/sleeptimer/src/sl_sleeptimer.o" "./gecko_sdk_3.2.3/platform/service/sleeptimer/src/sl_sleeptimer_hal_burtc.o" "./gecko_sdk_3.2.3/platform/service/sleeptimer/src/sl_sleeptimer_hal_prortc.o" "./gecko_sdk_3.2.3/platform/service/sleeptimer/src/sl_sleeptimer_hal_rtcc.o" "./gecko_sdk_3.2.3/platform/service/system/src/sl_system_init.o" "./gecko_sdk_3.2.3/platform/service/system/src/sl_system_kernel.o" "./gecko_sdk_3.2.3/platform/service/udelay/src/sl_udelay.o" "./gecko_sdk_3.2.3/platform/service/udelay/src/sl_udelay_armv6m_gcc.o" "./gecko_sdk_3.2.3/protocol/bluetooth/src/sl_bt_rtos_adaptation.o" "./gecko_sdk_3.2.3/util/silicon_labs/silabs_core/memory_manager/sl_malloc.o" "./gecko_sdk_3.2.3/util/third_party/crypto/mbedtls/library/cipher.o" "./gecko_sdk_3.2.3/util/third_party/crypto/mbedtls/library/cipher_wrap.o" "./gecko_sdk_3.2.3/util/third_party/crypto/mbedtls/library/error.o" "./gecko_sdk_3.2.3/util/third_party/crypto/mbedtls/library/platform.o" "./gecko_sdk_3.2.3/util/third_party/crypto/mbedtls/library/platform_util.o" "./gecko_sdk_3.2.3/util/third_party/crypto/mbedtls/library/psa_crypto.o" "./gecko_sdk_3.2.3/util/third_party/crypto/mbedtls/library/psa_crypto_aead.o" "./gecko_sdk_3.2.3/util/third_party/crypto/mbedtls/library/psa_crypto_cipher.o" "./gecko_sdk_3.2.3/util/third_party/crypto/mbedtls/library/psa_crypto_client.o" "./gecko_sdk_3.2.3/util/third_party/crypto/mbedtls/library/psa_crypto_driver_wrappers.o" "./gecko_sdk_3.2.3/util/third_party/crypto/mbedtls/library/psa_crypto_ecp.o" "./gecko_sdk_3.2.3/util/third_party/crypto/mbedtls/library/psa_crypto_hash.o" "./gecko_sdk_3.2.3/util/third_party/crypto/mbedtls/library/psa_crypto_mac.o" "./gecko_sdk_3.2.3/util/third_party/crypto/mbedtls/library/psa_crypto_rsa.o" "./gecko_sdk_3.2.3/util/third_party/crypto/mbedtls/library/psa_crypto_se.o" "./gecko_sdk_3.2.3/util/third_party/crypto/mbedtls/library/psa_crypto_slot_management.o" "./gecko_sdk_3.2.3/util/third_party/crypto/mbedtls/library/psa_crypto_storage.o" "./gecko_sdk_3.2.3/util/third_party/crypto/mbedtls/library/threading.o" "./gecko_sdk_3.2.3/util/third_party/crypto/sl_component/se_manager/src/sl_se_manager.o" "./gecko_sdk_3.2.3/util/third_party/crypto/sl_component/se_manager/src/sl_se_manager_attestation.o" "./gecko_sdk_3.2.3/util/third_party/crypto/sl_component/se_manager/src/sl_se_manager_cipher.o" "./gecko_sdk_3.2.3/util/third_party/crypto/sl_component/se_manager/src/sl_se_manager_entropy.o" "./gecko_sdk_3.2.3/util/third_party/crypto/sl_component/se_manager/src/sl_se_manager_hash.o" "./gecko_sdk_3.2.3/util/third_party/crypto/sl_component/se_manager/src/sl_se_manager_key_derivation.o" "./gecko_sdk_3.2.3/util/third_party/crypto/sl_component/se_manager/src/sl_se_manager_key_handling.o" "./gecko_sdk_3.2.3/util/third_party/crypto/sl_component/se_manager/src/sl_se_manager_signature.o" "./gecko_sdk_3.2.3/util/third_party/crypto/sl_component/se_manager/src/sl_se_manager_util.o" "./gecko_sdk_3.2.3/util/third_party/crypto/sl_component/sl_alt/source/sl_mbedtls.o" "./gecko_sdk_3.2.3/util/third_party/crypto/sl_component/sl_alt/source/sl_psa_its_nvm3.o" "./gecko_sdk_3.2.3/util/third_party/crypto/sl_component/sl_alt/source/sl_se_management.o" "./gecko_sdk_3.2.3/util/third_party/crypto/sl_component/sl_protocol_crypto/src/sli_protocol_crypto_radioaes.o" "./gecko_sdk_3.2.3/util/third_party/crypto/sl_component/sl_protocol_crypto/src/sli_radioaes_management.o" "./gecko_sdk_3.2.3/util/third_party/crypto/sl_component/sl_psa_driver/src/sli_psa_driver_common.o" "./gecko_sdk_3.2.3/util/third_party/crypto/sl_component/sl_psa_driver/src/sli_psa_driver_init.o" "./gecko_sdk_3.2.3/util/third_party/crypto/sl_component/sl_psa_driver/src/sli_psa_trng.o" "./gecko_sdk_3.2.3/util/third_party/crypto/sl_component/sl_psa_driver/src/sli_se_driver_aead.o" "./gecko_sdk_3.2.3/util/third_party/crypto/sl_component/sl_psa_driver/src/sli_se_driver_builtin_keys.o" "./gecko_sdk_3.2.3/util/third_party/crypto/sl_component/sl_psa_driver/src/sli_se_driver_cipher.o" "./gecko_sdk_3.2.3/util/third_party/crypto/sl_component/sl_psa_driver/src/sli_se_driver_key_derivation.o" "./gecko_sdk_3.2.3/util/third_party/crypto/sl_component/sl_psa_driver/src/sli_se_driver_key_management.o" "./gecko_sdk_3.2.3/util/third_party/crypto/sl_component/sl_psa_driver/src/sli_se_driver_mac.o" "./gecko_sdk_3.2.3/util/third_party/crypto/sl_component/sl_psa_driver/src/sli_se_driver_signature.o" "./gecko_sdk_3.2.3/util/third_party/crypto/sl_component/sl_psa_driver/src/sli_se_opaque_driver_aead.o" "./gecko_sdk_3.2.3/util/third_party/crypto/sl_component/sl_psa_driver/src/sli_se_opaque_driver_cipher.o" "./gecko_sdk_3.2.3/util/third_party/crypto/sl_component/sl_psa_driver/src/sli_se_opaque_driver_mac.o" "./gecko_sdk_3.2.3/util/third_party/crypto/sl_component/sl_psa_driver/src/sli_se_opaque_key_derivation.o" "./gecko_sdk_3.2.3/util/third_party/crypto/sl_component/sl_psa_driver/src/sli_se_transparent_driver_aead.o" "./gecko_sdk_3.2.3/util/third_party/crypto/sl_component/sl_psa_driver/src/sli_se_transparent_driver_cipher.o" "./gecko_sdk_3.2.3/util/third_party/crypto/sl_component/sl_psa_driver/src/sli_se_transparent_driver_hash.o" "./gecko_sdk_3.2.3/util/third_party/crypto/sl_component/sl_psa_driver/src/sli_se_transparent_driver_mac.o" "./gecko_sdk_3.2.3/util/third_party/crypto/sl_component/sl_psa_driver/src/sli_se_transparent_key_derivation.o" "./gecko_sdk_3.2.3/util/third_party/freertos/cmsis/Source/cmsis_os2.o" "./gecko_sdk_3.2.3/util/third_party/freertos/kernel/croutine.o" "./gecko_sdk_3.2.3/util/third_party/freertos/kernel/event_groups.o" "./gecko_sdk_3.2.3/util/third_party/freertos/kernel/list.o" "./gecko_sdk_3.2.3/util/third_party/freertos/kernel/queue.o" "./gecko_sdk_3.2.3/util/third_party/freertos/kernel/stream_buffer.o" "./gecko_sdk_3.2.3/util/third_party/freertos/kernel/tasks.o" "./gecko_sdk_3.2.3/util/third_party/freertos/kernel/timers.o" "./gecko_sdk_3.2.3/util/third_party/freertos/kernel/portable/GCC/ARM_CM33_NTZ/non_secure/port.o" "./gecko_sdk_3.2.3/util/third_party/freertos/kernel/portable/GCC/ARM_CM33_NTZ/non_secure/portasm.o" "./gecko_sdk_3.2.3/util/third_party/freertos/kernel/portable/MemMang/heap_4.o" "./gecko_sdk_3.2.3/util/third_party/freertos/kernel/portable/SiliconLabs/tick_power_manager.o" "./gecko_sdk_3.2.3/util/third_party/segger/systemview/SEGGER/SEGGER_RTT.o" "C:/SiliconLabs/SimplicityStudio/v5/developer/sdks/gecko_sdk_suite/v3.2//protocol/bluetooth/lib/EFR32MG21/GCC/binapploader.o" "C:/SiliconLabs/SimplicityStudio/v5/developer/sdks/gecko_sdk_suite/v3.2//protocol/bluetooth/lib/EFR32MG21/GCC/libbluetooth.a" "C:/SiliconLabs/SimplicityStudio/v5/developer/sdks/gecko_sdk_suite/v3.2//platform/emdrv/nvm3/lib/libnvm3_CM33_gcc.a" "C:/SiliconLabs/SimplicityStudio/v5/developer/sdks/gecko_sdk_suite/v3.2//platform/radio/rail_lib/autogen/librail_release/librail_efr32xg21_gcc_release.a" -lgcc -lc -lm -lnosys -Wl,--end-group -Wl,--start-group -lgcc -lc -lnosys -Wl,--end-group
	@echo 'Finished building target: $@'
	@echo ' '

	@echo 'Building out file: soc_Pairing_Process.out'
	arm-none-eabi-objcopy "soc_Pairing_Process.axf" "soc_Pairing_Process.out"
	@echo ' '

	@echo 'Building hex file: soc_Pairing_Process.hex'
	arm-none-eabi-objcopy -O ihex "soc_Pairing_Process.axf" "soc_Pairing_Process.hex"
	@echo ' '

	@echo 'Building bin file: soc_Pairing_Process.bin'
	arm-none-eabi-objcopy -O binary "soc_Pairing_Process.axf" "soc_Pairing_Process.bin"
	@echo ' '

	@echo 'Building s37 file: soc_Pairing_Process.s37'
	arm-none-eabi-objcopy -O srec "soc_Pairing_Process.axf" "soc_Pairing_Process.s37"
	@echo ' '

	@echo 'Running size tool'
	arm-none-eabi-size "soc_Pairing_Process.axf" -A
	@echo ' '

# Other Targets
clean:
	-@$(foreach FILE, $(EXECUTABLES), $(shell $(RM) $(FILE)) )
	-@$(foreach FILE, $(OBJS), $(shell $(RM) $(FILE)) )
	-@$(foreach FILE, $(C_DEPS), $(shell $(RM) $(FILE)) )
	-$(RM) soc_Pairing_Process.axf
	-@echo ' '

.PHONY: all clean dependents main-build

-include ../makefile.targets
