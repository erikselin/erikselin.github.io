LITERATURE_REVIEW := literature_review
FINAL_PAPER := final_paper

default: litrev presout

litrev:
	latex -draftmode ${LITERATURE_REVIEW}
	bibtex ${LITERATURE_REVIEW}
	latex -draftmode ${LITERATURE_REVIEW}
	pdflatex ${LITERATURE_REVIEW}
	rm ${LITERATURE_REVIEW}.aux
	rm ${LITERATURE_REVIEW}.bbl
	rm ${LITERATURE_REVIEW}.blg
	rm ${LITERATURE_REVIEW}.log
	rm ${LITERATURE_REVIEW}.dvi

presout:
	latex -draftmode ${FINAL_PAPER}
	bibtex ${FINAL_PAPER}
	latex -draftmode ${FINAL_PAPER}
	pdflatex ${FINAL_PAPER}
	rm ${FINAL_PAPER}.aux
	rm ${FINAL_PAPER}.bbl
	rm ${FINAL_PAPER}.blg
	rm ${FINAL_PAPER}.log
	rm ${FINAL_PAPER}.dvi

clean:
	rm *.aux
	rm *.bbl
	rm *.blg
	rm *.dvi
	rm *.log
