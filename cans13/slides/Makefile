LX = latex
PP = ps2pdf
PX = pdflatex
BX = bibtex
DP = dvips
AR = evince

TEXFLAGS = -interaction=nonstopmode -enable-installer
SOURCEDIR = ./
FILEN = cans13

all:
	-$(LX) $(TEXFLAGS) $(FILEN)
	-$(BX) $(FILEN)
	-$(LX) $(TEXFLAGS) $(FILEN)
	-$(LX) $(TEXFLAGS) $(FILEN)
	-$(DP) $(FILEN)
	-$(PP) $(FILEN).ps

view:
	-$(AR) $(FILEN).pdf &

clean:
	-@$(RM) *.pdf
	-@$(RM) *~
	-@$(RM) *.aux
	-@$(RM) *.log
	-@$(RM) *.out
	-@$(RM) *.bbl
	-@$(RM) *.blg
	-@$(RM) *.toc
	-@$(RM) latexSuiteTemp*
	-@$(RM) *.dvi
	-@$(RM) *.ps
	-@$(RM) *.swp
	-@$(RM) *.lof
	-@$(RM) *.lot
	-@$(RM) *.idx
	-@$(RM) *.ilg
	-@$(RM) *.ind
	-@$(RM) *.nav
	-@$(RM) *.snm

quick:
	-$(LX) $(TEXFLAGS) $(FILEN)
	-$(DP) $(FILEN)
	-$(PP) $(FILEN).ps
	-$(AR) $(FILEN).pdf &

cleanall:
	-@$(RM) *~
	-@$(RM) *.aux
	-@$(RM) *.log
	-@$(RM) *.out
	-@$(RM) *.bbl
	-@$(RM) *.blg
	-@$(RM) *.toc
	-@$(RM) latexSuiteTemp*
	-@$(RM) *.dvi
	-@$(RM) *.ps
	-@$(RM) *.pdf
	-@$(RM) *.swp
	-@$(RM) *.lof
	-@$(RM) *.lot
	-@$(RM) *.idx
	-@$(RM) *.ilg
	-@$(RM) *.ind
	-@$(RM) *.nav
	-@$(RM) *.snm
