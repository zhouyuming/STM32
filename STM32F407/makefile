TARGET = stm32test

DEBUG = 1

OPT = #-Og

BUILD_DIR = build

C_SOURCES =  \

# ASM sources
ASM_SOURCES =  \
startup_stm32f407xx.s

# ASMM sources
ASMM_SOURCES = 

# ASMMC sources
ASMMC_SOURCE = 

PREFIX = arm-none-eabi-

ifdef GCC_PATH
CC = $(GCC_PATH)/$(PREFIX)gcc
AS = $(GCC_PATH)/$(PREFIX)gcc -x assembler-with-cpp
CP = $(GCC_PATH)/$(PREFIX)objcopy
SZ = $(GCC_PATH)/$(PREFIX)size
else
CC = $(PREFIX)gcc
AS = $(PREFIX)gcc -x assembler-with-cpp
CP = $(PREFIX)objcopy
SZ = $(PREFIX)size
endif
HEX = $(CP) -O ihex
BIN = $(CP) -O binary -S

CPU = -mcpu=cortex-m4

FPU = -mfpu=fpv4-sp-d16

FLOAT-ABI = -mfloat-abi=hard

MCU = $(CPU) -mthumb $(FPU) $(FLOAT-ABI)

AS_DEFS =

