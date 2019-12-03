   _____      __                  
  / ___/___  / /_      __  ______ 
  \__ \/ _ \/ __/_____/ / / / __ \
 ___/ /  __/ /_/_____/ /_/ / /_/ /
/____/\___/\__/      \__,_/ .___/ 
                         /_/      
0.Set-up
The set-up is done inside of "main.tex"

Line 8 has the document font size
Line 23-24 sets the schools name, city, and department
Line 33 set the course name
line 34-36 set the title(s). Note leaving them blank "{}" hides them
Line 42,45,48,51 set the students name(s). Note leaving them blank "{}" hides them
Line 55,49,63 set the Teacher/Examiner/Supervisor names, fill in the title yourself. . Note leaving them blank "{}" hides them
Line 68 if you do not want the document to have today's date on it it can be set here, for auto leave it as \def\tDate{\today}
Line 71,72 set the document header, this is seen on every page except front and abstract
Line 123 if you do not want a summary change this line to  \def\mPrintSummary{} if you want a summary please add something with in the curly brackets
Line 139 is for abbreviations if not used please comment out these line by appending a %
line 142 holds the table of contents if not needed please comment out these line by appending a %
line 145 holds the list of listing (code) if not needed please comment out these line by appending a %
line 148 holds the list of figures if not needed please comment out these line by appending a %
line 151 holds the list of tables if not needed please comment out these line by appending a %

If you want to add a new section or remove a section this is done in lines 162-184 the format is \input{path-to-.tex-file}
If you do not want new pages after etch section please remove or comment out (appending %) the \newline between lines 161-185
If you want your references and appendix to be use roman numerals please uncomment out line 189

if you do not want appendix to be present please comment out line 196-199

If you want paragrafs to look like Example 1 and want it to look like example 2, plese uncomment line 94 in "./staticpreamble.sty" and add "\\" after each paragraph

Example 1:
text text text text text text text
    new paragraph text text text t
ext text text text text text

Example 2:
text text text text text text text

text text text text text text text
text text text text

    _   __            _             __  _           
   / | / /___ __   __(_)___ _____ _/ /_(_)___  ____ 
  /  |/ / __ `/ | / / / __ `/ __ `/ __/ / __ \/ __ \
 / /|  / /_/ /| |/ / / /_/ / /_/ / /_/ / /_/ / / / /
/_/ |_/\__,_/ |___/_/\__, /\__,_/\__/_/\____/_/ /_/ 
                    /____/                          
1.Navigation

1.1 Text
Text can be found in the folder named "text" etch section is split in to its own file

1.2 Refrences and Bibtex
References is found a the path "./static/bibilio.bib" this is a bibtex file
    for examples and cheat sheet for formatting, please see: https://verbosus.com/bibtex-style-examples.html
    for automatic generation of bibtex file please see:
        Note: Scientifically articles generally have a download citation button. Primo has a button named "Export bibtex"
        http://www.citationmachine.net/bibtex/cite-a-website
        http://www.bibme.org/bibtex
        https://www.doi2bib.org/
        https://www.xarg.org/tools/isbn-to-bibtex/

1.2.1 in text refrences
in text refaces is done with either \textcite[OPTINAL-PAGE-INFORMATION]{bibtex-Refence-name} for name (Year, OPTINAL-PAGE-INFORMATION) and \parencite[OPTINAL-PAGE-INFORMATION]{bibtex-Refence-name} for (name, Year, OPTINAL-PAGE-INFORMATION)

1.3 Images
Picture should be placed in "./pics", picture should hopefully be svg for smaller size and better "resolution"

1.4 Tables
Tables can be automatically generated from these sites
    https://www.latex-tables.com/
    https://www.tablesgenerator.com/

1.5 Section depth
1 \section{section}
1.1 \subsection{subsection}
1.1.1 \subsubsection{subsubsection}
1.1.1.1 \paragraph{paragraph}

1.6 Abbreviations
This is done in the "./text/abbreviations.tex" to add new abbrivations and reffence using the following syntax \gls{abbRefName}


1.7 Figure

referenced with Figure \ref{FIGlable}

\begin{figure}[h]
	\centering
	\includegraphics[width=0.25 \textwidth]{Path to pic}
	\caption{Figure caption}
    \label{FIGlable}
\end{figure}

1.8 List
\begin{enumerate}
    \item bullet item
\end{enumerate}

\begin{itemize}
    \item numbered item
\end{itemize}

\begin{description}
    \item[name] discription
\end{description}

1.9 code/listings

code is done by using lstlisting please look here (https://en.wikibooks.org/wiki/LaTeX/Source_Code_Listings) for more information

    __  __     __    
   / / / /__  / /___ 
  / /_/ / _ \/ / __ \
 / __  /  __/ / /_/ /
/_/ /_/\___/_/ .___/ 
            /_/      
2.Help

How do I add character X,Y, and Z
    look here https://www.nyu.edu/projects/beber/files/Chang_LaTeX_sheet.pdf if it is not in there Google

How do I do X,Y, or Z and I get error A,B, and C
    1. Google



    ______                           __         
   / ____/  ______ _____ ___  ____  / /__  _____
  / __/ | |/_/ __ `/ __ `__ \/ __ \/ / _ \/ ___/
 / /____>  </ /_/ / / / / / / /_/ / /  __(__  ) 
/_____/_/|_|\__,_/_/ /_/ /_/ .___/_/\___/____/  
                          /_/                   
3.Examples of this template

Some examples of my and my fellow students at MDH bachelor thesis witch used some version of this template
http://urn.kb.se/resolve?urn=urn:nbn:se:mdh:diva-44152
http://urn.kb.se/resolve?urn=urn:nbn:se:mdh:diva-44035
http://urn.kb.se/resolve?urn=urn:nbn:se:mdh:diva-44115



    __    _                              
   / /   (_)_______  ____  ________      
  / /   / / ___/ _ \/ __ \/ ___/ _ \     
 / /___/ / /__/  __/ / / (__  )  __/     
/_____/_/\___/\___/_/ /_/____/\___/      
                                         
4.License
This template is free to modify, change, and distribute. But, please give credit in the template (not rendered document) to the authors of this template, Mikael Andersson and the whole Network engineering class of 2016 (MDH) for making version 3 named (TeX Mall v3) and Johannes Henriksson for updating and maintaining this fork of the template and changing it from MDH to ORU and making it ORU compliant.



   ________                              __               
  / ____/ /_  ____ _____  ____ ____     / /   ____  ____ _
 / /   / __ \/ __ `/ __ \/ __ `/ _ \   / /   / __ \/ __ `/
/ /___/ / / / /_/ / / / / /_/ /  __/  / /___/ /_/ / /_/ / 
\____/_/ /_/\__,_/_/ /_/\__, /\___/  /_____/\____/\__, /  
                       /____/                    /____/   
5.Change log

v4.1
- added abbreviation
- added section text and explanation text form MDH thesis document
- added example text
- Translated text to English
- Moved pics folder for static to root

v4.0
- Change to compile with ORU
- removed logo
- Restructured and organized folders