pdf-clean: pdf clean-aux

pdf:
	pdflatex CRC-cards.tex
	pdflatex user-story.tex
	pdflatex UML-sequence.tex
	pdflatex UML-diagram.tex
	pdflatex report.tex

clean-pdf:
	rm *.pdf

clean-aux:
	rm *.log
	rm *.aux
	rm *.out

release: pdf clean-aux
	zip GrT-OOC.zip *.pdf README.txt
