# Minimal makefile for Sphinx documentation
#

# You can set these variables from the command line, and also
# from the environment for the first two.
SPHINXOPTS    ?=
SPHINXBUILD   ?= sphinx-build
SOURCEDIR     = source
BUILDDIR      = build

# Put it first so that "make" without argument is like "make help".
help:
	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)

.PHONY: help Makefile

# Catch-all target: route all unknown targets to Sphinx using the new
# "make mode" option.  $(O) is meant as a shortcut for $(SPHINXOPTS).
%: Makefile
	@$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)

.PHONY: dist
dist: html
	rm -rf $(BUILDDIR)/linuxmint-fuer-anwender $(BUILDDIR)/linuxmint-fuer-anwender.zip
	mkdir -p $(BUILDDIR)/linuxmint-fuer-anwender
	cd $(BUILDDIR)/html && zip -q -r ../linuxmint-fuer-anwender/html.zip .
	-cp $(BUILDDIR)/latex/*.pdf $(BUILDDIR)/linuxmint-fuer-anwender/ 2>/dev/null || true
	cd $(BUILDDIR)/linuxmint-fuer-anwender && zip -q -r ../linuxmint-fuer-anwender.zip .
	@echo ""
	@echo "=========================================================="
	@echo "Package successfully created at:"
	@echo "docs/$(BUILDDIR)/linuxmint-fuer-anwender.zip"
	@echo "=========================================================="

