export SRC	= presentation
export LATEX	= pdflatex

D_SRC	= src
OUT	= presentation.pdf

$(OUT) : 
	make -C $(D_SRC)
	mv $(D_SRC)/$(SRC).pdf $(OUT)
	
view : 
	make -C $(D_SRC)
	mv $(D_SRC)/$(SRC).pdf $(OUT)
	evince $(OUT)

clean :
	-rm *.log
	-make -C $(D_SRC) $@

cleanall : clean
	-rm $(OUT)
	
