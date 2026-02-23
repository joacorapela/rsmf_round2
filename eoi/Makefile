all: eoi.pdf eoiWithoutInstructions.pdf

eoi.pdf: eoi.tex maturityAndUKresearchBenefit.tex motivationVisionAndImpact.tex benefitToUK.tex edia.tex proposedWork.tex sustainability.tex deliveryTeamAndMechanisms.tex
	pdflatex eoi.tex
	bibtex eoi.aux
	pdflatex eoi.tex
	pdflatex eoi.tex

eoiWithoutInstructions.pdf: eoiWithoutInstructions.tex maturityAndUKresearchBenefit.tex motivationVisionAndImpact.tex benefitToUK.tex edia.tex proposedWork.tex sustainability.tex deliveryTeamAndMechanisms.tex
	pdflatex eoiWithoutInstructions.tex
	bibtex eoiWithoutInstructions.aux
	pdflatex eoiWithoutInstructions.tex
	pdflatex eoiWithoutInstructions.tex

