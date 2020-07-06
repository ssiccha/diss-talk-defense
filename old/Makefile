# Settings
TARGET=main
PREFIX=Socle
OUTNAME=2019-Siegen-Quasipolynomial-normalisers-category-permutation-groups
TEX=latexmk --pdf -file-line-error -halt-on-error

# Rules
all : $(OUTNAME).pdf
.PHONY: all, clean

$(OUTNAME).pdf : *.tex references.bib
	$(TEX) $(TARGET).tex && mv $(TARGET).pdf $(OUTNAME).pdf

clean :
	rm -f $(TARGET).pdf *.aux *.bcf *.bbl *.blg *.fls \
	    *.fdb_latexmk *.log *.nav *.out *.run.xml *.snm *.toc *.xyc
