all: slides_almagro_et_al_2024.pdf

slides_almagro_et_al_2024.pdf: slides_almagro_et_al_2024.tex
	pdflatex -draftmode $<
	pdflatex $<
	rm $(addprefix $(basename $<),.log .aux .out .toc)
	rm $(addprefix $(basename $<),.snm .nav)
	rm $(addprefix $(basename $<),.blg .bbl)

# bibtex slides.aux