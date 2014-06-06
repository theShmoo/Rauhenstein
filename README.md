#Rauhenstein

This project is a style file for latex that helps to create beautiful plannings for scouting activities

##Usage

You have to compile the pages from LaTeX -> PS -> PDF to get the eps working!

There are 3 possible styles for the startpage of a new document:

### Planung

__Example:__
```TeX
\documentclass[a4paper, 12pt]{article}
\usepackage[planung]{rauhenstein}
\usepackage{blindtext}
\planungsdatum{28.11.2013}			%required
\ort{im Heim}						%required
\thema{Patrullenrat Heimstunde}		%required
\durchfuehrungsdatum{28.11.2013}	%optional
\untertitel{Reflexion zur}			%optional
\schreiber{David}					%optional
\planende{Jakob, Lisi}				%optional
\planungsort{Jakobs Hood}			%optional
\foto{rauhenstein}					%optional
\begin{document}
\rauhenstein
```

### Besichtigung

__Example:__
```TeX
\documentclass[a4paper, 12pt]{article}
\usepackage[besichtigung]{rauhenstein}
\planungsdatum{28.11.2013}			%required
\ort{auf der Wiese}					%required
\durchfuehrungsdatum{28.11.2013}	%optional
\schreiber{David}					%optional
\planende{Jakob, Lisi}				%optional
\planungsort{Jakobs Hood}			%optional
\begin{document}
\rauhenstein
```

### Kurzes Protokoll

__Example:__
```TeX
\documentclass[a4paper, 12pt]{article}
\usepackage[kurzesprotokoll]{rauhenstein}
\planungsdatum{28.11.2013}			%required
\ort{im Heim}						%required
\durchfuehrungsdatum{28.11.2013}	%optional
\schreiber{David}					%optional
\planende{Jakob, Lisi}				%optional
\planungsort{Jakobs Hood}			%optional
\begin{document}
\rauhenstein
```

##Installation

Creating a local package repository :

![Creating a local package repository](https://raw.githubusercontent.com/theShmoo/Rauhenstein/master/create_local_repo.png)

Press Add and add a folder that has the following folder structure:
* Local Tex Files
  * bibtex
    * bib
      * misc
  * bst
    * misc
  * dict
  * tex
    *latex
      *misc

Put the following files into the subfolder: _Local Tex Files/tex/latex/misc_

* gusp.eps (GuSp Logo)
* rauhenstein.eps (Rauhenstein Trupp Logo)
* rauhenstein.sty (Latex Style File)
* rauhenstein-bg.eps (Rauhenstein Trupp Logo Black and White)

Refresh database with miktex
 