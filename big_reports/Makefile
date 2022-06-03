#
# LateX Makefile
# 

all: $(FILE).tex
	pdflatex $(FILE) && bibtex $(FILE)||true && pdflatex $(FILE) && pdflatex $(FILE)
	firefox $(FILE).pdf & 
	mkdir -p build
	mv report.{aux,bbl,blg,log,out,run.xml,toc} report-blx.bib build

clean: 
	rm -rfv build
