#!/usr/bin/make -f
# Makefile for DISTRHO Plugins #

NAME = drumcloud

FILES_DSP = \
        SendNoteExamplePlugin.cpp \
        AudioFileLoader.cpp

FILES_UI = \
        DrumCloudUI.cpp \
        AudioFileLoader.cpp

DPF_TARGET_DIR = ../bin
DPF_BUILD_DIR = ../build
DPF_PATH = ../dep/dpf

include ../dep/dpf/Makefile.plugins.mk


# Use C++17
CXXFLAGS += -std=gnu++17

BUILD_C_FLAGS += -I ../dep/dr_libs
BUILD_CXX_FLAGS += -I ../dep/dr_libs

UI_TYPE = opengl

TARGETS += lv2
TARGETS += vst2
TARGETS += vst3
TARGETS += clap

all: $(TARGETS)
