TOP        = ../..
SWIG       = $(TOP)/../preinst-swig
SRCS       = multimap.c
TARGET     = example
INTERFACE  = example.i
SWIGOPT    =

check: build
	$(MAKE) -f $(TOP)/Makefile SRCS='$(SRCS)' TARGET='$(TARGET)' INTERFACE='$(INTERFACE)' go_run

build:
	$(MAKE) -f $(TOP)/Makefile SRCS='$(SRCS)' SWIG='$(SWIG)' \
	SWIGOPT='$(SWIGOPT)' TARGET='$(TARGET)' INTERFACE='$(INTERFACE)' go

clean:
	$(MAKE) -f $(TOP)/Makefile INTERFACE='$(INTERFACE)' go_clean
