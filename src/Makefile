

DOC = draft.pdf

all: $(DOC)


%.pdf: %.tex
	pdflatex $<

clean:
	rm -f *.aux *.dvi *.log *.pdf
