#
# Makefile
#
# Makefile for macchina.io WebTunnel bundle
#

include $(POCO_BASE)/build/rules/global

include $(POCO_BASE)/OSP/BundleCreator/BundleCreator.make

objects = BundleActivator

target         = io.macchina.protocols.webtunnel
target_version = 1
target_libs    = PocoWebTunnel PocoOSP PocoNet PocoUtil PocoXML PocoJSON PocoFoundation

postbuild      = $(SET_LD_LIBRARY_PATH) $(BUNDLE_TOOL) -n$(OSNAME) -a$(OSARCH) -o../bundles WebTunnel.bndlspec

include $(POCO_BASE)/build/rules/dylib
