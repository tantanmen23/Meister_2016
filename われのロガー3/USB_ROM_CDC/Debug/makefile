################################################################################
# Automatically-generated file. Do not edit!
################################################################################

-include ../makefile.init

RM := rm -rf

# All of the sources participating in the build are defined here
-include sources.mk
-include src/subdir.mk
-include subdir.mk
-include objects.mk

ifneq ($(MAKECMDGOALS),clean)
ifneq ($(strip $(C_DEPS)),)
-include $(C_DEPS)
endif
endif

-include ../makefile.defs

# Add inputs and outputs from these tool invocations to the build variables 

# All Target
all: USB_ROM_CDC.axf

dependents:
	-cd C:/Users/Yusuke/Documents/LPCXpresso_8.1.4_606/workspace/CMSISv2p00_LPC11Uxx/Debug && $(MAKE) clean all
	-cd C:/Users/Yusuke/Documents/LPCXpresso_8.1.4_606/workspace/USB_ROM_CDC/Release && $(MAKE) clean all
	-cd C:/Users/Yusuke/Documents/LPCXpresso_8.1.4_606/workspace/LPC11Uxx_Driver_Lib/Debug && $(MAKE) clean all

# Tool invocations
USB_ROM_CDC.axf: $(OBJS) $(USER_OBJS) C:/Users/Yusuke/Documents/LPCXpresso_8.1.4_606/workspace/CMSISv2p00_LPC11Uxx/Debug/libCMSISv2p00_LPC11Uxx.a C:/Users/Yusuke/Documents/LPCXpresso_8.1.4_606/workspace/USB_ROM_CDC/Release/USB_ROM_CDC.axf C:/Users/Yusuke/Documents/LPCXpresso_8.1.4_606/workspace/LPC11Uxx_Driver_Lib/Debug/libLPC11Uxx_Driver_Lib.a
	@echo 'Building target: $@'
	@echo 'Invoking: MCU Linker'
	arm-none-eabi-gcc -nostdlib -L"C:\Users\Yusuke\Documents\LPCXpresso_8.1.4_606\workspace\CMSISv2p00_LPC11Uxx\Debug" -L"C:\Users\Yusuke\Documents\LPCXpresso_8.1.4_606\workspace\USB_ROM_CDC\inc" -L"C:\Users\Yusuke\Documents\LPCXpresso_8.1.4_606\workspace\LPC11Uxx_Driver_Lib\Debug" -Xlinker -Map="USB_ROM_CDC.map" -Xlinker --gc-sections -mcpu=cortex-m0 -mthumb -T "USB_ROM_CDC_Debug.ld" -o "USB_ROM_CDC.axf" $(OBJS) $(USER_OBJS) $(LIBS)
	@echo 'Finished building target: $@'
	@echo ' '
	$(MAKE) --no-print-directory post-build

# Other Targets
clean:
	-$(RM) $(EXECUTABLES)$(OBJS)$(C_DEPS) USB_ROM_CDC.axf
	-@echo ' '

post-build:
	-@echo 'Performing post-build steps'
	-arm-none-eabi-size "USB_ROM_CDC.axf"; # arm-none-eabi-objcopy -O binary "USB_ROM_CDC.axf" "USB_ROM_CDC.bin" ; checksum -p LPC11U35_501 -d "USB_ROM_CDC.bin";
	-@echo ' '

.PHONY: all clean dependents
.SECONDARY: post-build
C:/Users/Yusuke/Documents/LPCXpresso_8.1.4_606/workspace/CMSISv2p00_LPC11Uxx/Debug/libCMSISv2p00_LPC11Uxx.a:
C:/Users/Yusuke/Documents/LPCXpresso_8.1.4_606/workspace/USB_ROM_CDC/Release/USB_ROM_CDC.axf:
C:/Users/Yusuke/Documents/LPCXpresso_8.1.4_606/workspace/LPC11Uxx_Driver_Lib/Debug/libLPC11Uxx_Driver_Lib.a:

-include ../makefile.targets
