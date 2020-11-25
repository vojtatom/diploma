TEX = xelatex
BIB = bibtex
GLO = makeglossaries
MAIN = main.tex

all : main

bib : 
	$(TEX) -jobname=output $(MAIN)
	$(BIB)	output.aux
	$(TEX) -jobname=output $(MAIN)
	$(TEX) -jobname=output $(MAIN)

main :
	$(TEX) -jobname=output $(MAIN)

glo:
	$(TEX) -jobname=output $(MAIN)
	$(GLO) output
	$(TEX) -jobname=output $(MAIN)

tot :
	$(TEX) -jobname=output $(MAIN)
	$(GLO) output
	$(BIB)	output.aux
	$(TEX) -jobname=output $(MAIN)
	$(TEX) -jobname=output $(MAIN)
clean : 
	find *.aux | xargs rm
	find output* | grep -v .pdf | xargs rm
	find main* | grep -v .tex | xargs rm