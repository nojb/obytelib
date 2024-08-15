###########################################################################
##                                                                       ##
##                              OByteLib                                 ##
##                                                                       ##
##                            Benoit Vaugon                              ##
##                                                                       ##
##    This file is distributed under the terms of the CeCILL license.    ##
##    See file ../LICENSE-en.                                            ##
##                                                                       ##
###########################################################################

include ../etc/Makefile.conf

_build/%: $(SRCS) prim.ml config.ml
	@rm -f $@
	$(OCAMLBUILD) -cflag -g -lflag -g $*

config.ml: ../etc/config.ml
	cp $< $@

prim.ml: ../etc/prim.ml
	cp $< $@
