#---------
#
# CppUTest Examples Makefile
#
#----------

#Set this to @ to keep the makefile quiet
ifndef SILENCE
	SILENCE = @
endif

#--- Inputs ----#
COMPONENT_NAME = TWI
CPPUTEST_HOME = /Users/ssyi/Desktop/cpputest-3.6

CPPUTEST_USE_EXTENSIONS = N
CPP_PLATFORM = Gcc
CPPUTEST_CXXFLAGS += -Wno-old-style-cast

# This line is overriding the default new macros.  This is helpful
# when using std library includes like <list> and other containers
# so that memory leak detection does not conflict with stl.
#CPPUTEST_MEMLEAK_DETECTOR_NEW_MACRO_FILE = -include ApplicationLib/ExamplesNewOverrides.h
SRC_DIRS = \
	src

TEST_SRC_DIRS = \
	tests

INCLUDE_DIRS =\
  .\
  include\
  $(CPPUTEST_HOME)/include\

include $(CPPUTEST_HOME)/build/MakefileWorker.mk


