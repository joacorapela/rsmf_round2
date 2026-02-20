all: eoi.pdf

eoi.pdf: eoi.tex maturityAndUKresearchBenefit.tex motivationVisionAndImpact.tex benefitToUK.tex edia.tex proposedWork.tex sustainability.tex deliveryTeamAndMechanisms.tex
	pdflatex eoi.tex
	bibtex eoi.aux
	pdflatex eoi.tex
	pdflatex eoi.tex
