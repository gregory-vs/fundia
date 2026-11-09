MAIN=main.tex

.PHONY: all pdf watch clean

all: pdf

pdf:
	mkdir -p build
	latexmk -pdf -interaction=nonstopmode -synctex=1 -outdir=build $(MAIN)

watch:
	mkdir -p build
	latexmk -pdf -interaction=nonstopmode -synctex=1 -pvc -outdir=build $(MAIN)

clean:
	latexmk -c
	rm -rf build
