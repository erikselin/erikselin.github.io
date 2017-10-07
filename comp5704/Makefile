LITERATURE_REVIEW := literature_review

default:
	latex -draftmode ${LITERATURE_REVIEW}
	bibtex ${LITERATURE_REVIEW}
	latex -draftmode ${LITERATURE_REVIEW}
	pdflatex ${LITERATURE_REVIEW}
	rm ${LITERATURE_REVIEW}.aux
	rm ${LITERATURE_REVIEW}.bbl
	rm ${LITERATURE_REVIEW}.blg
	rm ${LITERATURE_REVIEW}.log
	rm ${LITERATURE_REVIEW}.dvi

clean:
	rm *.aux
	rm *.bbl
	rm *.blg
	rm *.dvi
	rm *.log
