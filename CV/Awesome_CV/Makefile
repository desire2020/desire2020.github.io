SOURCES := cv.tex awesome-cv.cls $(wildcard cv/*.tex)

.PHONY: all publish clean

all: cv.pdf

cv.pdf: $(SOURCES)
	latexmk -xelatex -interaction=nonstopmode -halt-on-error cv.tex

publish: cv.pdf
	install -m 0644 cv.pdf ../SidiLu.pdf

clean:
	latexmk -c cv.tex
