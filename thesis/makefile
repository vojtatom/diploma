TEX = pdflatex
BIB = bibtex
GLO = makeglossaries
MAIN = DP_Tomas_Vojtech_2021.tex

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
	find output* | grep -v .pdf | xargs rm
	find DP_Tomas_Vojtech_2021* | grep -v .tex | xargs rm