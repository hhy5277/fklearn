# Minimal makefile for Sphinx documentation
#

# You can set these variables from the command line.
SPHINXBUILD   = sphinx-build
SPHINXPROJ    = fklearn
SOURCEDIR     = source
BUILDDIR      = build
APIDOC        = sphinx-apidoc
APIDOCDIR     = source/api
PROJECTDIR    = ../src/fklearn

# Put it first so that "make" without argument is like "make help".
help:
	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(O)

.PHONY: help Makefile

apidoc:
	$(APIDOC) -o "$(APIDOCDIR)" "$(PROJECTDIR)"

# Catch-all target: route all unknown targets to Sphinx using the new
# "make mode" option.  $(O) is meant as a shortcut for $(SPHINXOPTS).
%: Makefile
	@$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(O)
