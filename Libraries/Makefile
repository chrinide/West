# Makefile for Libraries

default: all

all: title json_do base64_do

json_do:
	if test -d Json ; then \
	( cd Json ; if test "$(MAKE)" = "" ; then make $(MFLAGS) all; \
	else $(MAKE) $(MFLAGS) all ; fi ) ; fi

base64_do:
	if test -d Base64 ; then \
	( cd Base64 ; if test "$(MAKE)" = "" ; then make $(MFLAGS) all; \
	else $(MAKE) $(MFLAGS) all ; fi ) ; fi

clean: json_undo base64_undo 

json_undo:
	if test -d Json ; then \
	( cd Json ; if test "$(MAKE)" = "" ; then make clean ; \
	else $(MAKE) clean ; fi ) ; fi

base64_undo:
	if test -d Base64 ; then \
	( cd Base64 ; if test "$(MAKE)" = "" ; then make clean ; \
	else $(MAKE) clean ; fi ) ; fi

distclean: clean

title :
	@echo "              "
	@echo "##############"
	@echo "## Libraries #"
	@echo "##############"
	@echo "              "
