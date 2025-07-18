all: slides_ganong_et_al_2020.pdf

slides_ganong_et_al_2020.pdf: slides_ganong_et_al_2020.tex
	pdflatex -draftmode $<
	pdflatex $<
	rm $(addprefix $(basename $<),.log .aux .out .toc)
	rm $(addprefix $(basename $<),.snm .nav)
	rm $(addprefix $(basename $<),.blg .bbl)

# bibtex slides.aux