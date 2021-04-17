DOCNAME=essderc2k21

all: report

.PHONY: clean

report:
	pdflatex $(DOCNAME).tex
	bibtex $(DOCNAME).aux
	pdflatex $(DOCNAME).tex
	pdflatex $(DOCNAME).tex
	cp -f $(DOCNAME).pdf ${HOME}
view: report
	okular $(DOCNAME).pdf

clean:
	rm *.blg *.bbl *.aux *.lo
