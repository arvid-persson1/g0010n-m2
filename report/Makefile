MAIN = main

TRASH = $(MAIN).aux $(MAIN).bcf $(MAIN).log $(MAIN).run.xml $(MAIN).bbl $(MAIN).blg $(MAIN).toc

$(MAIN).pdf: *.tex references.bib
	pdflatex $(MAIN) > /dev/null
	biber $(MAIN)    > /dev/null
	pdflatex $(MAIN) > /dev/null
	pdflatex $(MAIN) > /dev/null

clean:
	rm -f $(TRASH)

.PHONY: clean

