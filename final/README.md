#   LaTeX setup for short paper
A UNIX Makefile compiling the .tex and resolving all citations is included.

bibliography.bib holds all the references in BibTeX format, readily available from the academic journal webpages.
##  Building
    	make

resolves bibtex citations and builds a dvi.

	make pdf

resolves bibtex citations and builds a pdf.

	make clean

removes .aux .log etc..

##  Bibliography
References in BibTeX format, readily available from the academic journal
webpage or Google Scholar.

Add your BibTeX-formatted references to:
    func_oop_testing.bib

##  Vim
I do something like this for a hotkey binding in vim:

	nmap <F9> :!make clean && make pdf<CR> 

Within vim, this command makes sure you're in path:

	:lcd %:h

vim-latexsuite is comfy! you milage may vary..

These settings also makes vim happy:
    set wrap
    set linebreak  
    set nolist
    set wrapmargin=0
    set textwidth=0

Many pdf-viewers common on a GNU/Linux setup, such a Evince will auto-reload an
updated document.
