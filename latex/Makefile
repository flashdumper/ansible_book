LATEX=/Library/TeX/texbin/latex
TOPDF=/Library/TeX/texbin/dvipdf
SOURCE=main
SRC2PDF=/Library/TeX/texbin/pdflatex --file-line-error --synctex=1

all: src2pdf

dvi:
		${LATEX} ${SOURCE}.tex

dvi2pdf: dvi
		${TOPDF} ${SOURCE}.dvi

pdf: dvi2pdf


src2pdf:
		${SRC2PDF} ${SOURCE}.tex


clean:
		rm -f ${SOURCE}.{log,aux}

