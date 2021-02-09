TEX = xelatex
BIB = bibtex

all : test.pdf

bib : 
	$(TEX) -jobname=output hello.tex
	$(BIB)	output.aux
	$(TEX) -jobname=output hello.tex
	$(TEX) -jobname=output hello.tex

test.pdf : hello.tex
	$(TEX) -shell-escape -jobname=output hello.tex

clean : 
	rm output*
