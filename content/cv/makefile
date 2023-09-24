##
# Make all four CVs - English-Long, English-Short, German-Long, German-Short, cleanup unused files.
# Make my CVs
#
# @file
# @version 0.1
ENGLISH_OPT   =\AtBeginDocument{\toggletrue{ENGLISH}}
LONGCV_OPT     =\AtBeginDocument{\toggletrue{LONGCV}}

all: english-short english-long german-short german-long

english-short:
	latexmk -pdf -usepretex="$(ENGLISH_OPT)"
	latexmk -c
	mv cv.pdf sibaev-cv-english.pdf

english-long:
	latexmk -pdf -usepretex="$(ENGLISH_OPT)$(LONGCV_OPT)"
	latexmk -c
	mv cv.pdf sibaev-cv-english-long.pdf


german-short:
	latexmk -pdf
	latexmk -c
	mv cv.pdf sibaev-cv-german.pdf

german-long:
	latexmk -pdf -usepretex="$(LONGCV_OPT)"
	latexmk -c
	mv cv.pdf sibaev-cv-german-long.pdf

# end
