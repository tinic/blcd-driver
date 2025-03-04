# Must be name of the .kicad_pro, .kicad_pcb and root .kicad_sch
PROJECT_NAME ?= $(basename $(wildcard *.kicad_pro))
# Directory containing PROJECT_NAME.kicad_* files
PROJECT_ROOT = .

# Can be a string or number indicating release revision
# REVISION = 0
# Define and set to 1 to limit info output
# KICADMK_QUIET = 1
# Define and set to 1 to append git describe tag and hash to export zips
# KICADMK_APPEND_GIT ?= 1
# Define and set to 0 to not generate log of variables to include in exports
# KICADMK_INCLUDE_LOG = 1
# Define and set to 1 to print the log content at start to shell
# KICADMK_PRINT_LOG = 0
# Set to 1 to generate separated pdf and/or svg with pcb files
# PCB_SEPARATE_PDF = 1
# PCB_SEPARATE_SVG = 1
# Define the PCB copper layers
PCB_COPPER_LAYERS = "F.Cu,B.Cu"
# Substitutes VRML models with STEP/IGS models, which are more widely supported
STEP_FLAGS = --subst-models

# Define a command that generates a BoM - kibom installed with pip by default but could be path to Python script
# ?= a good idea so that a CI and override this with a env
BOM_CMD ?= python3 -m kibom
# BOM_CMD ?= python3 ~/KiBoM/KiBOM_CLI.py
# KiBoM by default creates output with _bom_REV.csv appended, pass a config file to it to match target BoM name
# BOM_CMD_FLAGS = --cfg $(PROJECT_ROOT)/bom.ini

# Location of KiCad Makefile repository if not defined in environment, eg: export KICADMK_DIR=/home/me/kicad-makefile
# KICADMK_DIR = ./kicad-makefile

# Optionally include a supplier Makefile to define flags used by that supplier
# include $(KICADMK_DIR)/suppliers/PCBWay.mk

# Include the KiCad Makefile
include $(KICADMK_DIR)/Kicad.mk
